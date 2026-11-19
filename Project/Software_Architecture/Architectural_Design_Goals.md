

**Architectural Design Goals:**



DG-01: Security| Users must log in, and each user can only use the functions and see the data allowed for their role (Student, Internship Coordinator, Academic Supervisor, Company Supervisor). Passwords are stored as one-way hashes, and the session ends after 30 minutes of inactivity.|FR-01, NFR-01, NFR-02, NFR-07| Priority: High| The system stores students’ personal data, applications, logbooks and evaluations. A user acting outside their role (for example, a student approving their own logbook) would break the internship process and expose private data.



DG-02: Maintainability| The system is divided into components with clear responsibilities and well-defined interfaces, so that a change in one function (for example, logbook management) does not require changes in unrelated components.| NFR-13| Priority: High| Independent components can also be implemented by team members working in parallel.



DG-03: Reliability| Saved records must remain available and consistent: placements, supervisor assignments, logbooks and feedback cannot refer to students or internships that do not exist, incomplete forms are never saved, and data is backed up every 24 hours.| NFR-03, NFR-04, NFR-06, NFR-10| Priority: High| Applications, logbooks and evaluations are official academic records. Losing or corrupting them would affect students’ internship results.



DG-04: Performance| The system must remain responsive with 1,000 registered users and 100 users at the same time, and show confirmation or error feedback within 2 seconds after a submission.| NFR-05, NFR-09, NFR-15| Priority: Medium| Many students submit logbooks near the same deadlines.

