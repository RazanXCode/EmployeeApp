# EmployeeApp

EmployeeApp is an ASP.NET Core MVC application for managing employees, including CRUD (Create, Read, Update, Delete) operations.

## Prerequisites
Ensure you have the following installed:
- .NET SDK (Latest version)
- SQL Server or LocalDB
- Visual Studio

## Setup Instructions

### 1. Clone the Repository
```sh
 git clone <repository-url>
 cd EmployeeApp
```

### 2. Restore Dependencies
```sh
dotnet restore
```

### 3. Configure the Database
Update the connection string in **`appsettings.json`**:
```json
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\MSSQLLocalDB;Database=EmployeeDB;Trusted_Connection=True;MultipleActiveResultSets=true"
}
```

### 4. Apply Migrations and Seed Database
```sh
dotnet ef migrations add InitialCreate
dotnet ef database update
```

### 5. Run the Application
```sh
dotnet run
```
The app will be available at: [https://localhost:5001](https://localhost:5001) (or another port specified in the output).

## Features
- Add, Edit, Delete, and View employees.
- Uses Entity Framework Core for database management.


## Contributing
Feel free to submit issues or pull requests to improve the application.

