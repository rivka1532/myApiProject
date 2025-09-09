# My API Project

A comprehensive ASP.NET Core Web API project featuring book management and user authentication with Google OAuth integration.

## 🚀 Features

- **Book Management**: Complete CRUD operations for books
- **User Authentication**: JWT-based authentication system
- **Google OAuth**: Integration with Google authentication
- **Email Services**: MailKit integration for email functionality
- **Logging**: Serilog implementation for comprehensive logging
- **API Documentation**: Swagger/OpenAPI documentation

## 🛠️ Technologies Used

- **Framework**: .NET 8.0
- **Authentication**: JWT Bearer tokens, Google OAuth
- **Email**: MailKit
- **Logging**: Serilog
- **API Documentation**: Swagger/Swashbuckle
- **Language**: C#

## 📁 Project Structure

```
├── Controllers/
│   ├── BookController.cs    # Book management endpoints
│   └── UserController.cs    # User authentication endpoints
├── Models/
│   ├── Book.cs             # Book entity model
│   ├── User.cs             # User entity model
│   └── Role.cs             # User role model
├── Services/               # Business logic services
├── Interfaces/             # Service interfaces
├── Data/                   # Data access layer
└── Properties/             # Application properties
```

## 🚀 Getting Started

### Prerequisites

- .NET 8.0 SDK
- Visual Studio or VS Code
- SQL Server (optional, for database)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/rivka1532/ApiProject.git
   cd ApiProject
   ```

2. Restore dependencies:
   ```bash
   dotnet restore
   ```

3. Update configuration in `appsettings.json`:
   - Configure database connection string
   - Set up Google OAuth credentials
   - Configure email settings

4. Run the application:
   ```bash
   dotnet run
   ```

5. Access the API documentation at: `https://localhost:5001/swagger`

## 📚 API Endpoints

### Books
- `GET /api/books` - Get all books
- `GET /api/books/{id}` - Get book by ID
- `POST /api/books` - Create new book
- `PUT /api/books/{id}` - Update book
- `DELETE /api/books/{id}` - Delete book

### Users
- `POST /api/users/register` - Register new user
- `POST /api/users/login` - User login
- `POST /api/users/google-auth` - Google OAuth login

## ⚙️ Configuration

The application uses the following key configurations:

- **JWT Settings**: Token expiration, secret key
- **Google OAuth**: Client ID and secret
- **Email Settings**: SMTP configuration
- **Database**: Connection strings

## 🤝 Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is for educational and development purposes.
