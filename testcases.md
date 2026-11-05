# Test Cases - Library Management System

| Test Case ID | Test Case | Input | Expected Result |
|--------------|-----------|-------|-----------------|
| TC01 | Register Student | Valid name, email and password | Account should be created and student details saved |
| TC02 | Register With Empty Fields | Empty name or email | Error message should appear |
| TC03 | Register Duplicate Student | Email that is already registered | "Student already exists" error should appear |
| TC04 | Search Book By Title | Valid book title | Matching books should appear with availability |
| TC05 | Search Book By Author | Valid author name | Matching books should appear with availability |
| TC06 | Search Non-existent Book | Title that is not in the library | "No books found" should appear |
| TC07 | Search With Empty Input | Empty search box | Error message or full book list should appear |
| TC08 | Issue Available Book | Valid student ID and available book | Issue date and due date should be recorded |
| TC09 | Issue Unavailable Book | Book that is already issued | "Book not available" error should appear |
| TC10 | Issue Invalid Book | Book ID that does not exist | Error message should appear |
| TC11 | Return Book On Time | Valid issued book returned before due date | Book should become available and fine should be 0 |
| TC12 | Return Book Late | Valid issued book returned after due date | Book should become available and fine should be calculated |
| TC13 | Return Book Not Issued | Book that was never issued to the student | Error message should appear |
| TC14 | View Borrowing History | Open borrowing history of a student | All previously issued books should appear |
| TC15 | View Empty History | Student with no borrowed books | "No borrowing history" should appear |
