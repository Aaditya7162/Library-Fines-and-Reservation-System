📚 Library Fines and Reservation System (CLI)
✅ Overview

The Library Fines and Reservation System is a Python-based Command Line Interface (CLI) application designed to manage essential library activities such as book borrowing, reservations, returns, and fine calculation. It provides a simple and structured digital alternative to manual library record-keeping. The system is lightweight, runs entirely in the terminal, and stores data in .txt files for persistence across sessions.

This system is suitable for small to medium libraries, schools, or individual use.

✨ Features

Book Catalogue Management
Add, search, and view available books.

Book Issue & Return System
Records issue and return dates, and calculates late fines.

Reservation System
Users can reserve books already borrowed; allocation is handled on a queue basis.

Fine Calculation & Tracking
Automatically calculates overdue fines and maintains payment status.

User Login Authentication
Basic login system to restrict access to authorized users only.

Persistent Data Storage
Book and user records are stored in .txt files.

🧠 Section-Wise Code Explanation
1. Data Storage & File Handling

The program uses text files to store information such as book records, issued books, and user details. This allows the system to retain data even after the program is closed.

2. User Authentication

A simple login system validates username and password before giving access to the main menu. This prevents unauthorized use.

3. Menu-Driven Program Structure

After login, users interact with the system using a menu. Each menu option triggers a function responsible for one core library feature. This modular approach keeps the code structured and readable.

4. Book Management

Functions allow adding new books, searching for books, and displaying all available books. The system stores book details such as title, author, and quantity.

5. Issue, Return & Reservation Handling

The system records issue/return dates and checks for overdue duration to compute fines. If a book is unavailable, the reservation system places the user in a waiting queue and allocates the book once returned.

🧑‍💻 User Manual (How to Use)
🔹 Running the Program

Install Python (if not installed).

Place all program .py files and data .txt files in the same folder.

Run the file using:

python library_system.py

🔹 Login

Enter the correct username and password to access the system.

Example:

Enter Username: admin
Enter Password: admin123
Login Successful!

🔹 Using the Menu

You will see options like:

1. Add Book
2. View Books
3. Issue Book
4. Return Book
5. Reserve Book
6. Calculate Fine
7. Exit


Enter the option number to perform the task.

🧾 Example Flow (Issuing a Book)
Enter choice: 3
Enter Book Name: Python Basics
Enter Student Name: Riya
Book issued successfully!

🧱 Data Structures Used
-> Feature	Data Structure Used	Purpose
-> Storing book records	List / Text files	Maintain list of all books
-> Issued & Reserved books	Lists / File storage	Track current and reserved books
-> Username & Password	Strings	Authentication
-> Menu navigation	Functions	Modular program design

🚀 Future Enhancements

-> Add a database instead of .txt files (e.g., SQLite, MySQL)

-> Implement role-based access (Admin & Student)

-> Add GUI using Tkinter / PyQt or Web UI with Flask

-> Enable book removal and editing

-> Generate automated fine reports

-> Add email or SMS reminders for due dates
