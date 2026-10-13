**Core Processes Matrix**



P1 – 1.0 Authenticate Users



Input Data

\- Login credentials from Student, Internship Coordinator, Academic Supervisor, and Company Supervisor

\- Stored credentials and role data from D1 User Accounts



Output Data

\- Authentication result and role access

\- Credential lookup from D1 User Accounts



Rules

1\. Both username and password fields must be filled in. Otherwise, the login is rejected and the empty field is identified.

2\. The entered username is checked in D1 User Accounts. If no matching account exists, access is denied.

3\. The entered password is hashed and compared with the stored password hash. Passwords are never stored or displayed in plain text.

4\. If the credentials match, the user's role is identified and access is granted only to the functions allowed for that role.

5\. If the credentials do not match, an authentication failure message is returned.

6\. An authenticated session ends automatically after 30 minutes of inactivity and the user must log in again.







P2 – 2.0 Manage Internship Applications



Input Data

\- Internship application from Student

\- Required and additional documents from Student

\- Application review decision from Internship Coordinator

\- Stored applications and documents from D2 Internship Records



Output Data

\- Application status to Student

\- Submitted applications and documents to Internship Coordinator

\- Application records and documents stored in D2 Internship Records



Rules

1\. Only an authenticated student can submit an internship application.

2\. All required application fields must be complete and valid.

3\. Required internship documents must be uploaded before the application can be submitted.

4\. Additional documents are accepted only when requested or required for a specific application.

5\. When submitted, the application status is set to "Submitted".

6\. Only Internship Coordinators can review submitted applications and documents.

7\. The coordinator can update the application status to "Approved" or "Rejected".

8\. Students can view only their own application status.

9\. Only an approved application can proceed to placement.







P3 – 3.0 Manage Placements \& Progress



Input Data

\- Placement and supervisor assignment from Internship Coordinator

\- Student record filter criteria from Internship Coordinator

\- Stored placement data from D2 Internship Records

\- Stored progress data from D2 Internship Records



Output Data

\- Placement and internship information

\- Filtered student internship records

\- Placement status to Student

\- Internship progress to Student

\- Assigned student and internship details to Company Supervisor

\- Placement and progress records stored in D2 Internship Records



Rules

1\. A placement record can only be created for a student whose internship application is approved.

2\. A placement record must include company details, internship position, start date, and end date.

3\. The end date must be later than the start date.

4\. A placement is not complete until an Academic Supervisor and Company Supervisor are assigned.

5\. Only the Internship Coordinator can create or update placement records and supervisor assignments.

6\. Students can view only their own placement and supervisor information.

7\. Company Supervisors can view only students assigned to them.

8\. Internship progress shows completed internship weeks and the status of each weekly logbook.

9\. The coordinator can filter student records based on application or placement status.







P4 – 4.0 Manage Logbooks \& Notifications



Input Data

\- Weekly logbook from Student

\- Logbook review comments from Academic Supervisor

\- Approval or revision decision from Academic Supervisor

\- Stored logbooks and review status from D3 Logbooks \& Feedback



Output Data

\- Logbook review result and comments to Student

\- Notifications to Student

\- Submitted weekly logbooks to Academic Supervisor

\- Logbook status and progress to Academic Supervisor

\- Notifications and reminders to Academic Supervisor

\- Logbook records stored in D3 Logbooks \& Feedback



Rules

1\. Only a student with an active placement can submit weekly logbooks.

2\. Each logbook must correspond to one internship week within the placement dates.

3\. Only one logbook can normally be submitted for each internship week.

4\. A second submission is allowed when revision has been requested.

5\. A logbook with missing required fields is rejected without creating an incomplete record.

6\. When submitted, the logbook status is set to "Submitted".

7\. Academic Supervisors can view only the logbooks of students assigned to them.

8\. The supervisor may approve the logbook or request revision.

9\. A revision request must include comments explaining what the student should correct.

10\. Notifications are generated for missing logbooks, revision requests, and logbooks awaiting supervisor review.







P5 – 5.0 Manage Evaluation \& Feedback



Input Data

\- Student feedback

\- Student performance evaluation from Company Supervisor

\- Stored feedback data from D3 Logbooks \& Feedback



Output Data

\- Feedback submission confirmation to Student

\- Feedback submission confirmation to Company Supervisor

\- Feedback records stored in D3 Logbooks \& Feedback



Rules

1\. Feedback and evaluations can only be submitted after the internship is completed.

2\. A student can submit feedback only about their own internship experience.

3\. A Company Supervisor can evaluate only students assigned to them.

4\. Only one student feedback form and one company evaluation are recorded for each internship placement.

5\. All required fields must be complete and valid before submission.

6\. Each feedback record must be linked to an existing student and internship placement.

7\. Once saved, the feedback is kept for future reference.

