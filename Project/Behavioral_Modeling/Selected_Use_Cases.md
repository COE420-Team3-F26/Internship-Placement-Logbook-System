**Selected Use Cases**



UC-02|Submit Internship Application |PA: Student| Allows a student to complete an internship application, upload the required documents, and submit it so that the internship coordinator can review it.| It is the starting point of the internship workflow (FR-02, FR-13). It involves the Student, InternshipApplication and InternshipDocument classes, includes UC-13 (Upload Internship Documents), and has a repeated document upload and a completeness check, so it shows iteration and guards.



UC-07|Review and Approve Logbook |PA: Academic Supervisor| Allows the academic supervisor to review each submitted weekly logbook, add comments, and either approve it or request a revision.| It is the core of the weekly monitoring process (FR-04, FR-07, FR-08). It includes UC-04 (View Weekly Logbooks), is extended by UC-16 (Request Logbook Revision), has two different outcomes, and sends a notification to the student when a revision is requested.

