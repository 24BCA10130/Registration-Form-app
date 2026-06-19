# Registration-Form-app

# Android SQLite CRUD Application

A simple Android application built using **Kotlin** and **SQLite** that demonstrates basic CRUD (Create, Read, Update, Delete) operations.

## Features

### User Registration

* Register users with:

  * Username
  * Email
  * Password
* Stores user data in SQLite database.
* Displays success/failure messages using Toast.

### Login Screen

* Simple login interface.
* Navigation to the CRUD operations page.

### CRUD Operations

* **View Data** – Display all registered users.
* **Update Data** – Update email and password using username.
* **Delete Data** – Remove a user record using username.

---

## Technologies Used

* Kotlin
* Android Studio
* SQLite Database
* ConstraintLayout
* AlertDialog
* Intent Navigation

---

## Project Structure

```plaintext
app/
└── java/com/example/training/
    ├── MainActivity.kt       # Registration Screen
    ├── MainActivity2.kt      # Login Screen
    ├── Mainlist.kt           # CRUD Operations Screen
    └── DBHelper.kt           # SQLite Helper Class

res/
└── layout/
    ├── activity_main.xml
    ├── activity_main2.xml
    └── activity_mainlist.xml
```

---

## Database Schema

### Table: users

| Column   | Type |
| -------- | ---- |
| username | TEXT |
| email    | TEXT |
| password | TEXT |

```sql
CREATE TABLE users (
    username TEXT,
    email TEXT,
    password TEXT
);
```

---

## Application Flow

```plaintext
Registration Screen
        ↓
Login Screen
        ↓
Options Screen
    ├── View Data
    ├── Update Data
    └── Delete Data
```

---

## Screens Included

### Registration Screen

* User enters username, email, and password.
* Data is saved into SQLite database.

### Login Screen

* Provides login UI.
* Allows navigation to the options page.

### Options Screen

Contains:

* View Data
* Update Data
* Delete Data

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/android-sqlite-crud.git
```

2. Open the project in Android Studio.

3. Sync Gradle files.

4. Run the app on:

   * Android Emulator
   * Physical Android Device

---

## Learning Objectives

This project demonstrates:

* SQLite Database Integration
* Android Activity Navigation
* CRUD Operations
* Kotlin Basics
* AlertDialog Usage
* Toast Messages
* ConstraintLayout Design

---

## Future Enhancements

* Login Authentication
* Password Encryption
* Input Validation
* Search Functionality
* RecyclerView for Data Display
* Room Database Integration
* MVVM Architecture

---

## Author

Developed for learning Android development with Kotlin and SQLite.

---

## License

This project is open-source and available for educational purposes.
