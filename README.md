📚 Library Management System
A comprehensive console-based Library Management System built in Python that allows librarians to manage books, track issues/returns, generate statistics, and persist data.

🎯 Features
Core Operations
Add Books: Add new books with ID, title, author, category, and quantity

View All Books: Display all books in a formatted table

Search Books: Search by Book ID or Title (partial matching supported)

Update Books: Modify existing book information

Delete Books: Remove books from the library (with confirmation)

Issue & Return Management
Issue Books: Issue books to students with automatic stock updates

Return Books: Return borrowed books with stock replenishment

Availability Check: Prevents issuing unavailable books

Statistics & Reports
Total Books Count: View total number of books

Category Distribution: See unique book categories

Most Issued Book: Identify the most popular book

Available vs Issued Books: Track library inventory health

Data Persistence
Save Data: Save library records to a text file

Load Data: Automatically load saved data on startup

Auto-save Reminder: Prompt to save before exit

Practice Problems
Includes 5 LeetCode-style programming problems:

Reverse Book Titles

Find Book with Highest Quantity

Merge Two Library Catalogs

Count Books in a Category

Find Book by ID

🚀 Getting Started
Prerequisites
Python 3.6 or higher

No external libraries required (uses only standard library)

Installation
Clone the repository:

bash
git clone https://github.com/yourusername/library-management-system.git
cd library-management-system
Run the application:

bash
python Library_Management_system_Python_project.py
📖 Usage Guide
Main Menu Options
text
1. Add Book          - Add a new book to the library
2. View All Books    - Display all books in the catalog
3. Search Book       - Find a book by ID or title
4. Update Book       - Modify book details
5. Delete Book       - Remove a book (with confirmation)
6. Issue Book        - Issue a book to a student
7. Return Book       - Return a borrowed book
8. Library Statistics - View library summary statistics
9. Save Data         - Save current data to file
10. Load Data        - Load data from file
11. Practice Problems - Run coding practice problems
12. Exit            - Exit the application
Data File Format
The library data is stored in library_data.txt with the following format:

text
book_id,title,author,category,quantity,issued_count
B001,The Great Gatsby,F. Scott Fitzgerald,Fiction,5,2
B002,1984,George Orwell,Dystopian,3,1
📊 Data Structure
Each book is stored as a dictionary with the following fields:

Field	Type	Description
book_id	String	Unique identifier for the book
title	String	Book title
author	String	Book author(s)
category	String	Book category/genre
quantity	Integer	Available copies
issued_count	Integer	Total times issued
🛠️ Code Structure
text
Library Management System
├── Global Variables
│   └── books list, DATA_FILE
├── Data Persistence Functions
│   ├── load_data()
│   └── save_data()
├── Core CRUD Operations
│   ├── add_book()
│   ├── view_books()
│   ├── search_book()
│   ├── update_book()
│   └── delete_book()
├── Issue/Return Operations
│   ├── issue_book()
│   └── return_book()
├── Statistics
│   └── generate_statistics()
├── Practice Problems
│   ├── reverse_titles()
│   ├── highest_quantity()
│   ├── merge_catalogs()
│   ├── count_category()
│   └── find_book_by_id()
└── Main Menu
    └── main()
💡 Key Features Explained
Data Persistence
Automatically loads data when the program starts

Saves data manually through the menu

Uses CSV-style format for easy backup and editing

Input Validation
Prevents duplicate Book IDs

Validates numeric inputs (quantity)

Confirms before deleting books

Handles empty inputs gracefully

Search Capabilities
Exact match by Book ID

Partial match by Title (case-insensitive)

Displays all matching books

Statistics
Real-time inventory tracking

Most popular book identification

Category diversity metrics

🔄 Workflow Example
Add a Book:

text
Enter Book ID: B001
Enter Book Title: Python Programming
Enter Book Author: John Doe
Enter Book Category: Technology
Enter Quantity: 5
Book 'Python Programming' added successfully!
Issue a Book:

text
Enter Book ID: B001
Enter Student Name: Alice
Book 'Python Programming' issued to Alice
Remaining copies: 4
View Statistics:

text
Total Books: 10
Total Categories: 5
Most Issued Book: Python Programming (Issued: 3 times)
Available Books: 25
Issued Books: 8
🎓 Learning Outcomes
This project demonstrates:

File I/O operations in Python

CRUD operations with lists and dictionaries

Input validation and error handling

Data persistence techniques

Modular programming concepts

Real-world application development

📝 Future Enhancements
Add user authentication (librarian/student roles)

Implement due date tracking for issued books

Add book reservation system

Create GUI version using Tkinter

Add database support (SQLite/MySQL)

Generate PDF reports

Add barcode scanning support

Email notifications for overdue books

🤝 Contributing
Fork the repository

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👩‍💻 Author
Rida Hafeez
