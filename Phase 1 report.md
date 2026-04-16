
# CITS3301/4401 Software Requirements & Design


##  Project Report (Phase 1) 
## Group Number: 20

## Team Members:

| Name | Student ID | GitHub Username |
|------|----------------|-----------------|
| Peiyu Yu | 23901307 | YUPeiyu123 |
| Xing Wang | 23932778 | estherwangx95 |
| Md Faraz Kabir Khan | 24427672 | farazkabir |
| Robin Varughese  Mathew | 24702715 | robin20516 |
| Bisha Babu Babu | 24741489 | bishababu1506-ops |


---



# 4. Phase 1 Tasks

## 4.1 Project Setup and Team Organisation
### 4.1.1 Team Communication & Responsibilities

#### Communication Methods
The team will primarily communicate through Microsoft Teams, using both video meetings and messaging features. Tasks will be allocated to team members during meetings and confirmed through text messages for clarity and follow-up. 

#### Meeting Frequency & Format
Meetings will be held on an as-needed basis, depending on the progress of the project. The preferred format is online, although face-to-face meetings may be arranged when necessary. A summary of each meeting will be shared in the group chat for reference and continuity.

#### Accountability & Progress Tracking
The project will be hosted on **GitHub**, where progress will be tracked and managed. Clear deadlines will be established, ensuring that each member is accountable for completing their assigned work on time.


### 4.1.2 Version Control Strategy

#### Repository Hosting
The project will be hosted on **GitHub**, using a private repository to manage all files and documentation.

#### Branching Strategy
The team will adopt a **feature-branch workflow**:
- `main` branch → Stable, final version
- Feature branches → Created for each task (e.g., `feature/4.6-use-case`, `feature/4.1-introduction`)

#### Merging Process
- All changes must be submitted via **Pull Requests (PRs)**.
- At least one peer review approval  is required before merging.
- Conflicts must be resolved collaboratively by the team member and reviewer.

#### Version Control Policies
- Small, frequent commits are encouraged for traceability.
- No direct commits to `main` branch are allowed.
- All PRs must include a description of changes and testing notes.


### 4.1.3 Risk Management & Quality Assurance

#### Potential Risks & Mitigation

- **Member unavailability (illness or workload issues):**  
  Tasks will be distributed with overlap where possible to ensure backup support.

- **Missed deadlines:**  
  Weekly progress tracking and task breakdown into smaller milestones will help reduce delays.

- **Communication breakdown:**  
  Regular meetings and centralized communication tools (MS Teams) will reduce miscommunication.

- **Service outage (GitHub or tools unavailable):**  
  Local backups and periodic exports of critical documents will be maintained.


#### Quality Assurance Approach

- All documents and deliverables will undergo peer review before submission.
- A standard template format will be used for documentation to ensure consistency.
- Feedback from reviews will be incorporated before final submission.

<div style="page-break-after: always; break-after: page;"></div>

## 4.2 Version Control and Effort Tracking

The group uses a private version-controlled repository (e.g., GitHub) to manage all project work. All project documentation is maintained using **Markdown (.md) files only**, ensuring that content remains lightweight, readable, and easy to track through version control.

Using Markdown allows effective collaboration, as changes can be clearly reviewed and attributed to individual team members. It also supports proper change tracking, unlike binary formats such as `.docx` or `.pdf`.

Final reports are generated from Markdown files using `Typora` to produce the submitted PDF deliverable, ensuring consistency in formatting and structure.

The repository itself is not submitted for assessment but may be reviewed upon request to verify contributions and development history.



<div style="page-break-after: always; break-after: page;"></div>

## 4.3 Stakeholder Identification and User Stories 
### a) Stakeholders:
#### 1. PhD Student Principal Researcher

A PhD student acting as a principal researcher is responsible for preparing and submitting ethics applications for their research projects. They must provide detailed research descriptions, supporting documents, and respond to feedback from reviewers.
They benefit from the system through improved guidance, clear submission requirements, and transparency in tracking application status.

#### 2. Administrative Staff

Administrative staff are responsible for managing incoming applications, checking completeness, and coordinating the review workflow. They also monitor application progress and maintain records.
They benefit from reduced manual tracking (e.g., spreadsheets and emails), improved consistency, and better oversight of application status.

### b) User Stories:
#### PhD Student (Principal Researcher)

