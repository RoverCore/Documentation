---
title: "MVC - Model View Controller"
linkTitle: "Model View Controller"
weight: 10
description: >
  The model-view-controller (MVC) pattern divides an application into three components: A model, a view, and a controller.
---

## What is a Model View Controller?

The Model-View-Controller (MVC) pattern consists of three separate branches. The model branch is what defines the overall structure of data and manages it. The view branch contains files that return representations of the data that the user can see and effectively read. Controllers work with user inputs to perform actions on models or return views. This pattern is very well known and has many standard conventions to go along with it.

## Benefits of MVC

MVC has many well documented benefits. Its strongly defined structures allow for good organization when dealing with large projects. The MVC's structure also allows for asynchronous method invocation, meaning methods can be called and the rest of the program is able to be run while waiting for the called method to finish. This allows for faster loading applications. These methods can be run by using the keyword "await" to call a method that has been defined with the "async" property.

Because the MVC format is separated into multiple sections, people can work on different components of the code simultaneously without causing issues. This separation can also make debugging simpler.

## Routing

Routing in a MVC usually follows a specific convention, but it can be done nearly any way by altering the startup code. When making a project with a MVC using ASP.NET Core 6, the default routing is the following:

```csharp
app.MapControllerRoute(
    name: "default",
    pattern: "{controller=Home}/{action=Index}/{id?}");

```

This code specifies the pattern of routing on startup. The name field allows you to define what route should be followed for different situations. The pattern field describes what comes after the default domain name in the link of a web application, and tells the program exactly what to do when given the information. The code shown also provides default values for the pattern. When using multiple routes, routing will often be defined as follows:

```csharp
app.UseEndpoints(endpoints =>
{
    endpoints.MapRazorPages();

    endpoints.MapControllerRoute(
        name: "default",
        pattern: "{controller=Home}/{action=Index}/{id?}"
    );
});

```

This code also shows how endpoints can be used to determine what routing should be used.

## Areas

Areas are an organizational structure in MVC that allows programs to have much more effective routing and a set hierarchy to operate with. Areas contain their own controllers, models, and views. This effectively makes area its own structure; thus, their content corresponds to a specific function or purpose in a program. For example, a program designed for a car dealership may have areas like "Rent," "Purchase," and "Sell," in order to reasonably separate the code. Areas are important in large programs in order to separate code in functional categories that may differ from simply their form (instead of grouping all controllers or all models, group their functions together).
	
In terms of routing, areas can simplify the routes necessary for certain pages and also group similar pages together. For example, examine the following code:

```csharp
app.UseEndpoints(endpoints =>
{
    endpoints.MapControllerRoute(
        name: "Areas",
        pattern: "{area:exists}/{controller=Home}/{action=Index}/{id?}");

    endpoints.MapControllerRoute(
        name: "default",
        pattern: "{controller=Home}/{action=Index}/{id?}");
});
```

Now, all "Purchase" or "Sell" pages can be accessed directly from referencing their area in the URL. Without this routing, these pages could exist in all different routes based on controllers they interact with.

## Action Methods

Action methods are defined in controllers to associate user actions with a program output. Actions are associated with an "ActionResult," which includes any of the following:

* ViewResult
* EmptyResult
* ContentResult
* FileContentResult
* FilePathResult
* FileStreamResult
* JavaScriptResult
* JsonResult
* RedirectResult
* RedirectToRouteResult
* PartialViewResult
* HttpUnauthorizedResult

Action methods can also include parameters of any type if necessary. Here is an example of defining an action method.

```csharp
public ActionResult Index()
{
    return View(); 
}
```

Now, when `/Index` is referenced in the URL, the program will return the corresponding view.

## Request Types

Request Types identify the different possible actions that are invoked upon a program, often in order to retrieve and/or send data. Requests that aren't `GET` are defined by writing HTTP followed by the request type (as seen below) before an action method:

```csharp
public class StudentController : Controller 

[HttpPost] 

public ActionResult PostAction() // handles POST requests by default
{ 
    return View("Index"); 
}
```

Examples of Request Types include:
* HttpGet: Retrieve information identified by a request
* HttpPost: Annotate, post messages, submitting a form, etc.
* HttpPut: Send data to be stored
* HttpDelete: Deletes resource

## References

[CodeAcademy](https://www.codecademy.com/article/mvc)

[TutorialsTeacher Routing in MVC](https://www.tutorialsteacher.com/mvc/routing-in-mvc)

[GeeksforGeeks](https://www.geeksforgeeks.org/benefit-of-using-mvc/)

[Microsoft](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/areas?view=aspnetcore-6.0)

[TutorialsTeacher Action Methods](https://www.tutorialsteacher.com/mvc/action-method-in-mvc)

[TutorialsTeacher Action Verbs](https://www.tutorialsteacher.com/mvc/actionverbs-in-mvc#:~:text=The%20MVC%20framework%20includes%20HttpGet,handle%20HttpGet%20request%20by%20default)

