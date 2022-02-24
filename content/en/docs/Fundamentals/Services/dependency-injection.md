
---
title: "DI - Dependency Injection"
linkTitle: "Dependency Injection"
weight: 1
date: 2017-01-05
description: >
  Learn about DI and why this simple concept is useful.
---




## What is Dependency Injection?

Dependency Injection is the practice of passing dependencies to objects or other frameworks.

##How does it work?

Here is the main class where it functions

```C#
public class MyDependency
{
    public void WriteMessage(string message)
    {
        Console.WriteLine($"MyDependency.WriteMessage called. Message: {message}");
    }
}
```
This separate class depends on the top class to function

```C#
public class IndexModel : PageModel
{
    private readonly MyDependency _dependency = new MyDependency();

    public void OnGet()
    {
        _dependency.WriteMessage("IndexModel.OnGet");
    }
}
```

Dependency injection plays its place when you decide to replace the method and test it with another class. Replacing the _dependency.WriteMessage with a different method, to test a more optimal way of going about with the code is Dependency Injection. Dependency injection also allows you to prepare all the required methods to function a code. With a simple connection to the script you need you can change the WriteMessage method above.

These swappable methods/classes use things called services.

##What are Services?

The swappable methods that Dependency Injection uses are called Services. Services are well-defined classes that serve a specific purpose. Any service registered with Dependency Injection can usually be resolved in Program.cs and app.Services.

Services also offer service scopes.

```C#
using DependencyInjectionSample.Interfaces;
using DependencyInjectionSample.Services;

var builder = WebApplication.CreateBuilder(args);

builder.Services.AddRazorPages();

builder.Services.AddScoped<IMyDependency, MyDependency>();

var app = builder.Build();
```
##What are Service lifetimes?

There are three types of service lifetimes
1. Scoped
2. Transient
3. Singleton

##Scoped

Service scope is a type of method that allows two different page managers to share the same dependencies.

Usually, this is not possible, but service scopes allow this by creating an overhanging method 
Another unique aspect of service scopes is that it allows for a ServiceKey to provide a default implementation.

For web applications, scoped lifetimes are created once per user request.

You usually register scoped services with AddScoped
###Service Scope Constructors
**Below constructs a new scope for a service scope class.**
protected constructor(parent: ServiceScope | undefined);

[Service Scope Method Details](https://docs.microsoft.com/en-us/javascript/api/sp-core-library/servicescope?view=sp-typescript-latest#:~:text=ServiceScope%20provides%20a%20formalized%20way,dependencies%20in%20an%20extensible%20way.)
[More Method Details Link](https://docs.microsoft.com/en-us/dotnet/api/microsoft.extensions.dependencyinjection.servicecollectionserviceextensions.addscoped?view=dotnet-plat-ext-6.0)

##Transient

Transient lifetime services are created each time they're requested from the service container. This lifetime works best for lightweight, stateless services. Register transient services with AddTransient

In apps that process requests, transient services are disposed of at the end of the request.

[Transient lifetime methods](https://docs.microsoft.com/en-us/dotnet/api/microsoft.extensions.dependencyinjection.servicecollectionserviceextensions.addtransient?view=dotnet-plat-ext-6.0)

##Singleton

These are a type of services that usually are created either the first time they are requested or when providing an implementation instance directly to the container.

Every subsequent request of the service implementation from the dependency injection container uses the same instance. If the app requires singleton behavior, allow the service container to manage the service's lifetime. Don't implement the singleton design pattern and provide code to dispose of the singleton. Services should never be disposed of by code that resolved the service from the container. If a type of factory is registered as a singleton, the container disposes of the singleton automatically.

##How do you make a Service?
![Tutorial](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/create-windows-services-in-c-sharp/Images/image002.png)

*In Visual Studios,  go to File > New > Project and select “Window Service”*

*Right-click screen > Add installer*

*Right-click screen > View code (F7)*

*Type out your code*


*Right-click project in Solution > Rebuild*

*Run code in command prompt:*

*cd C:\Windows\Microsoft.NET\Framework\v4.0.30319*

###Common rules for creating services:

Avoid stateful, static classes and members. Avoid creating global state by designing apps to use singleton services instead.

Avoid direct instantiation of dependent classes within services. Direct instantiation couples the code to a particular implementation.

Make services small, well-factored, and easily testable.

##How are services registered?

The ‘Add’ extension methods are used to register all of the services required by a framework feature.

```C#
using Microsoft.Extensions.DependencyInjection.ConfigSample.Options;

var builder = WebApplication.CreateBuilder(args);

builder.Services
    .AddConfig(builder.Configuration)
    .AddMyDependencyGroup();

builder.Services.AddRazorPages();

var app = builder.Build();
```






####Helpful Resources
[ServiceScope class](https://docs.microsoft.com/en-us/javascript/api/sp-core-library/servicescope?view=sp-typescript-latest#:~:text=ServiceScope%20provides%20a%20formalized%20way,dependencies%20in%20an%20extensible%20way)
[ASP.NET Core Web Host](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/web-host?view=aspnetcore-6.0#scope-validation)
[Dependency injection in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-6.0)
[Introduction to services and dependency injection](https://angular.io/guide/architecture-services)
