# ASP.NET MVC RichTextEditor - Rename Image

An ASP.NET MVC 5 application demonstrating dynamic image upload and renaming functionality using Syncfusion RichTextEditor component, with automatic filename conflict resolution.

## Features

* **Image Upload Integration**: Seamlessly upload images directly from the RichTextEditor
* **Automatic File Renaming**: Prevents naming conflicts by appending sequential identifiers
* **Custom Response Handling**: Returns modified filenames through HTTP response headers
* **Directory Management**: Automatically creates upload directory if it doesn't exist
* **Error Handling**: Graceful exception handling for upload operations

## Prerequisites

* Visual Studio 2022
* .NET Framework 4.6.1 or higher
* NuGet Package Manager

## How to run the project

1. Checkout this project to a location in your disk
2. Open the solution file (RenameImage.sln) using Visual Studio 2022
3. Restore the NuGet packages by rebuilding the solution
4. Press F5 or click Run to start the application
5. Navigate to the home page and test image upload functionality

## Technical Details

This sample uses Syncfusion EJ2 components with ASP.NET MVC 5. The `HomeController.Rename()` action handles POST requests, accepts file uploads, and implements intelligent filename management. Uploaded files are saved to the `~/Uploads` folder with automatic conflict resolution appending "rteImage[x]-" prefix when duplicates are detected.
