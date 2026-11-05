# Library Management System - Test Cases

## Use Case Diagram Test Cases

| ID | Use Case | Input | Expected Output | Status |
|----|----------|-------|-----------------|--------|
| TC01 | Student Registration | Valid name, email, password | Account created successfully | Pass |
| TC02 | Student Registration | Email already registered | Error: email already exists | Pass |
| TC03 | Login | Correct ID and password | Student dashboard opens | Pass |
| TC04 | Login | Wrong password | Error: invalid credentials | Pass |
| TC05 | Search Book | Valid title or author | Matching books are displayed | Pass |
| TC06 | Search Book | Book not in library | Message: no books found | Pass |
| TC07 | Issue Book | Available book | Issue date and due date recorded | In Progress |
| TC08 | Issue Book | Book already issued | Error: book not available | In Progress |
| TC09 | Return Book | Issued book returned on time | Availability updated, no fine | To Do |
| TC10 | Return Book | Book returned after due date | Fine calculated and shown | To Do |

## Activity Diagram Test Cases

| ID | Activity Flow | Condition | Expected Result | Status |
|----|---------------|-----------|-----------------|--------|
| TC11 | Search, then Issue | Book is available | Book issued, status becomes Issued | In Progress |
| TC12 | Search, then Issue | Book is unavailable | Issue request rejected | In Progress |
| TC13 | Issue, then Return | Returned before due date | Status becomes Available | To Do |
| TC14 | Issue, then Return | Returned after due date | Fine added before closing | To Do |
| TC15 | Login | Three wrong attempts | Account locked or warning shown | To Do |

## Data Flow Diagram Test Cases

| ID | Data Flow | Input Data | Expected Data Stored or Output | Status |
|----|-----------|------------|--------------------------------|--------|
| TC16 | Student to Registration to Student Database | Student details | Record saved in Student table | Pass |
| TC17 | Student to Search to Book Database | Search keyword | Book details read from Book table | Pass |
| TC18 | Student to Issue to Issue Records | Book ID, Student ID | Issue record saved with dates | In Progress |
| TC19 | Student to Return to Issue Records and Book Database | Book ID | Issue record closed, book marked Available | To Do |
| TC20 | Return to Fine to Student | Days late | Fine amount calculated and displayed | To Do |
| TC21 | Student to History to Issue Records | Student ID | Previous issued books displayed | To Do |
