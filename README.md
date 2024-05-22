
## Student-feedback-system
## Overview
The Student Feedback System is a web-based application designed to collect and manage feedback from students. This system allows administrators to securely log in, manage passwords, and view feedback submitted by students. The feedback collected can be used to make data-driven decisions to improve the quality of education and services provided by the university.
## Features
**Admin Login:**
- Secure login system for administrators.
**Password Management:**
- Administrators can change their passwords securely.
**Student Feedback Submission:**
- Students can submit feedback through a web form.
**Feedback Storage:**
- Feedback is stored securely in a relational database.
**Security Measures:**
- Includes session management, password hashing, and protection against SQL injection.
## Technology Stack
**Server-Side Scripting Language:** PHP

**Database Management System:**  MySQL

**Web Development:**
- HTML
- CSS
## Database Design

**Tables**

1. **students**

- student_id: INT, Primary Key
- name: VARCHAR(100)
- Other relevant student details
2. **feedback**

- feedback_id: INT, Primary Key
- student_id: INT, Foreign Key referencing students(student_id)
- feedback_text: TEXT
- submission_time: TIMESTAMP
3. **admin**

- aid: VARCHAR(50), Primary Key
- password: VARCHAR(255)
- name: VARCHAR(100)
