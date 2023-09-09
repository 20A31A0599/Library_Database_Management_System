
<body>

<h1>Library Management System</h1>

<p>The Library Management System is a Python application built using the Tkinter library for the graphical user interface and pymysql for database connectivity. It serves as a tool for managing a library's inventory and tracking book issuances.</p>

<h2>Features</h2>

<ul>
<li>Librarian Interface:</li>
<ul>
<li>Add books to the library database.</li>
<li>Issue and return books to/from students.</li>
<li>View available books.</li>
<li>View books that have been issued.</li>
<li>Delete books from the database.</li>
</ul>
<li>Admin Interface:</li>
<ul>
<li>Add and manage users (librarians or other admins).</li>
<li>View user information.</li>
<li>Delete users.</li>
</ul>
</ul>

<h2>Prerequisites</h2>

<ul>
<li>Python 3.6 or higher</li>
<li>pymysql</li>
</ul>

<h2>Usage</h2>

Clone or download this repository.
Navigate to the project directory:
cd Library-Management-System


3. Run the application:

python library_management_system.py

Log in as a librarian or an admin.
For librarians, you can manage books, issue/return books, etc.
Admins can add/manage users.
<h2>Database Setup</h2>

The application uses a MySQL database to store book and user information. You need to set up a MySQL server and create the necessary database and tables. Here are the steps:

Install MySQL on your system if it's not already installed.

Start the MySQL server.

Create a new database named Library.

Create the following tables within the Library database:

Book: To store book information (subject, title, author, serial number).
BookIssue: To track book issuance (student ID, serial number, issue date, expiry date).
Login: To store user information (name, user ID, branch, mobile number).
Update the database connection details in the code (library_management_system.py) to match your MySQL server configuration:

con = p.connect(host="localhost", user="root", password="your_mysql_password", database="Library")

<h2>Contributing</h2>

Contributions are welcome! If you find any bugs, want to add new features, or have suggestions for improvements, please feel free to open an issue or submit a pull request.
