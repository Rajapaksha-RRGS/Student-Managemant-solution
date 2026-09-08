# Student Managemant Solution

Windows Forms application for managing students, classes, attendance, user registration, and attendance reports.

## Tech Stack
- .NET 9.0 (`net9.0-windows`)
- Windows Forms
- MySQL (via `MySql.Data`)
- PDF report export (via `DinkToPdf`)

## Project Structure
- `Student Managemant solution.sln` - Visual Studio solution
- `Student Managemant/` - Main WinForms project
- `photos/user_table.sql` - Sample SQL dump for `user_table`

## Features
- Login and forgot password flow
- Role-aware main dashboard (Admin / Student views)
- Class management
- Student management and registration
- Attendance management
- Class and student attendance reporting with PDF export

## Prerequisites
- Windows OS
- Visual Studio 2022 (or newer) with .NET desktop workload
- .NET 9 SDK
- MySQL server (or XAMPP MySQL)

## Database Setup
1. Create a MySQL database named `attendens_managment_system`.
2. Import SQL files for your tables (sample `user_table` dump is available at `photos/user_table.sql`).
3. Confirm connection settings match the app connection strings used in code:
   - Server: `localhost`
   - Database: `attendens_managment_system`
   - User: `root`
   - Password: empty

## Run the Application
1. Open `Student Managemant solution.sln` in Visual Studio.
2. Restore NuGet packages.
3. Build and run the `Student Managemant` project.
4. Login using records from your `user_table` data.

## Notes
- The app currently uses hard-coded MySQL connection strings in forms/user controls.
- Ensure all required database tables exist before running attendance and report features.
