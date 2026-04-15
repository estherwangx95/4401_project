<div style="page-break-after: always;"></div>

## 4.4 Elicitation Interview 

### a) Supplemental Interview Questions  

In this interview, the term *researcher* is narrowed to specifically refer to **PhD students acting as principal researchers**.  

The project brief identifies researchers broadly (honours, master’s, PhD students, and academic staff), but requires each research activity to have a **principal investigator** responsible for the application and compliance process.  

These questions focus on the needs of PhD students fulfilling this role.


#### 1. Draft Saving and Auto-Save

**Question:**  
Would you like the system to allow you to save an ethics application as a draft and return to complete it later? Would you also expect an auto-save feature while working on long applications?

**Justification:**  
Ethics applications are time-consuming and may not be completed in one session. This question helps determine whether draft saving and auto-save features are needed to improve usability and prevent data loss.


#### 2. Managing Multiple Applications

**Question:**  
If you need to manage an initial ethics application together with later amendments or extensions, what difficulties would you face? Would a dashboard showing status, deadlines, and required actions be helpful?

**Justification:**  
A principal researcher may manage multiple related activities or applications. The current process lacks clear tracking support. This question helps identify the need for dashboards, filtering, and status tracking.


#### 3. Clarity of Application Requirements

**Question:**  
Do you find the current application requirements clear, or do you often feel uncertain about what information is required? Would guidance such as templates, examples, or instructions be helpful?

**Justification:**  
Applicants may be unsure about required information. This question evaluates whether additional guidance (templates, examples, instructions) is needed to improve clarity and reduce errors.


#### 4. Validation Before Submission

**Question:**  
Would you prefer the system to automatically check for missing or incomplete sections before allowing submission?

**Justification:**  
Incomplete applications can delay review. This question determines whether built-in validation is required to improve submission quality.


#### 5. Communication Channels

**Question:**  
For communication related to an ethics application (e.g., clarification requests, revision feedback, decisions), would you expect interactions to occur within REMS, or through external tools such as email or Microsoft Teams?

**Justification:**  
Current communication occurs via email or informal channels. This question clarifies whether REMS should include internal communication or rely on external tools, helping define system scope and traceability.


#### 6. Notifications and Progress Updates

**Question:**  
How would you prefer to receive updates on the progress of your application: email notifications, a status dashboard, or both? Would reminder notifications for deadlines or revision requests be useful?

**Justification:**  
Delays and lack of transparency are key issues. This question identifies preferred methods for progress tracking and deadline awareness.


#### 7. Team Permissions and Collaboration

**Question:**  
If your research involves a supervisor or team members, should they be able to view the application, upload documents, or edit sections? What level of access control would you expect?

**Justification:**  
Ethics applications are collaborative, but access rights are unclear. This question helps determine the need for role-based permissions and collaboration features.


#### 8. Version Comparison and Revision Tracking

**Question:**  
When revisions are requested, would you find it useful to compare previous and revised versions side by side? Would you like changes to be highlighted?

**Justification:**  
Revision processes can be unclear. This question evaluates the need for version comparison and change tracking to support clarity during reviews.

### c) Interview Report

#### Meeting Details

- **Date:** 08 April, 2026
- **Time:** 17:00
- **Venue:** Building 225 (GEOGRAPHY AND GEOLOGY), G09 Seminar Room, UWA Campus 
- **Duration:** 20 Minutes


#### Attendance

##### Interviewers (Group 20 Members)
- Xing Wang (23932778)  
- Md Faraz Kabir Khan (24427672)  
- Bisha Babu (24741489)  
- Peiyu Yu (23901307)  
- Robin Varughese Mathew (24702715)  

##### Interviewee
- **Name:** Karla Ivkovic  
- **Role:** PhD Student acting as Principal Researcher  
- **Stakeholder Category:** Researcher (Principal Investigator)  


#### Summary of the Interview

This interview was conducted as part of the requirements elicitation phase for the REMS project. The interviewee represents a PhD student acting as a principal researcher, a key stakeholder involved in the ethics application and compliance lifecycle.

The interviewee provided clear direction on system usability and collaboration. She strongly supported features like auto-saving, draft management, and a centralized tracking dashboard. To minimize confusion during application building, she requested concrete examples over just standard instructions. The interviewee prefers communication and notifications to be handled through a dual approach using both the REMS platform and standard email. Notably, she prefer a flat access structure for research teammates rather than restrictive role-based permissions, and she prioritized simple access to historical file versions over complex, side-by-side text comparison tools.


