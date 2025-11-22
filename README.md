# 📦 Stock Management System

A comprehensive Java-based inventory management system designed for retail businesses to efficiently manage products, customers, suppliers, and sales operations through an intuitive command-line interface.

## ✨ Features

### 👤 User Roles
- **Manager Access**: Full system control with administrative privileges
- **Customer Access**: Browse products and make purchases

### 🎯 Core Functionalities

#### For Managers
- **Inventory Management**
  - View real-time stock levels
  - Add, update, and remove products
  - Low stock alerts and monitoring
  - Product search functionality

- **Customer Management**
  - Add and remove customer records
  - View customer database
  - Track customer purchase history

- **Supplier Management**
  - Maintain supplier database
  - Add and remove suppliers
  - Track supplier transactions

- **Sales Reporting**
  - Customer sales reports
  - Supplier purchase reports
  - Transaction history tracking

#### For Customers
- Browse available products
- Purchase items with real-time stock updates
- View product details and pricing

### 💾 Data Persistence
- Automatic data saving after each operation
- File-based storage system for:
  - Product inventory (`ProductData.txt`)
  - Customer records (`CustomerData.txt`)
  - Supplier information (`SupplierData.txt`)
  - Sales transactions (`SalesData.txt`)

### 🎨 User Interface
- Color-coded terminal output for better readability
- Clean, menu-driven navigation
- Input validation and error handling

## 🚀 Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Terminal/Command Prompt

### Installation

1. Clone the repository:
```bash
git clone https://github.com/win-x-u-r/StockManager.git
cd StockManager
```

2. Compile the Java files:
```bash
javac *.java
```

3. Run the application:
```bash
java StockManage
```

## 📖 Usage

### Login Options
Upon launching the application, you'll be presented with login options:
```
1. Manager - Access full system features
2. Customer - Browse and purchase products
3. Exit - Close the application
```

### Manager Operations

#### View Stock Levels
- Displays all products with current quantities
- Highlights low-stock items requiring reorder

#### Manage Products
- **Add Product**: Enter product details (ID, name, description, price, quantity)
- **Remove Product**: Delete products by ID or name
- **Update Product**: Modify existing product information
- **Search Product**: Find products by ID or name

#### Manage Customers
- **Add Customer**: Register new customers with ID and name
- **Remove Customer**: Delete customer records
- **View All Customers**: Display complete customer list

#### Manage Suppliers
- **Add Supplier**: Register new suppliers
- **Remove Supplier**: Delete supplier records
- **View All Suppliers**: Display complete supplier list

#### Sales Reports
- **Customer Sales**: View purchase history by customer
- **Supplier Reports**: Track inventory received from suppliers

### Customer Operations

#### Browse Products
View the complete product catalog with:
- Product ID and name
- Description
- Price
- Available quantity

#### Make a Purchase
1. Enter the product name
2. Specify the quantity
3. Provide your customer name
4. Transaction is recorded automatically

## 📁 Project Structure

```
StockManager/
├── StockManage.java      # Main application and menu system
├── Product.java          # Product class and operations
├── Customer.java         # Customer class and purchase logic
├── Supplier.java         # Supplier class and operations
├── Save.java             # Data persistence utilities
├── ProductData.txt       # Product inventory database
├── CustomerData.txt      # Customer records database
├── SupplierData.txt      # Supplier records database
├── SalesData.txt         # Transaction history log
└── README.md             # Project documentation
```

## 🛠️ Technical Details

### Classes Overview

- **StockManage**: Main controller with menu navigation and user interface
- **Product**: Handles product data, inventory operations, and stock management
- **Customer**: Manages customer information and purchase transactions
- **Supplier**: Maintains supplier records and relationships
- **Save**: Provides data persistence and file I/O operations

### Data Format

**ProductData.txt**
```
[ProductID] [Name] [Description] [Price] [Quantity]
```

**CustomerData.txt**
```
[CustomerID] [CustomerName]
```

**SupplierData.txt**
```
[SupplierID] [SupplierName]
```

**SalesData.txt**
```
[CustomerName] [Quantity] [ProductName] [Timestamp]
```

## 🎨 Features in Detail

### Auto-Save Functionality
Data is automatically saved after every transaction, ensuring:
- No data loss on unexpected closure
- Real-time synchronization with storage files
- Consistent state across sessions

### Color-Coded Interface
- 🔴 Red: Headers and important notices
- 🟢 Green: Success messages
- 🟡 Yellow: Warnings
- 🔵 Blue: Information
- 🟣 Purple: Special features
- 🔵 Cyan: Highlights

### Input Validation
- Prevents invalid menu selections
- Validates product quantities and IDs
- Ensures data integrity

## 🤝 Contributing

This is a university final project. Contributions, suggestions, and feedback are welcome!

## 📝 Development Notes

- Auto-save feature implemented after every action
- Login menu system with role-based access control
- Fixed issue with View Suppliers display reset
- File-based persistence for simplicity and portability

## 👥 Authors

Created as a Java Final Project for academic purposes.

## 📄 License

This project is created for educational purposes.

## 🙏 Acknowledgments

- Developed as part of a Java programming course
- Thanks to all team members who contributed to this project

---

**Note**: This application uses text files for data storage. For production use, consider implementing a proper database system.
