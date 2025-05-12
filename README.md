# 🧑‍💼 Node.js User Management System

A CRUD-based user management web app built with **Node.js**, **Express**, **Express-Handlebars (HBS)**, and **MySQL**.

## 📦 Features

- View, add, edit, delete, and search users
- Handlebars template engine with Bootstrap styling
- MySQL database integration
- Modular MVC architecture

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory and add your database credentials:

```
DB_HOST=localhost
DB_NAME=usermanagement_tut
DB_USER=root
DB_PASS=your_mysql_password
```

---

## 💽 Database Setup

Use **MySQL Workbench** (or any MySQL client) to set up your database:

### Create the Database

```sql
CREATE DATABASE usermanagement_tut;
USE usermanagement_tut;
```

### Create the `user` Table

```sql
CREATE TABLE user (
  id INT NOT NULL AUTO_INCREMENT,
  first_name VARCHAR(45) NOT NULL,
  last_name VARCHAR(45) NOT NULL,
  email VARCHAR(45) NOT NULL,
  phone VARCHAR(45) NOT NULL,
  comments TEXT NOT NULL,
  status VARCHAR(10) NOT NULL DEFAULT 'active',
  PRIMARY KEY (id)
) ENGINE=InnoDB;
```

### Insert Sample Users

```sql
INSERT INTO user (id, first_name, last_name, email, phone, comments, status) VALUES
(NULL, 'Amanda', 'Nunes', 'anunes@ufc.com', '012345678910', '', 'active'),
(NULL, 'Alexander', 'Volkanovski', 'avolkanovski@ufc.com', '012345678910', '', 'active'),
(NULL, 'Khabib', 'Nurmagomedov', 'knurmagomedov@ufc.com', '012345678910', '', 'active'),
(NULL, 'Kamaru', 'Usman', 'kusman@ufc.com', '012345678910', '', 'active'),
(NULL, 'Israel', 'Adesanya', 'iadesanya@ufc.com', '012345678910', '', 'active'),
(NULL, 'Henry', 'Cejudo', 'hcejudo@ufc.com', '012345678910', '', 'active'),
(NULL, 'Valentina', 'Shevchenko', 'vshevchenko@ufc.com', '012345678910', '', 'active'),
(NULL, 'Tyron', 'Woodley', 'twoodley@ufc.com', '012345678910', '', 'active'),
(NULL, 'Rose', 'Namajunas', 'rnamajunas@ufc.com', '012345678910', '', 'active'),
(NULL, 'Tony', 'Ferguson', 'tferguson@ufc.com', '012345678910', '', 'active'),
(NULL, 'Jorge', 'Masvidal', 'jmasvidal@ufc.com', '012345678910', '', 'active'),
(NULL, 'Nate', 'Diaz', 'ndiaz@ufc.com', '012345678910', '', 'active'),
(NULL, 'Conor', 'McGregor', 'cmcgregor@ufc.com', '012345678910', '', 'active'),
(NULL, 'Cris', 'Cyborg', 'ccyborg@ufc.com', '012345678910', '', 'active'),
(NULL, 'Tecia', 'Torres', 'ttorres@ufc.com', '012345678910', '', 'active'),
(NULL, 'Ronda', 'Rousey', 'rrousey@ufc.com', '012345678910', '', 'active'),
(NULL, 'Holly', 'Holm', 'hholm@ufc.com', '012345678910', '', 'active'),
(NULL, 'Joanna', 'Jedrzejczyk', 'jjedrzejczyk@ufc.com', '012345678910', '', 'active');
```

---

## 🚀 Run the App

```bash
npm start
```

Visit `http://localhost:3000` in your browser.

---

## 📂 Folder Structure

```
.
├── app.js
├── .env
├── views/
│   ├── home.hbs
│   ├── add-user.hbs
│   └── partials/
│       └── user-form.hbs
├── public/
├── routes/
├── controllers/
└── package.json
```

---

## ✅ Requirements

- Node.js
- MySQL Server (e.g., MySQL Workbench)
- Modern browser