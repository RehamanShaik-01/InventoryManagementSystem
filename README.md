

## 🛒 Inventory Management System — Java + MySQL

This is a **console-based Inventory Management System** built using **Java** and **MySQL**. It allows users to manage products, perform CRUD operations, and track inventory efficiently with database integration using JDBC.



### 📌 Features (10 Total)

1. ➕ Add New Product
2. 📄 View All Products
3. ❌ Delete Product
4. 🔍 Search Product by Name
5. 🚪 Exit



### 🛠 Technologies Used

* 💻 Java (JDK 17 or above recommended)
* 🐬 MySQL (MySQL 8.0+)
* 🔗 JDBC (MySQL Connector/J)



### ⚙️ Database Setup

1. **Create the database and table:**

```sql
CREATE DATABASE IF NOT EXISTS inventory_db;

USE inventory_db;

CREATE TABLE IF NOT EXISTS products (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    quantity INT NOT NULL,
    price DOUBLE NOT NULL,
    category VARCHAR(100) NOT NULL
);
```


### 📦 How to Run the Project

#### 1. Clone the Repository

```bash
git clone https://github.com/your-username/InventoryManagementSystem.git
cd InventoryManagementSystem
```

#### 2. Add MySQL Connector

Download the [MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/) and place the JAR file in your project directory.

#### 3. Compile and Run

```bash
javac -cp .;mysql-connector-java-8.3.0.jar InventoryManagementSystem.java
java -cp .;mysql-connector-java-8.3.0.jar InventoryManagementSystem
```


### ⚠️ Troubleshooting

* **SQLException: No suitable driver found**
  Ensure `mysql-connector-java-x.x.x.jar` is correctly included in the classpath.

* **Table already exists warning**
  Ignore if you’re running the setup multiple times.



### 📁 Project Structure

```
InventoryManagementSystem/
│
├── InventoryManagementSystemMySQL.java   # Main Java source code
├── mysql-connector-java-8.3.0.jar        # JDBC connector (you must download manually)
├── README.md                             # Project readme


### 🙋 Author

* Name: Shaik.Rehaman



