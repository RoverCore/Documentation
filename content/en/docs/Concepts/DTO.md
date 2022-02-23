---
title: "DTO - Data Transfer Objects"
linkTitle: "DTOs (Data Transfer Objects)"
weight: 35
description: >
  Learn about Data Transfer Objects (Also known as ViewModels in Asp.NET MVC).
---

## What are DTOs?

A data transfer object is a class that’s used for public display of another object in the app. A DTO makes a class more secure by hiding sensitive data.

## Benefits of using DTOs over raw entities?

A layer of DTOs isolates the domain model from the presentation, resulting in both loose coupling and optimized data transfer. In loose coupling, you can change one service without changing the other by reducing interdependencies. If DTOs are used, a change in the requirements that forces a move to a different amount of data doesn't have any impact on the service layer or even the domain.

## What is overposting?

Overposting is a type of cyber attack that targets websites. More specifically, overposting targets controllers that expect an input from a user, but have other variables that are intentionally hidden from the user. For example, if a model has an “IsAdmin” variable that limits what a user can and cannot do, a hacker who knows this information can manually add an extra field to an input that would allow them to change the “IsAdmin” variable.

## How is overposting prevented?

Take a look at an example set of code by [Scott Hanselmen](https://www.hanselman.com/blog/aspnet-overpostingmass-assignment-model-binding-security):

```csharp
public class Person
{
    public int ID { get; set; }
    public string First { get; set; }
    public string Last { get; set; }
    public bool IsAdmin { get; set; }
}
```

```csharp
[HttpPost]
[ValidateAntiForgeryToken]
public async Task<IActionResult> Create(Person person)
{
```

```csharp
 if (ModelState.IsValid)
    {
        _context.Add(person);
        await _context.SaveChangesAsync();
        return RedirectToAction("Index");
    }
    return View(person);
}
```

Here we see an entity and a corresponding action that accepts the entity as a parameter. Let's say that the controller only wants the “First” and “Last” variables to be gathered from an input. A hacker can very easily add another field to an input that allows them to edit either the “ID” or the “IsAdmin” field. Now, look at the same code again but this time it is using binding.

```csharp
[HttpPost]
[ValidateAntiForgeryToken]
public async Task<IActionResult> Create([Bind("First,Last")] Person person)
{
    if (ModelState.IsValid)
    {
        _context.Add(person);
        await _context.SaveChangesAsync();
        return RedirectToAction("Index");
    }
    return View(person);
}
```

Now the action has bound the desired variables to "person". This means that the action will only accept inputs that create either the “First” or “Last” variables and will not take any inputs from anything else. This makes the other variables such as “IsAdmin” completely inaccessible to hackers.

## Notes from Microsoft

Microsoft recognizes DTOs as being superior to binding in terms of security. Take note of these resources for more information on DTO’s and their security in terms of overposting: [Create Data Transfer Objects](https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5), [Microsoft Security note about Overposting](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/crud?view=aspnetcore-6.0#security-note-about-overposting).

## Examples

Below is an example on a Class and a corresponding DTO that limits what parts of the class are visible. For an example, of regular binding see the “**How is overposting prevented?**” section of this document.

```csharp
public class User {
 
    private String id;
    private String name;
    private String password;
    private List<Role> roles;
 
    public User(String name, String password, List<Role> roles) {
        this.name = Objects.requireNonNull(name);
        this.password = this.encrypt(password);
        this.roles = Objects.requireNonNull(roles);
    }
 
    // Getters and Setters
 
   String encrypt(String password) {
       // encryption logic
   }
}
```

```csharp
public class UserDTO {
    private String name;
    private List<String> roles;
    
    // standard getters and setters
}
```

## References
[Cutting Edge - Pros and Cons of Data Transfer Objects](https://docs.microsoft.com/en-us/archive/msdn-magazine/2009/august/pros-and-cons-of-data-transfer-objects)

[Create Data Transfer Objects (DTOs)](https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5)

[Preventing mass assignment or over posting in ASP.NET Core](https://andrewlock.net/preventing-mass-assignment-or-over-posting-in-asp-net-core/#:~:text=Mass%20assignment%2C%20also%20known%20as,not%20expect%20to%20be%20set.)

[The DTO Pattern](https://www.baeldung.com/java-dto-pattern)

[ASP.NET - Overposting/Mass Assignment Model Binding Security](https://www.hanselman.com/blog/aspnet-overpostingmass-assignment-model-binding-security)
