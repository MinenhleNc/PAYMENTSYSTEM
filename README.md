# 🏦 APDS - Task 3  
## International Banking Payment System  

### 👥 Group Members
| Name | Student Number |
|------|----------------|
| Abongile Mazongolo | ST10043271 |
| Minenhle Ncongwane | ST10266839 |
| Favour Ajayi | ST10022295 |
| Tsebo Letele | ST10364068 |

---

## 📘 Overview
The **International Banking Payment System** is a secure web-based payment application that allows customers to register, log in, and make payments.  
Administrators can manage employee accounts, and employees can verify customer payments.  

This system implements:
- Password hashing and salting for secure login  
- Input validation using Regular Expressions (RegEx)  
- HTTPS/SSL enforcement for secure data transmission  
- SonarQube integration for code quality and security analysis  
- Role-based access control (Customer, Employee, Admin)

---

## ⚙️ Technologies Used
- **Node.js**
- **npm (Node Package Manager)**
- **React.js** (Frontend)
- **Express.js** (Backend)
- **MySQL** (Database)
- **bcrypt** (Password hashing)
- **SonarQube** (Code scanning)
- **Visual Studio Code (VS Code)**

---

## 🧩 Installation Guide

### 🧱 Prerequisites
Before running the project, ensure that you have:
- **Node.js** and **npm** installed  
- **MySQL Server** running locally  
- **An IDE** such as Visual Studio Code (VS Code)  

---

### 🔽 Step 1: Clone the Repository
Open your terminal and run:
```bash
[git clone https://github.com/YOUR_GITHUB_USERNAME/international-banking-payment-system.git](https://github.com/MinenhleNc/PAYMENTSYSTEM.git)

🚀 Running the Application
🖥️ Backend Setup

Open a new terminal window in your IDE.

Navigate to the backend folder:

cd backend


Install all backend dependencies:

npm install


Start the backend server:

npm run dev


The backend will start on http://localhost:5000

💻 Frontend Setup

Open another terminal window in your IDE.

Navigate to the frontend folder:

cd frontend


Install all frontend dependencies:

npm install


Start the frontend application:

npm start


The frontend will start on http://localhost:3000

🗄️ Database Configuration

Open MySQL and create a database:

CREATE DATABASE paymentsystem;


Configure the connection details in backend/config/db.js:

host: 'localhost',
user: 'root',
password: 'YOUR_PASSWORD',
database: 'paymentsystem'

🧠 How to Use
📝 Registering a New Account

Launch the frontend application (http://localhost:3000).

You will be directed to the Register page.

Fill in the required fields:

Full Name

ID Number (12 digits)

Account Number (10 digits)

Email

Password

Confirm Password

Click Register to submit your information.
The password will be securely hashed before being stored in the database.

🔐 Logging In

After successful registration, you’ll be redirected to the Login page.

Enter your Email and Password used during registration.

Click Login to access your dashboard.

💳 Making a Payment

After login, you’ll land on the Customer Dashboard.

Fill out the Make a Payment form:

Amount to pay

Currency (choose from dropdown)

Recipient’s Account Number

SWIFT Code

Click Pay Now to complete the transaction.

Your payment will appear in the transaction history below with a Pending status until verified by an employee.

📜 Viewing Transactions

Your transaction history (at the bottom of the dashboard) displays:

Account Number

Amount Paid

Date of Payment

Payment Status (Pending / Verified)

🚪 Logging Out

To securely end your session, click the Logout button at the top-right corner of the dashboard.

👨‍💼 Updated Features
🔑 Employee Login

Employees log in using their Email, Password, and Role.

After authentication, they can access the Employee Dashboard.

🧭 Admin Dashboard

The admin dashboard displays the system logo (top left) and user info with a Logout button (top right).

Admins can:

View all registered employees (email and role)

Create new employee accounts

To create a new employee:

Enter Email, Password, and Role

Click Add Employee

The new employee will appear in the list.

🧾 Employee Dashboard

The Employee Dashboard includes:

System logo (top left)

“Employee” label and Logout button (top right)

Displays a list of customer payments:

Account Number

Amount

Date

Status

Action (Verify)

Employees can review pending payments and mark them as Verified.

🔒 Security Features

Password hashing using bcrypt

RegEx input validation for all fields

SSL/HTTPS enforced

Protection against common attacks:

SQL Injection (parameterized queries)

XSS (input sanitization)

CSRF (token-based protection)

Brute-force (rate limiting)

🧰 SonarQube DevSecOps Integration

SonarQube was used for static code analysis both locally and via cloud to ensure:

No security vulnerabilities

No code smells

Clean, maintainable code

Scan Steps:

Install SonarQube Scanner

Configure the project in sonar-project.properties

Run:

sonar-scanner


View detailed security and quality reports in your SonarQube dashboard.

📺 Video Demonstration

A full video demonstration showing:

Frontend and backend setup

Registration, login, and payment flow

Employee and admin functionality

SonarQube scanning

🎥 YouTube Link: [INSERT YOUR VIDEO LINK HERE]

🧾 Admin Login Credentials
Role	Email	Password
Admin	admin@company.com
	Minimie12@
🧠 Summary

This project successfully implements secure login, payment processing, and verification features following best security practices. It integrates DevSecOps tools (SonarQube) and demonstrates full role-based system functionality across customer, employee, and admin levels.

📜 License

This project is for educational purposes only (APDS - Task 3, 2025).
