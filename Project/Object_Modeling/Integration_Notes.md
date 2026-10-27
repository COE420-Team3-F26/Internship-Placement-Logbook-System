# Integration Notes

We combined our three individual UML class diagrams into one diagram for the Internship Placement and Weekly Logbook System. We compared the classes, their methods, and their relationships to avoid duplicates and connect the different parts of the system.

Miriam's part included User, Student, InternshipCoordinator, InternshipApplication, and Feedback. In the combined diagram, we added placement-related methods to InternshipCoordinator and linked applications to internships.

Raghad's part included Supervisor, AcademicSupervisor, CompanySupervisor, WeeklyLogbook, and Notification. These were connected to internships, students, and the logbook review process.

Ahmad's part included InternshipPlacement, Company, InternshipDocument, and InternshipProgress. We renamed InternshipPlacement to Internship in the combined diagram and connected it to the application, company, supervisors, and logbooks.

All 14 classes from the individual inventories are included in the combined diagram. We kept shared classes in one place and retained the inheritance relationships for the user and supervisor roles.

We also added the main associations and multiplicities. For example, students submit applications, approved applications can lead to internships, and internships are linked to companies and weekly logbooks. Notes in the diagram explain additional conditions such as supervisor assignments and logbook revisions.
