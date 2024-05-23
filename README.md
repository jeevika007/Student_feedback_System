
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
## Usage
**Admin Login**
- Open the application in your web browser.
- Log in using your admin credentials.
- Access the admin dashboard to manage feedback and change passwords.
**Student Feedback Submission**
- Navigate to the feedback submission form.
- Fill in the required fields and submit your feedback.
## Security Measures
- **Session Management:**
    - Admin sessions are managed to maintain login state securely.
- **Password Hashing:**
    - Admin passwords are hashed using SHA1 before storing in the database.
- **SQL Injection Prevention:**
    - Parameterized queries are used to prevent SQL injection attacks.
## Future Enhancements
- **Improved Password Security:**
    - Upgrade password hashing algorithm to bcrypt for better security.
- **User Authentication:**
    - Implement authentication for students to ensure only registered students can submit feedback.
## Acknowledgements

 I would like to express my sincere gratitude to all those who have contributed to the successful completion of this project, including my DBMS professor, peers, the open-source community, and my friends and family.



