# StudentPortal

Version 1.0 — initial commit

## Overview

StudentPortal is a simple Razor Pages / ASP.NET Core (MVC-style controllers) web application demonstrating CRUD operations with Entity Framework Core and a SQL Server database. This repository contains the web project, EF Core migrations, and supporting code for managing students.

## Prerequisites

- .NET 7 SDK
- Visual Studio 2022 (recommended) or VS Code
- SQL Server or LocalDB for development

## Setup

1. Clone the repository:

2. Update the database connection string in `StudentPortal.Web/appsettings.json` or use user secrets. For local development you can use LocalDB:

3. Restore packages and build:

## Database and Migrations

The project uses EF Core migrations. To create or apply migrations locally:

- Add a migration (when you change the model):

Migrations are intended to be committed to source control; the database file itself should not be committed.

## Run the app

Open the solution in Visual Studio and press F5, or run from the command line:

Then open `https://localhost:5001` (or the URL shown in the console) and navigate to the Students pages.



