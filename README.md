# 💵 Expense Tracker

## Overview

Expense Tracker is a web application designed to help users manage their personal finances by tracking income and expenses. This project utilizes ASP.NET Core MVC framework and follows best practices for maintainability and scalability.

## Features

- **User Authentication:** Secure user login and registration.
- **Income & Expense Tracking**: Add, edit, delete, and view income and expense transactions.
- **Categorization**: Categorize transactions for better organization.
- **Dashboard**: Visual representation of income and expense data.
- **Reports**: Generate financial reports based on user data.

<br>

<div align="center">
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/121405754-b4f48f80-c95d-11eb-8893-fc325bde617f.png" alt=".NET Core" title=".NET Core"/></code>
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/121405384-444d7300-c95d-11eb-959f-913020d3bf90.png" alt="C#" title="C#"/></code>
	<code><img width="50" src="https://github.com/marwin1991/profile-technology-icons/assets/19180175/3b371807-db7c-45b4-8720-c0cfc901680a" alt="MSSQL" title="Microsoft SQL Server"/></code>
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/117447155-6a868a00-af3d-11eb-9cfe-245df15c9f3f.png" alt="JavaScript" title="JavaScript"/></code>
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/192158954-f88b5814-d510-4564-b285-dff7d6400dad.png" alt="HTML" title="HTML"/></code>
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/183898674-75a4a1b1-f960-4ea9-abcb-637170a00a75.png" alt="CSS" title="CSS"/></code>
	<code><img width="50" src="https://user-images.githubusercontent.com/25181517/183898054-b3d693d4-dafb-4808-a509-bab54cf5de34.png" alt="Bootstrap" title="Bootstrap"/></code>
</div>

<br>

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
  ```bash
  git clone https://github.com/KaziNizamul/Expense-Tracker.git
  ```

2. Navigate to the project directory:
  ```bash
  cd Expense-Tracker
  ```

3. Install the necessary packages:
  ```bash
  dotnet restore
  ```

4. Update the database connection string in appsettings.json:
  ```json
  "ConnectionStrings": {
    "DevConnection": "Server=db5479.databaseasp.net; Database=db5479; User Id=db5479; Password=2k@MC7a=-xG6; Encrypt=False; MultipleActiveResultSets=True;"
  }
  ```
5. Apply the migrations to create the database:
  ```bash
  dotnet ef database update
  ```

6. Run the application:
  ```bash
  dotnet run
  ```

<br>

## Project Structure

The project is structured as follows:

- Controllers: Contains the controllers that handle HTTP requests and responses.
  - HomeController.cs: Manages the homepage and general views.
  - AccountController.cs: Handles user authentication.
  - TransactionController.cs: Manages CRUD operations for transactions.

- Models: Contains the data models used in the application.
  - ApplicationUser.cs: Represents a user in the application.
  - Transaction.cs: Represents a financial transaction.

- Views: Contains the Razor views for rendering the user interface.
  - Home: Views related to the homepage.
  - Account: Views for user authentication.
  - Transaction: Views for managing transactions.

- Data: Contains the database context and migrations.
  - ApplicationDbContext.cs: The database context for Entity Framework Core.
  - Migrations: Contains the database migrations.

- wwwroot: Contains static files such as CSS, JavaScript, and images.
