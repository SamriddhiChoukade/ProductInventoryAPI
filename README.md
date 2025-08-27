# 🛒 Product Inventory API (ASP.NET Core Web API + EF Core + SQLite)

This is a simple **RESTful API** built with **ASP.NET Core Web API** and **Entity Framework Core** to manage products in an inventory.


## 🚀 Features
- Add new product (Name, Description, Price, StockQuantity, Category)
- Get all products (with optional filter by category & sort by price)
- Get product by ID
- Update product details (price, stock, etc.)
- Soft Delete / Toggle Active-Inactive (instead of permanent delete)
- Low-stock alert (stock < 5)


## 🛠 Tech Stack
- **Backend Framework:** ASP.NET Core Web API  
- **ORM:** Entity Framework Core  
- **Database:** SQLite (`products.db`)  
- **Language:** C#  


## 📂 Project Structure
ProductInventoryAPI/
├── Controllers/ --> ProductsController.cs (API endpoints)
├── Models/ --> Product.cs (Entity class)
├── Data/ --> AppDbContext.cs (EF Core DbContext)
├── Program.cs --> App startup & middleware
├── appsettings.json --> Database connection string
└── products.db --> SQLite database file (auto-created)



## 🔧 Setup Instructions

### 1️⃣ Clone the Repository
First clone this repo from GitHub:
```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>/ProductInventoryAPI

###Install Dependencies

Restore NuGet packages:

dotnet restore

###database
dotnet ef database update

###Run the API

Start the project:

dotnet run

