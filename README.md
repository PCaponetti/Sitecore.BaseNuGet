# Sitecore.BaseNuGet
A better starting point for NuGet packages for Sitecore

Features include
- UPDATED Sitecore.NuGet.dll with bug that was keeping the script from finding the Sitecore connection file fixed
- automatic versioning based on date
- automatic moving of any compiled binaries to lib on build
- automatic nuget pack on build
- automatic ReadMe open after install-package

Steps to make your first module
1. Change file name of BaseNuGet.sln to desired module name and open
2. Change binary name to desired binary name
3. Add serialized item files to serialization folder
4. Add code to App_Code folder
5. Add GAC references to project so that it will build
6. Add any other nuget packages AND add those packages as references in the .nuspec file
7. Update the .nuspec file with project specific information (license, etc)
8. Build

On the other end you will have a shiny new nupkg file show up next to the .nuspec file.

Remember to install the NuGet package you will need Sitecore Rocks and to have the destination project connected to a Sitecore instance.  To do this just right-click the project in Solution Explorer, find the "Sitecore" menu and select "Connect to Sitecore".

Enjoy!
