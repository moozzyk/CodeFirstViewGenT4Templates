EF-CodeFirst-View-Generation-T4-Templates
=========================================

T4 templates for creating pre-generated views for applications using Entity Framework Code First

Note: Project relies on 7z.exe being in the %PATH%

Structure:
+
|
+--CodeFirstViewGenT4TemplateCSharp
|
+--CodeFirstViewGenT4TemplateVBNet

CodeFirstViewGenT4TemplateCSharp contains template for T4 templates for creating pre-generated views for C# apps
CodeFirstViewGenT4TemplateVBNet contains template for T4 templates for creating pre-generated views for VB.NET apps

Building:
Open the CodeFirstViewGenT4Templates.sln in Visual Studio and build. 

Installation:
Double click/enter on vsix files built in the previous step

Usage:
Create a new project. Install EntityFramework.dll from nuget (e.g. by running "Install-Package EntityFramework" from Package Manager Console). Create your entities and the class derived from DbContext. "Add New Item" to the project and go to "Code" category. Select "ËF Code First Pre-generated Views for C#/VB". Use the convention '{MyContext}.Views.tt'where {MyCOntext} is the name of the class derived from DbContext you would like to generate views for. Wait until views are generated (note that for bigger or more complicated (deep inheritance hierarchy) models it may take some time). 

Links:

Vsix files on Visual Studio Gallery:
Version for C#: http://visualstudiogallery.msdn.microsoft.com/ae7730ce-ddab-470f-8456-1b313cd2c44d
Version for VB.NET: http://visualstudiogallery.msdn.microsoft.com/118b44f2-1b91-4de2-a584-7a680418941d

Posts about these templates on my blog: 
http://blog.3d-logic.com/2012/05/28/entity-framework-code-first-and-pre-generated-views/
http://blog.3d-logic.com/2012/06/13/entity-framework-codefirst-view-generation-templates-on-visual-studio-code-gallery/

