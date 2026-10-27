# Class Model Consistency Check

We compared the combined class diagram with the requirements and use cases from Lab 3 and the Level-0 DFD from Lab 4.

## DFD Processes

1. P1 - Authenticate Users: User, Student, InternshipCoordinator, and Supervisor represent the user roles and login functionality.
2. P2 - Manage Internship Applications: Student, InternshipApplication, InternshipDocument, and InternshipCoordinator cover application submission, documents, and review.
3. P3 - Manage Placements & Progress: Internship, Company, InternshipProgress, AcademicSupervisor, and CompanySupervisor cover placement details, supervisor assignments, and progress.
4. P4 - Manage Logbooks & Notifications: WeeklyLogbook, Student, AcademicSupervisor, and Notification cover submissions, reviews, revisions, and reminders.
5. P5 - Manage Feedback: Feedback, Student, and CompanySupervisor cover feedback after the internship ends.

## Requirements and Relationships

- UC-02 and UC-03: Student, InternshipApplication, and InternshipCoordinator are linked, with methods for submitting and reviewing applications. This matches the use cases.
- UC-11: The diagram links InternshipApplication to Internship. A note states that a placement is created only after application approval.
- UC-10: AcademicSupervisor and CompanySupervisor are associated with Internship. A note explains that both must be assigned for the placement to be complete.
- UC-13 and UC-17: InternshipDocument is included, with a note explaining that documents may belong to an application or a placement.
- UC-06, UC-07, and UC-16: WeeklyLogbook and AcademicSupervisor include methods for submission, review, and requesting revisions. These match the logbook use cases.
- UC-14: InternshipProgress includes completed weeks and a method for viewing progress.
- UC-05 and UC-09: Feedback represents student feedback and company supervisor evaluations. The diagram includes a note about the two feedback types and their timing.

The main associations and multiplicities reflect the internship workflow. Some rules, such as requiring both supervisors and allowing one feedback record of each type, are described in notes because multiplicities alone do not express those conditions.
