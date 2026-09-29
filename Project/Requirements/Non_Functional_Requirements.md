**Non-Functional Requirements**

&#x20;

* Raghad Diab Contributions



NFR-01: Security/Authorization - The system should enforce role-based access control, allowing students, internship coordinators, academic supervisors, and company supervisors to access only the information and functions authorized for their roles. 

NFR-02: Security/Session Management - The system should automatically end a session after 30 minutes of inactivity and require the user to authenticate again. 

NFR-03: Reliability - Once an application, placement, logbook, or feedback record has been successfully saved, it should remain available after the user logs out, logs in again, or the application is restarted. 

NFR-04: Data Integrity - The database should enforce relationships and constraints so that placements, supervisor assignments, logbooks, and feedback cannot reference non-existent students, users, or internship records. 

NFR-05: Scalability - The system should support at least 1,000 registered users and 100 simultaneous active users while maintaining stable performance and full access to all core system functions. 





* Miriam Almimi Contributions



NFR-06: Robustness - If a user submits a form containing missing required fields or invalid values, the system shall reject the submission, preserve valid entered information where appropriate, and display a message identifying the field that must be corrected without creating an incomplete database record.

NFR-07: Security - User passwords should be stored using a secure one-way password hashing mechanism and should not be stored or displayed in plain text.

NFR-08: Portability - The web application should support the latest two major versions of Google Chrome, Microsoft Edge, and Mozilla Firefox without loss of core functionality.

NFR-09: Performance - The system should load dashboards, placement information, and logbook lists quickly during normal use and remain responsive when multiple users are using the system at the same time.

NFR-10: Recoverability - Internship application, placement, logbook, and feedback data should be backed up at least once every 24 hours to allow important data to be recovered in case of system failure, corruption, or accidental loss.

