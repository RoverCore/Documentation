---
title: "Authentication"
linkTitle: "ASP.NET Identity"
weight: 31
description: >
  Lead in description for Identity
---
## What is identity?
Identity is a core feature available on ASP.NET which provides a lot of functionality to websites and is a basis for overall web development. The heart of identity is it that gives web pages the ability for users to create and save accounts. Essentially this is a built in membership system. Data related to user accounts such as usernames, emails, passwords, names and dates can be saved into a SQL server database or other forms such as an Azure Table Storage. Some of identities features include the ability to: 
- Create, read, update and delete user accounts
- Confirm a users account
- Authenticate and Authorize a users account
- Recover or reset an accounts password
- Enable two factor authentication with SMS or mobile application (ex. Steam Guard)
- Allow a web application to use external already established identities/accounts such as Microsoft, Facebook, Google, GitHub etc. 


## Identity
In order to apply identity to a web application, one's project must contain the `Microsoft.AspNetCore.Identity.EntityFrameworkCore` package. This will allow for identity data and schema (outline/diagram/model/datatype) to access the SQL Server via the Entity Framework Core. You will be able to find the identity services added to the project in the ConfigureServices method of the Startup class. Thanks to dependency injection these services will be usable throughout the entire application. In order to use Identity in the application, UseIdentity must be called in the Configure method of Startup class. 	

The `IdentityDbContext` class is the base class for the Entity Framework database context used for identity. This class has the constructors ```C#IdentityDbContext()``` which initializes a new instance of the class as well as the `IdentityDbContext(DbContextOptions)` which initializes a new instance of IdentityDbContext. The properties included in this class include:
- RoleClaims- This will get or set the DbSet<TEntity> of role claims. 
- Roles- This will get or set the DbSet<TEntity> of roles.
- UserClaims- This will get or set the DbSet<TEntity> of User claims. 
- UserLogins- This will get or set the DbSet<TEntity> of User logins. 
- UserRoles- This will get or set the DbSet<TEntity> of User roles.
- Users- This will get or set the DbSet<TEntity> of Users. 
- UserTokens- This will get or set the DbSet<TEntity> of User tokens. 
- The only method in this class is OnModelCreating(ModelBuilder) which configures the schema needed for the identity framework. 

## Where is Identity in RoverCore?
RoverCore uses ASP.NET 6’s identity. Some notable updates include simplified development, better performance, and productivity from the hot reload function. Using dependency injection, identity is useful in RoverCore due to the UserManager and SignInManager services. Both of those services are used in any controller if necessary. For Example
```C#
  private readonly UserManager<ApplicationUser> _userManager;
    private readonly SignInManager<ApplicationUser> _signInManager;

    public AccountController(UserManager<ApplicationUser> userManager, SignInManager<ApplicationUser> signInManager)
    {
        _userManager = userManager;
        _signInManager = signInManager;
    }
  ```



**Customization of ApplicationUser/ApplicationRole**
An application role is an entity that enables an application to run with its own permissions. You are able to customize the application role to enable access to specific data to only those users who go through the application in a specific way. Because application roles are entities, they can access other databases only through databases linked to a basic level or guest account.
An application user is a built-in user account that is used to perform integration and system back-end service to support a particular feature. Customization is limited by an application user due them being built-in and unable to be updated.
**What is a  userManager?**
A class that can handle a user’s role and account on a website is called UserManager.The background of UserManager is that it’s a class that controls the user by means of creating, deleting and updating the users. There are various methods of UserManager you can use that can find a user via username, email, and the User’s ID. The functionality of UserManager includes adding/removing roles ie: Admin account versus a student account. Lastly also includes generation of password hashes, validation of users and more additional privacy. 
Examples:
```C#
  Public class YourController : BasedController<YourController>
{
private readonly UserManager<ApplicationUser> _userManager;

public YourController(UserManager<ApplicationUser> userManager)
{
       _userManager = userManager;
       _userManager = signInManage;
}
  ```



**What is a signInManager?**
A service that is available through dependency injection is known as SignInManager. It’s a class that handles the user to sign in from the application. The service authenticates the user which is simply logging the user in and out. Cookies are also dished out from SignInManager. Cookies are small blocks of  data used to help users access a website. Authentication cookies help the website identify what account the user is on. Here are some examples.

```C#
  Public class YourController : BasedController<YourController>
{
private readonly SignInManager<ApplicationUser> _signInManager;

public YourController(UserManager<ApplicationUser> userManager)
{
_userManager = userManager;
_userManager = signInManage;
}
  ```



### Common Questions when Using Identity


#### How can I get the currently logged in user?

```C#
  var user = await _userManager.GetUser(User);
  ```


#### How do I add a new user to a role?

```C#
  // Add user to Admin role
var user = await _userManager.GetUser(User);
await _userManager.AddToRoleAsync(user, "Admin");
  ```


#### How do I create a user?
Make sure you created a model class inside your models folders. A simple method that stores a new user in the database using a specified password :
```C#
  var user = new ApplicationUser { Id = Guid.NewGuid().ToString(), UserName = "bill", Email = "bill@microsoft.com" };
var result = await _userManager.CreateAsync(user, "password");
if (result.Succeeded)
{
_logger.LogInformation("User created a new account with password.");
}
```


####**How do I change a user's password?**
```C#
Public class ChangePasswordViewModel
{
Public string CurrentPassword {get; set;}

Public string NewPassword {get; set;}
}
```


####**How can I get a user by their username?**
```C#
string getUser = System.Security.Principal.WindowsIdentity.GetCurrent().Name.ToString();
```




## References
* [Add Issue #7 Identity Documentation #12](https://github.com/RoverCore/Documentation/issues/7)
* [RoverCore](https://github.com/RoverCore/RoverCore)
* [Introduction to Identity](https://jakeydocs.readthedocs.io/en/latest/security/authentication/identity.html#:~:text=ASP.NET%20Core%20Identity%20is,Microsoft%20Account%2C%20Twitter%20and%20more.)
* [Application Roles](https://docs.microsoft.com/en-us/sql/relational-databases/security/authentication-access/application-roles?view=sql-server-ver15#:~:text=An%20application%20role%20is%20a,connect%20through%20a%20particular%20application.)
* [Identity model customization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/customize-identity-model?view=aspnetcore-6.0)
* [ASP.NET Core Identity Tutorial](https://www.tektutorialshub.com/asp-net-core/asp-net-core-identity-tutorial/)
* [ASP NET Core Identity tutorial from scratch](https://www.youtube.com/watch?v=egITMrwMOPU)
* [IdentityDbContext Class](https://docs.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.identity.entityframeworkcore.identitydbcontext?view=aspnetcore-6.0)
* [Get Current Logged In UserId of User in ASP.NET CORE Identity](https://youtu.be/OP_KDWlAgCQ)
* [Manage user roles in asp net core identity](https://youtu.be/1OaVUy1pRXA)
* [Register new user using asp net core identity](https://youtu.be/sPbDrqpme_w)
* [Change password in asp net core  ](https://youtu.be/r7VzoLhFLd0)
* [Implementing login functionality in asp net core](https://youtu.be/9d8DXXc71RI)
* It was revealed to me in a dream