1.	As a PhD student (principal researcher), I want to submit an ethics application with all required documents in a single system, so that my research can be reviewed efficiently without missing information.
2.	As a PhD student, I want to receive notifications and track the status of my application, so that I know when to respond to reviewer feedback or provide revisions.
3.  As a PhD student, I want to revise and resubmit my application after receiving feedback, so that I can address reviewers’ concerns and obtain approval.
4.  As a PhD student, I want to upload and manage different versions of supporting documents, so that changes over time are tracked and reviewers can access the correct version.

#### Administrative Staff
5.	As an administrative staff member, I want to verify that an application is complete before assigning it for review, so that reviewers only receive valid submissions.
6.	As an administrative staff member, I want to monitor the progress and status of all applications, so that I can ensure timely processing and identify delays.
7.  As an administrative staff member, I want to assign applications to appropriate committee members, so that each application is reviewed by qualified reviewers.
8.  As an administrative staff member, I want the system to maintain a record of all actions taken on applications, so that there is a clear audit trail for accountability and compliance.



<div style="page-break-after: always; break-after: page;"></div>

## 4.5 Requirements Specification 

For this task, our group chose the subsystem ethics application creation, submission, revision, and tracking for a PhD student acting as the principal researcher. This is a suitable scope because it focuses on one clear part of REMS and matches our chosen stakeholder. This scope was further refined by the interview with our selected stakeholder, which highlighted the need for draft saving, auto-save, guidance examples, basic validation, dashboard and email updates, shared teammate access, and access to older file versions.

The following requirements are written to be clear, testable, consistently structured, and uniquely identified, and each is labelled as either functional or non-functional.


| ID | Type | Requirement |
|---|---|---|
| FR-01 | Functional | The system shall allow a principal researcher to create a new ethics application for a research activity involving human participants. |
| FR-02 | Functional | The system shall require the principal researcher to enter required information before submission, including the project title, research description, methodology, participant risks, and research team details. |
| FR-03 | Functional | The system shall allow the principal researcher to save an incomplete application as a draft and return to it later. |
| FR-04 | Functional | The system shall automatically save the application while the principal researcher is working on it. |
| FR-05 | Functional | The system shall allow the principal researcher to upload supporting documents as part of an ethics application. |
| FR-06 | Functional | The system shall provide examples or guidance to help the principal researcher understand what information is needed in different parts of the application. |
| FR-07 | Functional | The system shall perform basic validation before submission and tell the principal researcher if required fields or sections are missing. |
| FR-08 | Functional | The system shall record the date and time when an application is submitted. |
| FR-09 | Functional | The system shall show the current status of each application to the principal researcher, including draft, submitted, under review, revision requested, approved, conditionally approved, and rejected. |
| FR-10 | Functional | The system shall provide a dashboard so the principal researcher can view multiple applications, amendments, or extensions and check their current status. |
| FR-11 | Functional | The system shall allow the principal researcher to view clarification requests, revision requests, and decisions inside REMS. |
| FR-12 | Functional | The system shall send email notifications to the principal researcher for important updates, including submission confirmation, revision requests, and final decisions. |
| FR-13 | Functional | The system shall allow the principal researcher to edit and resubmit an application when clarification or revision has been requested. |
| FR-14 | Functional | The system shall allow authorised research teammates to access the same application. |
| FR-15 | Functional | The system shall allow authorised research teammates to view, edit, and upload documents to the shared application with the same level of access. |
| FR-16 | Functional | The system shall store previous versions of application files and allow authorised users to open older versions of those files. |
| FR-17 | Functional | The system shall require user authentication before any application can be created, viewed, edited, or submitted. |
| NFR-01 | Non-functional | The system shall present forms, statuses, and guidance in a clear and consistent way so that the principal researcher can understand the process without needing help from administrative staff. |
| NFR-02 | Non-functional | The system shall protect confidentiality by making sure that only authenticated and authorised users can access application information and supporting documents. |
| NFR-03 | Non-functional | The system shall keep an audit trail of important actions, including draft creation, auto-save, submission, revision, resubmission, and status changes. |
| NFR-04 | Non-functional | The system shall support file versioning so that current and previous versions of documents can be clearly identified and accessed. |
| NFR-05 | Non-functional | The system shall send email notifications within a reasonable time after a status change, clarification request, or revision request is recorded in REMS. |


These requirements were based on the REMS scenario and the interview results. Together, they describe a clear subsystem that supports the principal researcher in creating, submitting, revising, and tracking ethics applications. They also include important system constraints such as authentication, confidentiality, versioning, and audit trails.
