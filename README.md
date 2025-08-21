:

📚 Library Management System (Java + Swing)

This is a simple Library Management System built in Java with a Swing GUI. It allows users to manage library items such as books, CDs, DVDs, and journals. The system supports borrowing, returning, and listing available items.

✨ Features

Add new items (Books, EBooks, Reference Books, CDs, DVDs, Journals)

List available items with their title, author, and ISBN

Borrow items (only borrowable items like Books, CDs, DVDs, and EBooks)

Return items and mark them as available again

GUI interface with buttons for common actions (Add, List, Borrow, Return, Exit)

🏗️ Project Structure

LibraryItem (Abstract Class):
Base class for all items in the library (title, author, ISBN, availability, quantity).

Borrowable (Interface):
For items that can be borrowed (e.g., PhysicalBook, CD, DVD, EBook).

Item Classes:

PhysicalBook

EBook

ReferenceBook (cannot be borrowed)

CD

DVD

Journal (cannot be borrowed)

Library:
Stores all items and handles add, borrow, return, and list operations.

LibraryUser:
Represents a user who can borrow and return items.

LibraryGUI (Main Class):
Provides the Swing-based graphical interface with buttons and dialogs.

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/library-management-system.git
cd library-management-system


Compile the Java files:

javac LibraryGUI.java


Run the program:

java LibraryGUI

📷 GUI Preview

Main Window: Welcome screen with buttons (Add Item, List Items, Borrow, Return, Exit)

Add Item: Form to input type, title, author, ISBN, and copies

List Available Items: Shows all currently available items

Borrow Item: Lets a user borrow a book/CD/DVD if available

Return Item: Allows a user to return borrowed items

📌 Notes

Reference books and journals cannot be borrowed.

EBooks are considered always available.

Borrowable items decrease in quantity when borrowed and are marked unavailable when copies reach 0.
