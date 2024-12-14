# FinTrack

FinTrack is a personal finance tracking application designed to help users manage and record their financial transactions effectively. Built with .NET MVC, Entity Framework, SQL Server, and Bootstrap, FinTrack offers seamless data management and an intuitive user experience.

## Features

- **Transaction and Category Management**: Record financial transactions and organize them into categories.
- **Data Integrity**: Transactions are linked to categories, ensuring that when a category is deleted, all associated transactions are also removed.
- **Search and Filter**: Search transactions by name and filter them by category or date for better data navigation.
- **Modals for CRUD Operations**: Add, delete, or update transactions and categories directly using modals without navigating to new pages.

## Technologies Used

- **Backend**: .NET MVC
- **Database**: SQL Server (Entity Framework)
- **Frontend**: Bootstrap for responsive design and user interface
- **ORM**: Entity Framework (raw SQL not used)

## Installation

### Prerequisites
- [.NET SDK](https://dotnet.microsoft.com/download)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- A code editor, e.g., [Visual Studio](https://visualstudio.microsoft.com/)

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/FinTrack.git
   ```
2. Navigate to the project directory:
   ```bash
   cd FinTrack
   ```
3. Restore dependencies:
   ```bash
   dotnet restore
   ```
4. Update the `appsettings.json` file with your SQL Server connection string.
5. Apply migrations and update the database:
   ```bash
   dotnet ef database update
   ```
6. Run the application:
   ```bash
   dotnet run
   ```
7. Open your browser and navigate to `https://localhost:5001`.

## Usage

### Transactions
- Add, edit, or delete transactions using the provided modals.
- Search for transactions by name.
- Filter transactions by category or date.

### Categories
- Add, edit, or delete categories directly via modals.
- Deleting a category will automatically delete all associated transactions.

## Project Structure
- `Controllers`: Contains MVC controllers for managing Transactions and Categories.
- `Models`: Entity Framework models for Transactions and Categories.
- `Views`: Razor views for UI components, including Bootstrap modals.
- `Migrations`: Auto-generated migrations for database schema management.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project idea was inspired by the [C# Academy](https://www.thecsharpacademy.com/).

---
