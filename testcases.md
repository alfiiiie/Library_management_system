# Library Management System - Test Cases

## Objective
To verify that each story in the storyboard works correctly, based on the use case, activity and data flow diagrams.

## Test Case 1 - Student Registration

**Test Input:** Student enters name, email and password.

**Expected Result:** The system creates the account and stores the student's details.

**Progress:** Completed

## Test Case 2 - Registration with Existing Email

**Test Input:** Student registers with an email that already exists.

**Expected Result:** The system shows an error message and does not create a duplicate account.

**Progress:** Completed

## Test Case 3 - Search Book

**Test Input:** Student searches a book by title or author.

**Expected Result:** The system displays matching books and their availability.

**Progress:** Completed

## Test Case 4 - Search Unavailable Book

**Test Input:** Student searches a book that is not in the library.

**Expected Result:** The system shows "No books found".

**Progress:** Completed

## Test Case 5 - Issue Book

**Test Input:** Student requests to borrow an available book.

**Expected Result:** The system records the issue date and due date.

**Progress:** In Progress

## Test Case 6 - Return Book with Fine

**Test Input:** Student returns a book after the due date.

**Expected Result:** The system updates availability and calculates the fine.

**Progress:** To Do

## Test Case 7 - Borrowing History

**Test Input:** Student opens borrowing history.

**Expected Result:** The system displays previously issued books.

**Progress:** To Do
