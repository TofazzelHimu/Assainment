CRUD with DataGridView

A simple Windows Forms application demonstrating how to implement CRUD (Create, Read, Update, Delete) operations with DataGridView. This project is designed to help beginners understand how to use DataGridView for CRUD operations in a desktop application.

Features

Create: Add new records using text boxes and add them to the DataGridView.
Read: Display existing records in the DataGridView.
Update: Modify selected records and update them in the DataGridView.
Delete: Remove selected records from the DataGridView.

Technologies

.NET Framework or .NET Core
C#
Windows Forms (WinForms)
DataGridView

Prerequisites
Before you begin, ensure you have met the following requirements:

Visual Studio installed with .NET Framework or .NET Core (depending on your setup)
Basic knowledge of C# and Windows Forms

Clone the Repository

git clone https://github.com/your-username/crud-with-datagridview.git
cd crud-with-datagridview

Setup Instructions

Open the .sln file in Visual Studio.
Restore NuGet packages if required.
Build the project using Ctrl + Shift + B.
Run the project (F5).

Database Setup 

If you're using a database (e.g., SQL Server, SQLite), make sure to:

Modify the connection string in the code as per your database setup.
Run the necessary SQL scripts to set up the database and table.
sql

CREATE TABLE Items (
    Id INT PRIMARY KEY IDENTITY(1,1),
    Name NVARCHAR(100),
    Quantity INT
);

Usage

Creating a New Record

Enter the name and quantity in the respective text boxes.
Click Add to insert the new record into the DataGridView.

Reading Records

On launching the application, all records will be displayed in the DataGridView.

Updating a Record

Select a row in the DataGridView.
The selected values will appear in the input text boxes.
Modify the data and click Update to save changes.

Deleting a Record

Select a row in the DataGridView.
Click Delete to remove the selected record.

Code Structure

Form1.cs: Contains the logic for CRUD operations and UI event handling.
Program.cs: Entry point for the Windows Forms application.

Key Methods

AddRecord(): Handles the addition of a new record to the DataGridView.
UpdateRecord(): Updates the selected record with modified data.
DeleteRecord(): Deletes the selected record.
LoadData(): Loads all records into the DataGridView when the application starts.


Contributing

Contributions are always welcome! If you'd like to contribute, please fork the repository and make the necessary changes, then submit a pull request.

Steps to Contribute:

Fork the repo.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit and push your changes (git push origin feature-branch).
Open a pull request.

License

This project is licensed under the MIT License.
