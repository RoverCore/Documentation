
---
title: "DI - Dependency Injection"
linkTitle: "Dependency Injection"
weight: 1
date: 2017-01-05
description: >
  Learn about DI and why this simple concept is useful.
---




## What Is Dependency Injection?

Dependency Injection is the concept of passing dependencies to objects or other frameworks. 

When a user wants to swap a class or dependency you can pass a different dependency in place of the old dependency.

## How Does Dependency Injection Work?

Here is the main class where it functions. Below is a service where it will authenticate requests.

```C#
using ClassPort.Domain.DTOs.Authentication;
using ClassPort.Domain.Entities.Identity;

namespace ClassPort.Infrastructure.Authentication.Services
{
    public interface IUserService
    {
        Task<AuthenticateResponse?> Authenticate(AuthenticateRequest model);
        Task<ApplicationUser?> GetById(string id);
    }
}
```
This separate class depends on ```namespace ClassPort.Infrastructure.Authentication.Services``` to function and authenticate the app.

```C#
using Microsoft.AspNetCore.Builder;
using Microsoft.Extensions.Configuration;
using Microsoft.Extensions.DependencyInjection;

namespace ClassPort.Infrastructure.Authorization;

public static class Startup
{
	/// <summary>
	///     Add authorization services required for authentication
	/// </summary>
	public static void ConfigureServices(IServiceCollection services, IConfiguration configuration)
	{

	}

	public static void Configure(IApplicationBuilder app, IConfiguration configuration)
	{
		app.UseAuthorization();
	}
}
```

Dependency injection plays its place when you decide to replace the dependency and test it with another dependency. 

Replacing the ```app.UseAuthorization``` with a different method, to test a more optimal way of going about with the code is dependency injection. 

Dependency injection also allows you to prepare all the required classes to function a code. 

With a simple connection to the script you need you can change the function of the public static void Configure method above.

These swappable methods connected to classes use things called services.

## What Are Services?

The swappable classes that dependency injection uses are called services. Services are well-defined classes that serve a specific purpose. Any service registered with dependency injection can usually be resolved in Program.cs and app.Services.

Services also offer service scopes.

```C#
using FluentEmail.MailKitSmtp;
using Microsoft.AspNetCore.Builder;
using Microsoft.Extensions.Configuration;
using Microsoft.Extensions.DependencyInjection;
using ClassPort.Domain.Entities.Settings;
using ClassPort.Infrastructure.Common.Email.Services;
using ClassPort.Infrastructure.Common.Templates.Models;

namespace ClassPort.Infrastructure.Common.Email;

public static void ConfigureServices(IServiceCollection services, IConfiguration configuration)
	{
		var settings = configuration.GetSection("Settings").Get<ApplicationSettings>();

		var provider = new VirtualFileProvider();

		services.AddSingleton<VirtualFileProvider>(provider);
		services.AddFluentEmail(settings.Email.DefaultSenderAddress, settings.Email.DefaultSenderName)
			.AddLiquidRenderer(config =>
			{
				config.FileProvider = provider;
			})
			.AddMailKitSender(new SmtpClientOptions
			{
				Server = settings.Email.Server,
				Port = settings.Email.Port,
				User = settings.Email.User,
				Password = settings.Email.Password,
				UseSsl = settings.Email.UseSsl,
				RequiresAuthentication = settings.Email.RequiresAuthentication,
				PreferredEncoding = settings.Email.PreferredEncoding,
				UsePickupDirectory = settings.Email.UsePickupDirectory,
				MailPickupDirectory = settings.Email.MailPickupDirectory
			});

        services.AddTransient<IEmailSender, EmailSender>();
	}
```
## What Are Service lifetimes?

There are three types of service lifetimes:
1. Scoped
2. Transient
3. Singleton

## Scoped

For web applications, a scoped lifetime indicates that services are created once per client request (connection). Register scoped services with AddScoped.

In apps that process requests, scoped services are disposed at the end of the request.

When using Entity Framework Core, the AddDbContext extension method registers DbContext types with a scoped lifetime by default.

By default, in the development environment, resolving a service from another service with a longer lifetime throws an exception.
## Transient Lifetimes

Transient lifetime services are created each time they are requested from the service container. This lifetime works best for lightweight, stateless services.

In apps that process requests, transient services are disposed of at the end of the request.


## Singleton

Singletons are a type of service that usually are created either the first time they are requested or when providing an implementation instance directly to the container.

Every subsequent request of the service implementation from the dependency injection container uses the same instance. If the app requires singleton behavior, allow the service container to manage the service's lifetime. Do not implement the singleton design pattern and provide code to dispose of the singleton. Services should never be disposed of by code that resolved the service from the container. If a type of factory is registered as a singleton, the container disposes of the singleton automatically.

## How do you make a Service?
[Tutorial](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/create-windows-services-in-c-sharp/Images/image002.png)

1. *In Visual Studios,  first create a project*

2. *Create a folder(Maybe call it Services)*
t
3. *Right-click Services > Create a class*

4. *Start programming your service*

5. *Now you can freely use your service within your code, As long as you reference it*

### Common rules for creating services:

Avoid stateful, static classes, and members. Avoid creating global state by designing apps to use singleton services instead.

A state is a behavorial pattern that is stored.

When multiple methods are required to share state, people tend to use global variables/objects to store such state.

Avoid direct instantiation of dependent classes within services. Direct instantiation couples the code to a particular implementation.

Make services small, well-factored, and easily testable.

## How are services registered?

The ‘Add’ extension methods are used to register all of the services required by a framework feature.

Below it shows the .AddSingleton method. Here it registers the services and configures it to the program.
```C#
using ConsoleDI.IEnumerableExample;
using Microsoft.Extensions.DependencyInjection;
using Microsoft.Extensions.Hosting;

namespace ConsoleDI.Example;

class Program
{
    static Task Main(string[] args)
    {
        using IHost host = CreateHostBuilder(args).Build();

        _ = host.Services.GetService<ExampleService>();

        return host.RunAsync();
    }

    static IHostBuilder CreateHostBuilder(string[] args) =>
        Host.CreateDefaultBuilder(args)
            .ConfigureServices((_, services) =>
                services.AddSingleton<IMessageWriter, ConsoleMessageWriter>()
                        .AddSingleton<IMessageWriter, LoggingMessageWriter>()
                        .AddSingleton<ExampleService>());
}
```






#### Helpful Resources and References
[ServiceScope class](https://docs.microsoft.com/en-us/javascript/api/sp-core-library/servicescope?view=sp-typescript-latest#:~:text=ServiceScope%20provides%20a%20formalized%20way,dependencies%20in%20an%20extensible%20way)
[ASP.NET Core Web Host](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/web-host?view=aspnetcore-6.0#scope-validation)
[Dependency injection in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-6.0)
[Service lifetime details](https://docs.microsoft.com/en-us/dotnet/core/extensions/dependency-injection#service-lifetimes)
[Transient lifetime methods](https://docs.microsoft.com/en-us/dotnet/api/microsoft.extensions.dependencyinjection.servicecollectionserviceextensions.addtransient?view=dotnet-plat-ext-6.0)
