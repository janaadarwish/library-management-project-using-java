# 📚 Library Management System — Java

A full-featured **GUI-based Library Management System** built in Java using **Java Swing**, developed as a university project at Helwan University. The system supports multiple user roles with dedicated dashboards, book management, reservations, notifications, and checkout history — all persisted via CSV files.

---

## 🖼️ Preview

> _Add screenshots of your GUI here._  
> Example: `![Dashboard](assets/dashboard.png)`

---

## ✨ Features

### 👤 User Roles
- **Admin** — Full system control, manage users and librarians
- **Librarian** — Manage books, handle reservations and returns
- **Patron** — Browse books, borrow, reserve, and track history

### 📖 Book Management
- Add, update, display, and search books
- Track book status and genre

### 🔄 Borrowing & Returns
- Borrow and return books through dedicated GUI screens
- Full checkout history tracking

### 🔔 Reservations & Notifications
- Patrons can request and reserve books
- Librarians can accept reservation requests
- Notification system for updates

### 💾 Data Persistence
- All data stored and loaded via CSV files:
  - `Library.csv` — Book catalog
  - `Users.csv` — User accounts
  - `CheckoutHistory.csv` — Borrowing records
  - `Notifications.csv` — System notifications
  - `reservationRequests.csv` — Pending reservations

---

## 🛠️ Built With

- **Java** — Core programming language
- **Java Swing** — GUI framework
- **CSV Files** — Lightweight data persistence
- **OOP Principles** — Encapsulation, inheritance, polymorphism, abstraction

---

## 📁 Project Structure

```
Library_Management/
├── main.java                    # Entry point
├── LoginGUI.java                # Login screen
├── SignupGUI.java               # Signup screen
│
├── Admin.java                   # Admin model
├── AdminDashboardGUI.java       # Admin dashboard
├── AdminLoginGUI.java           # Admin login
├── UpdateByAdminGUI.java        # Admin update user
│
├── Librarian.java               # Librarian model
├── LibrarianDashboardGUI.java   # Librarian dashboard
├── LibrarianLoginGUI.java       # Librarian login
│
├── Patron.java                  # Patron model
├── PatronDashboardGUI.java      # Patron dashboard
├── PatronLoginGUI.java          # Patron login
├── PatronHistoryGUI.java        # Borrowing history
│
├── Book.java                    # Book model
├── AddBookGUI.java              # Add book screen
├── DisplayBookGUI.java          # Display books
├── SearchBookGUI.java           # Search books
├── UpdateBookDataGUI.java       # Update book info
│
├── RequestReserveGUI.java       # Patron reservation request
├── ReservationRequestGUI.java   # View reservation requests
├── AcceptReservationGUI.java    # Accept reservations
├── ReturnBookGUI.java           # Return book screen
├── CheckoutHistoryGUI.java      # Checkout history
├── NotificationsGUI.java        # Notifications screen
│
├── User.java                    # Base user class
├── AccountType.java             # Account type enum
├── BookStatus.java              # Book status enum
├── Genre.java                   # Genre enum
│
├── Library.csv                  # Book data
├── Users.csv                    # User data
├── CheckoutHistory.csv          # Borrow records
├── Notifications.csv            # Notifications
└── reservationRequests.csv      # Reservation requests
```

---

## ⚙️ Getting Started

### Prerequisites
- Java JDK 8 or higher
- Any Java IDE (IntelliJ IDEA, Eclipse, VS Code)

### Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/janaadarwish/library-management-project-using-java.git
   ```

2. Open the project in your IDE

3. Compile and run `main.java`

---

## 🧠 OOP Concepts Applied

- **Encapsulation** — Private fields with getters/setters across all models
- **Inheritance** — `Admin`, `Librarian`, and `Patron` extend the base `User` class
- **Polymorphism** — Shared methods overridden per user role
- **Abstraction** — Business logic separated from GUI layer
- **Enums** — `AccountType`, `BookStatus`, and `Genre` for type safety

---

## 🔧 Possible Future Improvements

- [ ] Replace CSV storage with a proper database (MySQL / SQLite)
- [ ] Add due date tracking and fine calculation for late returns
- [ ] Improve UI design with JavaFX
- [ ] Add email notifications for reservations and due dates
- [ ] Implement search/filter by genre, author, or availability

---

## 👩‍💻 Author

**Jana Amin** — [@janaadarwish](https://github.com/janaadarwish)  
Computer Science Student @ Helwan University | AI & ML Enthusiast  
[LinkedIn](https://www.linkedin.com/in/jana-darwish-29613732b/) · [Kaggle](https://www.kaggle.com/janadarwish)
