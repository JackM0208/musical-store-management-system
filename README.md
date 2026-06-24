# 🎸 Music Store Management System

## 📖 Overview
The Music Store Management System is a comprehensive desktop application developed to streamline inventory operations for music store employees. Designed to manage musical instruments efficiently, this system minimizes manual tracking errors and provides a centralized platform for staff to oversee store assets. 

This project was developed as a core assignment for the Object-Oriented Programming (OOP) module, demonstrating the practical application of OOP principles, relational database management, and modern GUI development.

## 🏗️ Architecture
The system is engineered using a robust **3-Tier Architecture (View - Controller - Storage)**, ensuring a clean separation of concerns, scalability, and ease of maintenance:

*   **View Layer (Presentation):** Responsible for the user interface and user interactions. Initial UI/UX layouts were prototyped using **Figma**, ensuring an intuitive user journey, before being strictly implemented using **JavaFX** and **SceneBuilder**.
*   **Controller Layer (Business Logic):** Acts as the bridge between the View and the Storage layers. It processes user inputs, enforces business rules (e.g., data validation for instrument prices and stock levels), and handles the core application logic.
*   **Storage Layer (Data Access):** Manages all database interactions. It executes SQL queries to persist, update, retrieve, and delete instrument records from the underlying relational database securely.

## 💻 Tech Stack
*   **Language:** Java
*   **Build Tool:** Maven (Dependency management and project building)
*   **GUI Framework:** JavaFX (FXML)
*   **UI Prototyping & Layout:** Figma, SceneBuilder
*   **Database:** MySQL
*   **Paradigm:** Object-Oriented Programming (OOP)

## ✨ Core Features
*   **Dashboard Overview:** A centralized view displaying current inventory metrics and low-stock alerts.
*   **Instrument Management (CRUD):**
    *   **Create:** Add new musical instruments with details such as category (e.g., Guitars, Keys, Percussion), brand, model, price, and stock quantity.
    *   **Read:** Search and filter instruments based on specific criteria.
    *   **Update:** Modify existing instrument details or restock quantities.
    *   **Delete:** Remove discontinued or damaged items from the system.
*   **Employee Access:** Secure environment tailored specifically for store staff operations.

## ⚙️ Installation & Setup

### Prerequisites
*   [Java Development Kit (JDK) 11+](https://www.oracle.com/java/technologies/downloads/)
*   [Apache Maven](https://maven.apache.org/download.cgi)
*   [MySQL Server](https://dev.mysql.com/downloads/mysql/)

### Local Development Setup
1. **Clone the repository:**
   `git clone https://github.com/YOUR_GITHUB_USERNAME/music-store-management.git`
   `cd music-store-management`

2. **Database Configuration:**
   * Open your MySQL client and create a new database: `CREATE DATABASE music_store_db;`
   * Execute the provided `schema.sql` (located in the `src/main/resources/db` directory) to generate the necessary tables.
   * Update the database credentials (URL, Username, Password) in the Storage layer configuration file (e.g., `application.properties` or `DatabaseConnection.java`).

3. **Build the project:**
   `mvn clean install`

4. **Run the application:**
   `mvn javafx:run`

## 🤝 Contributors
*   **Phan Anh Minh** - *Core Logic, UI/UX Design & Architecture*
*   *(Add teammate names and roles here)*

---
*Developed during the Winter Semester - Object-Oriented Programming Course.*
