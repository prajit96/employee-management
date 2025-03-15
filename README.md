# Employee Management System API

## 📌 Overview
The **Employee Management System API** is a backend service built with **.NET 8** that allows organizations to manage employee data efficiently. It provides CRUD operations, authentication, and follows SOLID principles for maintainability.

## 🚀 Features
- 📝 **CRUD Operations**: Add, update, delete, and retrieve employee data.
- 🔑 **JWT Authentication**: Secure authentication and authorization.
- 🎯 **SOLID Principles**: Well-structured and maintainable codebase.
- 📦 **Entity Framework Core**: Database management with **MySQL**.
- 🛠 **Dependency Injection**: Enhancing modularity and testability.

## 🏗️ Technologies Used
- **.NET 8** (C#)
- **Entity Framework Core**
- **MySQL**
- **JWT Authentication**
- **Swagger (API Documentation)**
- **Visual Studio 2022**
- **Git & GitHub**

## 📂 Project Structure
```
EmployeeManagementAPI/
│-- Controllers/
│   ├── EmployeeController.cs
│   ├── LoginController.cs
│   ├── EmployeeController.cs
│-- Models/
│   ├── Employee.cs
│-- Services/
│   ├── IEmployeeService.cs
│   ├── EmployeeService.cs
│   ├── JwtService.cs
│-- Repositories/
│   ├── EmployeeRepository.cs
│   ├── IEmployeeRepository.cs
│-- Data/
│   ├── AppDbContext.cs
│-- Program.cs
│-- README.md
│-- .gitignore
```

## 🛠️ Setup & Installation
1️⃣ **Clone the Repository**
```sh
git clone https://github.com/prajit96/employee-management.git
cd employee-management
```

2️⃣ **Set Up Database Connection** (Update `appsettings.json`):
```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=EmployeeDataBase;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

3️⃣ **Run Migrations**
```sh
dotnet ef migrations add InitialCreate
dotnet ef database update
```

4️⃣ **Run the API**
```sh
dotnet run
```

## 🔑 Authentication
Use the `/api/auth/login` endpoint to obtain a **JWT Token** for accessing secured routes.

## 📖 API Endpoints
| HTTP Method | Endpoint | Description |
|------------|---------|-------------|
| `GET` | `/api/employees` | Fetch all employees |
| `GET` | `/api/employees/{id}` | Get employee by ID |
| `POST` | `/api/employees` | Add new employee |
| `PUT` | `/api/employees/{id}` | Update employee details |
| `DELETE` | `/api/employees/{id}` | Delete an employee |


## 🤝 Contributing
Pull requests are welcome! If you'd like to contribute, please fork the repository and submit a PR.

## ✨ Author
**[Prajit96](https://github.com/prajit96)** - Developer of this API.