####  Responses, Insights, and Requirements Refinements

##### Q1: Draft Saving and Auto-Save

**Response Summary:**  
Both draft saving and auto-save were strongly expected. The interviewee emphasized the importance of preserving progress due to the length and complexity of applications.

**Key Insights:**
- Draft saving is a baseline usability requirement  
- Auto-save is critical to prevent data loss  
- Applications are completed over multiple sessions  

**Requirements Refinements:**
- The system must allow saving applications as drafts at any time  
- The system must implement periodic auto-save without user action   


##### Q2: Managing Multiple Applications

**Response Summary:**  
A dashboard is necessary to manage multiple applications, including amendments and extensions.

**Key Insights:**
- Users often handle multiple applications or stages simultaneously  
- Lack of a centralized view creates confusion and inefficiency  
- Dashboard is a core system component, not optional  

**Requirements Refinements:**
- Provide a dashboard listing all applications (active, pending, historical)  
- Display status, deadlines, required actions, and application type  
- Support filtering and sorting (e.g., by status, date, type)  


##### Q3: Clarity of Application Requirements

**Response Summary:**  
Current requirements are often unclear. Worked examples are particularly helpful.

**Key Insights:**
- Ambiguity is a real usability barrier  
- Generic instructions are insufficient  
- Contextual examples significantly improve understanding  

**Requirements Refinements:**
- Provide contextual guidance for each section/question  
- Include worked examples based on realistic scenarios  
- Deliver guidance inline (e.g., tooltips or expandable help panels)  


##### Q4: Validation Before Submission

**Response Summary:**  
Basic validation is sufficient; complex validation is not mandatory.

**Key Insights:**
- Focus should be on completeness, not content correctness  
- Overly complex validation may hinder usability  

**Requirements Refinements:**
- Validate completion of mandatory fields before submission  
- Provide clear, field-level error messages  
- Allow users to review a summary before final submission  


##### Q5: Communication Channels

**Response Summary:**  
Both in-system communication and email notifications are expected.

**Key Insights:**
- A hybrid communication model is preferred  
- Email should complement, not replace system messaging  
- Communication traceability is important  

**Requirements Refinements:**
- Enable in-system messaging for feedback and decisions  
- Send email notifications for key events (e.g., updates, decisions)  
- Maintain communication history linked to applications  


##### Q6: Notifications and Progress Updates

**Response Summary:**  
The interviewee prefers both dashboard tracking and email notifications, including reminders.

**Key Insights:**
- Users rely on both passive (email) and active (dashboard) updates  

**Requirements Refinements:**
- Send email notifications for status changes  
- Provide real-time updates via dashboard  

##### Q7: Team Permissions and Collaboration

**Response Summary:**  
Team members should have equal access to applications.

**Key Insights:**
- Simplicity is preferred over granular role-based access  
- Flat access model reduces administrative overhead  
- Separation from external reviewers is still necessary  

**Requirements Refinements:**
- Allow principal investigators to add team members  
- Provide equal view/edit access to all team members  
- Restrict submission authority to the principal investigator  
- Maintain distinct access control for external users (e.g., reviewers)  


##### Q8: Version Comparison and Revision Tracking

**Response Summary:**  
Version comparison is not needed, but version history is important.

**Key Insights:**
- Users value access to previous versions  
- Side-by-side comparison may add unnecessary complexity  

**Requirements Refinements:**
- Maintain version history for all applications  
- Allow users to view previous versions at any time  
- Deprioritize comparison/diff features  


####  Summary of Requirements Refinements

| Q# | Topic                  | Key Refinement |
|----|------------------------|----------------|
| 1  | Draft & Auto-Save      | Both required; auto-save is essential |
| 2  | Application Dashboard  | Core feature for managing applications |
| 3  | Application Guidance   | Examples required; inline support |
| 4  | Validation             | Focus on completeness only |
| 5  | Communication          | Hybrid model: system + email |
| 6  | Notifications          | Dashboard + email + reminders |
| 7  | Collaboration          | Flat shared-access model |
| 8  | Version History        | History required; comparison not needed |

