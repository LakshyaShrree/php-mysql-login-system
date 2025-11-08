# 🔐 PHP MySQL Login System

A simple and secure **Login & Registration System** built using **PHP** and **MySQL**.  
It demonstrates how to connect a PHP webpage with a MySQL database to enable **user registration, login validation, session handling, and error management**.

---

## 🚀 Features

✅ User registration with input validation  
✅ Secure login using session handling  
✅ MySQL database connectivity  
✅ Error management (via `errors.php`)  
✅ Basic interface styling (`style.css`)  
✅ Product page accessible only to logged-in users (`product.php`)

---

## 📁 Project Structure

- **index.php** → Home page  
- **register.php** → User registration form  
- **login.php** → Login page  
- **server.php** → Handles login & registration logic  
- **errors.php** → Displays validation errors  
- **product.php** → Protected page (only for logged users)  
- **style.css** → Frontend styling  
- **README.md** → Project documentation  


---

## ⚙️ How to Run the Project

### 🧩 Step 1: Clone the Repository
```bash
git clone https://github.com/LakshyaShrree/php-mysql-login-system.git

🌐 Step 2: Set Up Local Server

Use XAMPP or WAMP and move the project folder into:
C:\xampp\htdocs\

🗄️ Step 3: Create a MySQL Database

Open phpMyAdmin → http://localhost/phpmyadmin

Create a new database (e.g., login_system)

Create a users table with this structure:
CREATE TABLE users (
  id INT(11) AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50) NOT NULL,
  email VARCHAR(100) NOT NULL,
  password VARCHAR(255) NOT NULL
);


🔧 Step 4: Update Database Connection

Edit your credentials inside server.php:
$db = mysqli_connect('localhost', 'root', '', 'login_system');


▶️ Step 5: Run the Project

Start Apache & MySQL in XAMPP, then open:
👉 http://localhost/php-mysql-login-system/index.php

🧠 Workflow

Register → User details stored in MySQL database.

Login → Credentials verified and session created.

Product Page → Accessible only to logged-in users.

Logout → Destroys session and redirects to login page.

💡 Future Improvements 

Add password reset via email.

Use password_hash() and password_verify() for encryption.

Create admin dashboard to manage users.

Add profile picture upload feature.

Improve UI using Bootstrap or Tailwind CSS.

👩‍💻 Author

Lakshya Shree Hariharan
📧 lakshyashreeh@gmail.com
https://www.linkedin.com/in/lakshya-shree-h
