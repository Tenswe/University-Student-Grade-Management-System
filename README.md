T-SQL UNIVERSITY MANAGEMENT SYSTEM




🚀 Project Overview
This project models the core student, course, instructor, and grading management processes within a university environment using T-SQL. The primary goals are to ensure data integrity, automate complex operations, and facilitate reporting processes.

🛠️ Technologies
Database Engine: Microsoft SQL Server

Programming Language: T-SQL (Transact-SQL)

Development Environment: SQL Server Management Studio (SSMS)

✨ Key Features (Implemented Database Structures)
The system is built on a robust foundation incorporating advanced T-SQL components:


Data Model & Integrity: Includes core tables like Students, Instructors, Courses, Enrollments, and Grades. All tables are properly related using PRIMARY KEY and FOREIGN KEY constraints.


Stored Procedures (SP): Procedures are designed to handle complex, multi-step operations efficiently (e.g., calculating the average for all students). Error handling using the TRY...CATCH structure is included.


User-Defined Functions (UDFs): A function is implemented to calculate a student's average and determine their "Passed / Failed" status using a CASE structure.


Triggers: A trigger automatically calculates the average and updates the GecisDurumu (Pass/Fail Status) table whenever a new grade is added, ensuring the database remains self-managing.


Transaction Management: The Transaction structure is applied to critical operations (COMMIT on success, ROLLBACK on error) to guarantee data consistency and atomicity.

Reporting Tools:

Views (VIEW): A view simplifies reporting by combining student names, courses, grades, and calculated averages.

Pivot Table: A PIVOT report structure is designed to display course averages in a clear, cross-tabular format.

Indexing: INDEXes are planned and created on frequently queried fields to optimize query performance.


Advanced Features: Logic to automatically add students with an average of 90+ to an "OnurListesi" (Honor Roll) table is included.

⚙️ Setup and Execution
Install SQL Server: Ensure Microsoft SQL Server and SSMS are installed on your machine.

Create Database: Create a new database named UniversiteSistemi in SSMS.

Run Scripts: Execute the provided T-SQL scripts in the correct order:

Start with schema creation (tables and constraints).

Follow with data insertion, then functions, triggers, and stored procedures.

Finally, execute reporting and performance scripts (VIEWs, INDEXes).

✅ Project Completion Status
All tables are functioning with established relationships.

Functions, triggers, and stored procedures are active.

Error management and transaction structures are in place.

Reporting and performance tools (view, pivot, index) are complete.

The system operates as an automatically managing mini-database
