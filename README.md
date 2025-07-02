# Pharmacy Management System

The **Pharmacy Management System** is a simple and efficient desktop-based solution for managing medicine inventory and automating key pharmacy tasks. It includes a Python script for interacting with a MySQL database and comes with a sample database file pre-filled with data for testing and setup.

---

## 🚀 Features

- View a complete list of medicines in the inventory  
- Add new medicines to the system  
- Update existing medicine details and quantity  
- Delete medicines from the database

---

## 🛠️ Prerequisites

Make sure the following software is installed on your system:

- **Python 3** → [Download Python](https://www.python.org/downloads/)  
- **MySQL Server** → [Download MySQL](https://dev.mysql.com/downloads/)  
- **phpMyAdmin (optional)** → [Download phpMyAdmin](https://www.phpmyadmin.net/downloads/)

---

## ⚙️ Installation

1. **Clone the repository** or download it as a ZIP:
   ```bash
   git clone https://github.com/your-username/pharmacy-management-system.git
   ```

2. **Set up the database**:
   - Start your MySQL server.
   - Create a new database (e.g., `pharmacy`).
   - Import the sample SQL file:
     - Using **phpMyAdmin**: Upload `database.txt` from the UI.
     - Using **command line**:
       ```bash
       mysql -u <username> -p <database_name> < database.txt
       ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

---

## 💻 Usage

1. Ensure your MySQL server is running.
2. Open your terminal or command prompt and navigate to the project directory.
3. Run the script:
   ```bash
   python project.py
   ```
4. Use the system to manage medicine records as needed.

---

## 🗃️ Database Structure

The sample database (`database.txt`) includes a table named `medicines_info` with the following columns:

| Column     | Type     | Description                             |
|------------|----------|-----------------------------------------|
| Med_code   | INT      | Unique ID for each medicine             |
| Med_name   | VARCHAR  | Name of the medicine (max 30 chars)     |
| Qty        | INT      | Quantity in stock                       |
| MRP        | DOUBLE   | Maximum retail price                    |
| Mfg        | DATE     | Manufacturing date                      |
| Exp        | DATE     | Expiry date                             |
| Purpose    | VARCHAR  | Intended use (max 30 chars)             |

---

## 🧱 Getting Started

1. Install MySQL server and (optionally) phpMyAdmin.
2. Create a new database (e.g., `pharmacy`).
3. Import the provided `pharmacy.sql` or `database.txt` file.
4. The `medicines_info` table and sample records will be ready to use.
