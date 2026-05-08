# StudentPortal

Version 1.0 — initial commit

## Overview

StudentPortal is a simple Razor Pages / ASP.NET Core (MVC-style controllers) web application demonstrating CRUD operations with Entity Framework Core and a SQL Server database. This repository contains the web project, EF Core migrations, and supporting code for managing students.

## Prerequisites

- .NET 7 SDK
- Visual Studio 2022 (recommended) or VS Code
- SQL Server or LocalDB for development
- (Optional) Git and GitHub account

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

## Tests

(Currently no automated tests are included. Add unit/integration tests under a `tests/` folder as needed.)

## Contributing

- Create a branch for your changes: `git checkout -b feat/your-feature`
- Add clear commit messages and push the branch to your fork or origin.
- Open a pull request describing the change.

## Security / Secrets

Do not commit production secrets or connection strings. Use user secrets in development or environment variables in CI. The repository includes a `.gitignore` to exclude IDE files and local secrets.

## License

This project does not include a license file. Add a `LICENSE` if you want to open source the code.

---

If you want a one-click GitHub Actions workflow, a CI build script, or a `CONTRIBUTING.md` template, tell me which and I will generate it.
