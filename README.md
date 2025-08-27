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

<img width="1872" height="842" alt="Screenshot 2025-08-27 155749" src="https://github.com/user-attachments/assets/d1d41259-589b-422c-bf6f-dc26c7b8fcb5" />

<img width="1832" height="854" alt="Screenshot 2025-08-27 155818" src="https://github.com/user-attachments/assets/4be8105c-fbbf-4935-997a-e5213201a6fe" />

<img width="1868" height="847" alt="Screenshot 2025-08-27 155846" src="https://github.com/user-attachments/assets/909fd74c-da6f-4819-8cf0-d52edb3656cb" />

<img width="1837" height="732" alt="image" src="https://github.com/user-attachments/assets/4af09a57-9612-41b3-b434-086e6398779b" />




