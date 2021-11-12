# Template metadata
Please find all the metadata for the template in the `.template.config` folder, in the `template.json` file.
> The json file `sourceName` property should match the root namespace to make `--output [folder]` switch to work properly with name substitution.

> The boilerplate is based on the webapi template.

# Install the template
From directory `working` run `dotnet new --install ./`. 

All files in the subfolder are added into the template, when creating a csproj (see 'Use the template' section below):  

```
> dotnet new --install ./
The following template packages will be installed:
   D:\Develop\Lab\dotnet-template-boilerplate\working

Success: D:\Develop\Lab\dotnet-template-boilerplate\working installed the following templates:
Template Name          Short Name  Language  Tags
---------------------  ----------  --------  ----------
Custom ASP.NET WebAPI  mywebapi    [C#]      Web/WebAPI
```

# Uninstall the template
To list the installed templates:

```
> dotnet new --uninstall --list
D:\Develop\Lab\dotnet-template-boilerplate\working
    Templates:
       Custom ASP.NET WebAPI (mywebapi) C#
    Uninstall Command:
       dotnet new --uninstall D:\Develop\Lab\dotnet-template-boilerplate\working
```
Run the uninstall command to uninstall.

# List all templates
To list the installed templates on your computer, run `dotnet new --list`. The `mywebapi` template is this boilerplate:

```
> dotnet new --list
Template Name                                 Short Name           Language    Tags
--------------------------------------------  -------------------  ----------  -------------------------------------
.
.
.
Console App                                   console              [C#],F#,VB  Common/Console
Custom ASP.NET WebAPI                         mywebapi             [C#]        Web/WebAPI
dotnet gitignore file                         gitignore                        Config
.
.
.
```

# Use the template
Run `dotnet new mywebapi --output [folder/csproj name]`. Create and start the newly created csproj by:
```
> dotnet new mywebapi --output VeryNiceWebApi
The template "Custom ASP.NET WebAPI" was created successfully.

> cd VeryNiceWebApi
> dotnet run
Building...
info: Microsoft.Hosting.Lifetime[14]
      Now listening on: https://localhost:7243
info: Microsoft.Hosting.Lifetime[14]
      Now listening on: http://localhost:5239
info: Microsoft.Hosting.Lifetime[0]
      Application started. Press Ctrl+C to shut down.
info: Microsoft.Hosting.Lifetime[0]
      Hosting environment: Development
info: Microsoft.Hosting.Lifetime[0]
      Content root path: D:\Develop\Lab\dotnet-template-boilerplate\test\VeryNiceWebApi\
info: Microsoft.Hosting.Lifetime[0]
```
