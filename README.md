# Logbook

Week (1) 10 hours
Cisco Networking Academy: Introduction to Cybersecurity

PortSwigger Labs Completed

SQL Injection: Nov/10, Table, Done
Authentication: Nov/10, Table, Done
Access Control: Nov/10, Table, Done





Week (2) 30 hours
PortSwigger
In this lab, we exploited an SQL injection vulnerability to bypass category and release constraints, displaying all products.

On November 17, 2024, I completed 3 PortSwigger labs using ZAP: SQL Injection, Authentication, and Access Control. I learned how to capture and modify HTTP requests, understand SQL injection vulnerabilities, and automate security testing. Challenges included syntax and tool integration, but instructions were clear. I gained valuable insights into identifying web app vulnerabilities.

In the Introduction to Cybersecurity course, I progressed as follows:

Knowledge Check: 100%
Module 1: 53%
Module 2: 61%
Module 3: 72%
Module 4: 5%
Module 5: Not yet started



Week (3) 20 hours
The Booking system project - Phase 1

Developed and tested a registration page using Docker and Deno.
Analyzed SQL injection vulnerabilities with PortSwigger and ZAP, simulating attacks like +OR+1=1--.
Investigated login system issues, including username enumeration and access control vulnerabilities.
Conducted automated security tests with ZAP on the server.
Updated findings and results in the logbook and GitHub repo with classmate assistance.

The following tasks were successfully completed:

Docker database created and tested.
booking_system_structure.sql added.
Registration page implemented in Deno.
Functionality test performed.
Vulnerability tests done, issues fixed, and two Checkmarx ZAP reports added.





Week (4) 15 hourse
The Booking system project - Phase 2

The following tasks were successfully completed:

Login page implemented with logging feature (GDPR compliant).
Functionality and vulnerability tests done for login.
Index page implemented, and system tests (functionality and vulnerability) conducted.
Two Checkmarx ZAP reports generated and added to the git repo.


Phase 1 established a solid foundation for the Booking System Project by setting up the development environment and core functionalities. The registration page (localhost:8000/register) was successfully implemented and tested, though some login functionality issues persisted. Despite this, functionality and vulnerability tests were completed, and Checkmarx ZAP reports were generated, converted to MD format, and added to the repository.

In Phase 2, the login page (localhost:8000) was successfully implemented and tested in Docker and Visual Studio Code after troubleshooting. Tutorial videos and guidance from a friend helped resolve issues efficiently. Security tests with ZAP produced reports like "User Agent Fuzzer | Informational | 24 |" and a HAR report. Browser challenges were resolved by switching to Microsoft Edge.


Week (5) 15 hours
The Booking system project - Phase 3

The project continued, focusing on authorization, logging, security testing, and GDPR. The updated index page with reservation features was implemented, tested, and submitted. Git repo and logbook updated.

- Weak password management → Fix hashing.
- Insufficient access control → RBAC must be implemented.
- Lack of input validation → Add XSS protection.
- Session vulnerability → Add a timeout and flags.
- Open API → Authentication must be added.


I started by reviewing lecture materials and videos. After resolving issues with incorrect files and starting fresh, I implemented and tested the reservation system on localhost:8000. Challenges included fixing small mistakes, implementing features like session management, and ensuring proper user inputs. I spent 15 hours, learned valuable lessons, and identified key areas for improvement: password hashing, RBAC, input validation, session timeout, and API authentication. Despite frustration, I successfully completed the task.



Week (6) 10 hourse
The Booking system project → Phase 4 (15.12.2024)

I created a new Docker container, restructured the database by removing the zephyr_users table, and added the booking system structure SQL. Successfully tested the localhost account page, ensuring full functionality.

Addressing GDPR concerns, explicit consent is essential for data processing, as required by GDPR. Without it, user rights remain unprotected, causing potential legal risks and reduced trust. Example: BBC's cookie management page.

Changes made:

Updated the empty privacy policy and terms of service.
Verified full compliance with GDPR requirements.



Week (7) 20 hourse
The Booking system project - Final phase


The assignment has been completed. A document was created with all required sections, including reflections on each topic. Screenshots were added for course completions, labs, and the booking system project. The Git repo and logbook were updated accordingly, and the document has been submitted.





# The booking system
1. Create a database
    1. Install Docker: https://www.docker.com/
    2. Load the postgres image: docker pull postgres
    3. Create a container: docker run --name booking_system_database -e POSTGRES_PASSWORD=Secret1234! -d -p 5432:5432 postgres
    4. Connect to the database: docker exec -it booking_system_database psql -U postgres -d postgres
    5. Copy the file booking_system_structure.sql to the clipboard.
    6. Paste the file into the psql terminal
2. Run the command: deno run --allow-net --allow-env --allow-read --watch app.js

# Pages
0. http://localhost:8000 --> GET
1. http://localhost:8000/register --> GET and POST
2. http://localhost:8000/login --> GET and POST
3. http://localhost:8000/logout --> GET
4. http://localhost:8000/resources --> GET and POST
5. http://localhost:8000/reservation --> GET and POST
6. http://localhost:8000/resourcesList --> GET
7. http://localhost:8000/terms --> GET
8. http://localhost:8000/privacynotice --> GET
9. http://localhost:8000/account --> GET
10. http://localhost:8000/accountInfo --> GET


