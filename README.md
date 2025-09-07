# Library Management System

A simple and efficient Library Management System built with Flask and SQLite. This project automates book management, user interactions, and transaction tracking with role-based access for admins and members.

---

## ✨ Features

-   **User Authentication**: Secure login and registration for members and admins.
-   **Role-Based Access Control**:
    -   **Admin**: Can manage the entire library, add/delete books, and view all transactions.
    -   **Member**: Can search for books, borrow, and return them.
-   **Book Management**: Admins can easily add new books and manage the existing catalog.
-   **Transaction Tracking**: All borrow and return activities are logged with timestamps.
-   **Responsive UI**: The interface is built with Bootstrap for a seamless experience on desktops, tablets, and mobile devices.
-   **Reporting Dashboard**: Admins have a dashboard to monitor key metrics like total books, total members, and overdue books.
-   **Search Functionality**: Users can easily search the library catalog by title or author.

---

## 🛠️ Tech Stack

-   **Backend**: Flask (Python)
-   **Database**: SQLite
-   **Frontend**: HTML, CSS, JavaScript
-   **UI Framework**: Bootstrap 5

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

-   Python 3.6+
-   `pip` for package management

### Installation & Setup

1.  **Clone the repository**

2.  **Create and activate a virtual environment:**
    ```sh
    # For Windows
    python -m venv venv
    .\venv\Scripts\activate

    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the required dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

4.  **Initialize the database:**
    This command will create the `library.db` file, set up the tables, and create a default admin user.
    ```sh
    python database.py
    ```
    -   **Default Admin Credentials:**
    -   **Username**: `admin`
    -   **Password**: `adminpassword`

5.  **Run the Flask application:**
    ```sh
    flask run
    ```
    The application will be available at `http://127.0.0.1:5000`.

---

## Usage

1.  Navigate to `http://127.0.0.1:5000`.
2.  Log in with the admin credentials or register as a new member.
3.  **Admins** can add/delete books and monitor all activity from the admin dashboard.
4.  **Members** can search for available books, borrow them, and see their currently borrowed items on their dashboard.
