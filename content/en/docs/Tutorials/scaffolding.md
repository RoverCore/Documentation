
---
title: "Scaffolding a Controller"
linkTitle: "Scaffolding a Controller"
weight: 2
date: 22-02-2022
description: >
  Learn what scaffolding is and why in RoverCore it's better than ever.
---

# CRUD Scaffolding

{{< alert title="Definition" >}}CRUD stands for Create, Read, Update, and Delete{{< /alert >}}

## Scaffolding a CRUD Controller

In order to scaffold a controller, we first have to create the model for which we would like to generate the controller.

### Creating a Model

In order to create a model, right-click on the folder in which you would like to place the model (here, we are placing it in the Entities folder), then hover over *Add*, and click *Class…* A window will pop up; in the field at the very bottom, change the name of the model (we will replace the default value with Widget), and then click *Add*.

![](https://i.imgur.com/vgnZ23V.gif)

This will create an empty model, which we will define as follows:
```csharp
public class Widget
	{
		[Key]
		public int WidgetId { get; set; }
		public string Name { get; set; }
		public string Description { get; set; }
		public bool Available { get; set; }
		public int Count { get; set; }
		public double Price { get; set; }
	}
```

## Scaffold a Controller

Before scaffolding, we have to add *Widget* to our database; we will do this by adding ```public DbSet<Widget> Widget { get; set; }``` in our ApplicationDbContext.cs file (located in the Infrastructure folder under Persistence), so that it looks like this:
```csharp
public DbSet<ConfigurationItem> ConfigurationItem { get; set; }
public DbSet<Member> Member { get; set; }
public DbSet<Template> Template { get; set; }
public DbSet<Widget> Widget { get; set; }
```
In order to scaffold a controller, we right-click on the folder in which we would like to place the controller (in our case the Controllers folder, located in the Presentation folder), hover over Add, and click *Controller*.

![](https://i.imgur.com/leVBPRL.gif)

In the window that appears, we select *MVC Controller with views, using Entity Framework*, and click Add. In the field for *Model class*, we select *Widget*, because that is the model we would like to scaffold the controller for, and in the field for *Data context* class, we select *ApplicationDbContext*, because that is the database we are using. We leave the default values for the other settings, and then type a name for our controller in the Controller field. We name ours *WidgetController*, then we click *Add* to scaffold the controller.

![](https://i.imgur.com/oPqj7WF.gif)

## Modifying a scaffolded CRUD Controller
### Modifying the Model
If you ever need to make changes to your model, you will need to modify its controller, as well as the pages referencing the model. For example, if we decide that we want to add a Color attribute to our Widget, we have to add it to the model:
```csharp
[Key]
public int WidgetId { get; set; }
public string Name { get; set; }
public string Description { get; set; }
public bool Available { get; set; }
public int Count { get; set; }
public double Price { get; set; }
public string Color { get; set; }
```
### Modifying the Pages
Afterwards, in order for everything to work properly, we must modify the pages using that model.
In Create.cshtml (located in the Widget folder, under the Views folder that had been generated for us), we have to add the following to create a field that will set the color of our widget:
```csharp
<div class="form-group">
	<label asp-for="Color" class="control-label"></label>
	<input asp-for="Color" class="form-control" />
	<span asp-validation-for="Color" class="text-danger"></span>
</div>
```
In Edit.cshtml, we add the same code as above to create a field that will allow us to edit the Color attribute of our Widget.
In both Delete.cshtml and Details.cshtml, we add the following so that our page can display the color along with the rest of the Widget’s properties:
```csharp
<dt class="col-sm-2">
	@Html.DisplayNameFor(model => model.Color)
</dt>
<dd class="col-sm-10">
	@Html.DisplayFor(model => model.Color)
</dd>
```
Index.cshtml does not need to be edited because it does not have the object’s properties hardcoded.
### Modifying the Controller
## Using Multiselect Lists
## Using Seeding

{{< alert title="Definition" >}}Data seeding is populating the database with initial data.{{< /alert >}}
We want to add some initial tags that can be selected for our Widget; in order to do that, we will create a class implementing ISeeder and call it WidgetTagSeed. 
{{< alert title="Note" >}}Any class that implements ISeeder will be registered as a service with a scoped lifetime.  The service can use a dependency injection for any needed services.  The only method that needs to be implemented is Task SeedAsync().{{< /alert >}}
### Adding a Dependency Injection
WidgetTagSeed will have to have access to the database, so we add a dependency injection, like this:
```csharp
private readonly ApplicationDbContext _context;

    public WidgetTagSeed(ApplicationDbContext context)
    {
        _context = context;
    }
   ```
   {{< alert title="Note" >}}Remember to add ```using RoverDemo.Infrastructure.Persistence.DbContexts;```{{< /alert >}}
### Creating a Method That Creates Initial Data
Now, we will create the method that will actually add some data to the database.
```csharp
public void CreateWidgetTag()
{
}
```
Now, we will create a *UI* WidgetTag; but first, we need to check if there already exists a tag with the name “UI.” If there is, the function should stop running, because we do not want to create duplicates.
```csharp
if (_context.WidgetTag.Where(x => x.Name == "UI").FirstOrDefault() != null)
{
	return;
}
```
If no WidgetTag with such a name exists, we can safely create it.
```csharp
var tag = new WidgetTag
{
    Id = Guid.NewGuid().ToString(),
    Name = "UI",
    Widgets = new List<Widget>()
};
```
Then, we add the tag to the database and save the changes.
```csharp
_context.Add(tag);
_context.SaveChangesAsync();
```
### Implementing ```Task SeedAsync()```
Now, we will implement ```SeedAsync()``` like this:
```csharp
 public Task SeedAsync()
    {
        CreateWidgetTag();
        return Task.CompletedTask;
    }
```
### References
[Data Seeding - EF Core | Microsoft Docs](https://docs.microsoft.com/en-us/ef/core/modeling/data-seeding)
