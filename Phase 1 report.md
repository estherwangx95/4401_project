CITS3301/4401 Software Requirements & Design

Project Report (Phase 1)

Group Number: 20

Team Members:

Name	Student ID	GitHub Username
Peiyu Yu	23901307	YUPeiyu123
Xing Wang	23932778	estherwangx95
Md Faraz Kabir Khan	24427672	farazkabir
Robin Varughese Mathew	24702715	robin20516
Bisha Babu Babu	24741489	bishababu1506-ops
4. Phase 1 Tasks

4.1 Project Setup and Team Organisation

4.1.1 Team Communication & Responsibilities

Communication Methods

The team will primarily communicate through Microsoft Teams, using both video meetings and messaging features. Tasks will be allocated to team members during meetings and confirmed through text messages for clarity and follow-up.

Meeting Frequency & Format

Meetings will be held on an as-needed basis, depending on the progress of the project. The preferred format is online, although face-to-face meetings may be arranged when necessary. A summary of each meeting will be shared in the group chat for reference and continuity.

Accountability & Progress Tracking

The project will be hosted on GitHub, where progress will be tracked and managed. Clear deadlines will be established, ensuring that each member is accountable for completing their assigned work on time.

4.1.2 Version Control Strategy

Repository Hosting

The project will be hosted on GitHub, using a private repository to manage all files and documentation.

Branching Strategy

The team will adopt a feature-branch workflow:

main branch → Stable, final version
Feature branches → Created for each task (e.g., feature/4.6-use-case, feature/4.1-introduction)
Merging Process

All changes must be submitted via Pull Requests (PRs).
At least one peer review approval is required before merging.
Conflicts must be resolved collaboratively by the team member and reviewer.
Version Control Policies

Small, frequent commits are encouraged for traceability.
No direct commits to main branch are allowed.
All PRs must include a description of changes and testing notes.
4.1.3 Risk Management & Quality Assurance

Potential Risks & Mitigation

Member unavailability (illness or workload issues):
Tasks will be distributed with overlap where possible to ensure backup support.

Missed deadlines:
Weekly progress tracking and task breakdown into smaller milestones will help reduce delays.

Communication breakdown:
Regular meetings and centralized communication tools (MS Teams) will reduce miscommunication.

Service outage (GitHub or tools unavailable):
Local backups and periodic exports of critical documents will be maintained.

Quality Assurance Approach

All documents and deliverables will undergo peer review before submission.
A standard template format will be used for documentation to ensure consistency.
Feedback from reviews will be incorporated before final submission.
4.2 Version Control and Effort Tracking

The group uses a private version-controlled repository (e.g., GitHub) to manage all project work. All project documentation is maintained using Markdown (.md) files only, ensuring that content remains lightweight, readable, and easy to track through version control.

Using Markdown allows effective collaboration, as changes can be clearly reviewed and attributed to individual team members. It also supports proper change tracking, unlike binary formats such as .docx or .pdf.

Final reports are generated from Markdown files using Typora to produce the submitted PDF deliverable, ensuring consistency in formatting and structure.

The repository itself is not submitted for assessment but may be reviewed upon request to verify contributions and development history.

4.3 Stakeholder Identification and User Stories

a) Stakeholders:

1. PhD Student Principal Researcher

A PhD student acting as a principal researcher is responsible for preparing and submitting ethics applications for their research projects. They must provide detailed research descriptions, supporting documents, and respond to feedback from reviewers. They benefit from the system through improved guidance, clear submission requirements, and transparency in tracking application status.

2. Administrative Staff

Administrative staff are responsible for managing incoming applications, checking completeness, and coordinating the review workflow. They also monitor application progress and maintain records. They benefit from reduced manual tracking (e.g., spreadsheets and emails), improved consistency, and better oversight of application status.

b) User Stories:

PhD Student (Principal Researcher)

As a PhD student (principal researcher), I want to submit an ethics application with all required documents in a single system, so that my research can be reviewed efficiently without missing information.
As a PhD student, I want to receive notifications and track the status of my application, so that I know when to respond to reviewer feedback or provide revisions.
As a PhD student, I want to revise and resubmit my application after receiving feedback, so that I can address reviewers’ concerns and obtain approval.
As a PhD student, I want to upload and manage different versions of supporting documents, so that changes over time are tracked and reviewers can access the correct version.
Administrative Staff

