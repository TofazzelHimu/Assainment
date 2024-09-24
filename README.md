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

QUERY:

USE [master] GO
/****** Object: Database [assignmentform] Script Date: 9/17/2024 4:51:00 PM ******/ CREATE DATABASE [assignmentform] CONTAINMENT = NONE ON PRIMARY ( NAME = N'assignmentform', FILENAME = N'E:\softweres\sql\MSSQL16.SQLEXPRESS\MSSQL\DATA\assignmentform.mdf' , SIZE = 8192KB , MAXSIZE = UNLIMITED, FILEGROWTH = 65536KB ) LOG ON ( NAME = N'assignmentform_log', FILENAME = N'E:\softweres\sql\MSSQL16.SQLEXPRESS\MSSQL\DATA\assignmentform_log.ldf' , SIZE = 8192KB , MAXSIZE = 2048GB , FILEGROWTH = 65536KB ) WITH CATALOG_COLLATION = DATABASE_DEFAULT, LEDGER = OFF GO
IF (1 = FULLTEXTSERVICEPROPERTY('IsFullTextInstalled')) begin EXEC [assignmentform].[dbo].[sp_fulltext_database] @action = 'enable' end GO
ALTER DATABASE [assignmentform] SET ANSI_NULL_DEFAULT OFF GO
ALTER DATABASE [assignmentform] SET ANSI_NULLS OFF GO
ALTER DATABASE [assignmentform] SET ANSI_PADDING OFF GO
ALTER DATABASE [assignmentform] SET ANSI_WARNINGS OFF GO
ALTER DATABASE [assignmentform] SET ARITHABORT OFF GO
ALTER DATABASE [assignmentform] SET AUTO_CLOSE OFF GO
ALTER DATABASE [assignmentform] SET AUTO_SHRINK OFF GO
ALTER DATABASE [assignmentform] SET AUTO_UPDATE_STATISTICS ON GO
ALTER DATABASE [assignmentform] SET CURSOR_CLOSE_ON_COMMIT OFF GO
ALTER DATABASE [assignmentform] SET CURSOR_DEFAULT GLOBAL GO
ALTER DATABASE [assignmentform] SET CONCAT_NULL_YIELDS_NULL OFF GO
ALTER DATABASE [assignmentform] SET NUMERIC_ROUNDABORT OFF GO
ALTER DATABASE [assignmentform] SET QUOTED_IDENTIFIER OFF GO
ALTER DATABASE [assignmentform] SET RECURSIVE_TRIGGERS OFF GO
ALTER DATABASE [assignmentform] SET DISABLE_BROKER GO
ALTER DATABASE [assignmentform] SET AUTO_UPDATE_STATISTICS_ASYNC OFF GO
ALTER DATABASE [assignmentform] SET DATE_CORRELATION_OPTIMIZATION OFF GO
ALTER DATABASE [assignmentform] SET TRUSTWORTHY OFF GO
ALTER DATABASE [assignmentform] SET ALLOW_SNAPSHOT_ISOLATION OFF GO
ALTER DATABASE [assignmentform] SET PARAMETERIZATION SIMPLE GO
ALTER DATABASE [assignmentform] SET READ_COMMITTED_SNAPSHOT OFF GO
ALTER DATABASE [assignmentform] SET HONOR_BROKER_PRIORITY OFF GO
ALTER DATABASE [assignmentform] SET RECOVERY SIMPLE GO
ALTER DATABASE [assignmentform] SET MULTI_USER GO
ALTER DATABASE [assignmentform] SET PAGE_VERIFY CHECKSUM
GO
ALTER DATABASE [assignmentform] SET DB_CHAINING OFF GO
ALTER DATABASE [assignmentform] SET FILESTREAM( NON_TRANSACTED_ACCESS = OFF ) GO
ALTER DATABASE [assignmentform] SET TARGET_RECOVERY_TIME = 60 SECONDS GO
ALTER DATABASE [assignmentform] SET DELAYED_DURABILITY = DISABLED GO
ALTER DATABASE [assignmentform] SET ACCELERATED_DATABASE_RECOVERY = OFF
GO
ALTER DATABASE [assignmentform] SET QUERY_STORE = ON GO
ALTER DATABASE [assignmentform] SET QUERY_STORE (OPERATION_MODE = READ_WRITE, CLEANUP_POLICY = (STALE_QUERY_THRESHOLD_DAYS = 30), DATA_FLUSH_INTERVAL_SECONDS = 900, INTERVAL_LENGTH_MINUTES = 60, MAX_STORAGE_SIZE_MB = 1000, QUERY_CAPTURE_MODE = AUTO, SIZE_BASED_CLEANUP_MODE = AUTO, MAX_PLANS_PER_QUERY = 200, WAIT_STATS_CAPTURE_MODE = ON) GO
ALTER DATABASE [assignmentform] SET READ_WRITE GO