As an administrative staff member, I want to verify that an application is complete before assigning it for review, so that reviewers only receive valid submissions.
As an administrative staff member, I want to monitor the progress and status of all applications, so that I can ensure timely processing and identify delays.
As an administrative staff member, I want to assign applications to appropriate committee members, so that each application is reviewed by qualified reviewers.
As an administrative staff member, I want the system to maintain a record of all actions taken on applications, so that there is a clear audit trail for accountability and compliance.






4.6 Use Case Diagram

a) Use case diagram:
![Use Case Diagram](Usecase.jpg)

b) Use case description:

Goal: To allow a researcher acting as principal investigator to complete and submit a research ethics application to the REMS for administrative review and subsequent ethics committee evaluation.

Actors:
- Primary Actor: Researcher (PhD student as Principal Investigator)
- Secondary Actor: Admin Officer

Preconditions:
- The researcher is registered and has a valid account in REMS.
- The researcher has logged in successfully.
- The researcher has prepared the necessary information about their research activity, including a description of the methodology, participant details, and any associated risks.
- At least one supporting document (e.g. consent form, information sheet, or risk assessment) is ready for upload.

Postconditions:
- The ethics application is recorded in REMS with a unique application ID.
- The application status is set to "Submitted -Pending Administrative Review."
- The admin officer is notified of the new submission.
- An audit trail entry is created recording the submission timestamp and the identity of the submitting researcher.


Main Success Scenario

1. The researcher navigates to the REMS dashboard and selects "Create New Application."
2. The system displays an application form with sections for research description, methodology, participant information, risk assessment, and supporting documents.
3. The researcher fills in the research title and provides a description of the research activity and its objectives.
4. The researcher enters the methodology, including details of how participants will be recruited, what data will be collected, and how it will be stored.
5. The researcher identifies all team members involved in the research activity and assigns their roles within the application.
6. The researcher uploads all required supporting documents, including consent forms and participant information sheets. The system stores each document with a version number and upload timestamp.
7. The researcher reviews all sections of the application using the system's summary view.
8. The researcher clicks "Submit Application." The system performs an automatic completeness check, verifying that all mandatory fields are filled and at least one supporting document has been uploaded.
9. The system accepts the submission, assigns a unique application ID, and sets the application status to "Submitted - Pending Administrative Review."
10. The system sends an automated notification to the researcher confirming successful submission, and notifies the admin officer of the incoming application.


Alternate Flow 1 - Incomplete Application

At step 8, if the system's completeness check detects one or more mandatory fields that are empty or a required document that has not been uploaded:

1. The system does not submit the application.
2. The system highlights the incomplete sections and displays a summary of what is missing.
3. The researcher corrects the identified issues and returns to step 7.



Alternate Flow 2 - Researcher Saves as Draft

At any point between steps 3 and 7, the researcher may choose to save the application as a draft instead of submitting:

1. The researcher clicks "Save Draft."
2. The system saves all entered data and uploaded documents against the application, assigning it a draft status.
3. The system confirms the save with a timestamp.
4. The researcher may close the application and return to complete it in a later session. The use case resumes from step 2 when the researcher reopens the draft.



Alternate Flow 3 — Session Timeout During Completion

At any point between steps 3 and 8, if the researcher's session expires due to inactivity:

1. The system automatically saves any entered data as a draft before terminating the session.
2. The researcher is redirected to the login page with a message indicating their session has expired and their progress has been saved.
3. Upon logging back in, the researcher is presented with the option to resume the saved draft. The use case resumes from step 2.



Special Requirements (Non-Functional)

- All supporting documents must be stored with version control so that earlier versions remain accessible for audit purposes.
- The application and all associated documents must only be visible to the submitting researcher, their nominated team members, and authorised administrative staff.
- The completeness check at step 8 must complete within 3 seconds of the researcher clicking submit.
- The system must maintain a full audit trail of all actions taken on the application, including saves, edits, and the final submission.
