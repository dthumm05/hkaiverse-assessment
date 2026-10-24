# Capstone Lab: Assignment Submission and Review Management System

## 1. Project Overview

**Project type:** Proposed software engineering capstone lab  
**Working title:** Assignment Submission and Review Management System  
**Primary workflow:** Assignment announcement → submission → review → marks and feedback release  
**Target users:** Students, faculty members, evaluators, and authorised support personnel  
**Proposed implementation:** A small web application with a database and role-based access control  
**Data policy:** Synthetic student, course, assignment, and marks data only

This capstone lab translates the workflow analysis from Task 1 into a practical software project. The aim is to develop a prototype that organises assignment information, records submission status, supports assessment review, and makes released marks and feedback easier to track.

The project is based on a preliminary student-perspective analysis. It does not claim that faculty members have confirmed the proposed workflow or that the institution has approved a new system.

## 1.1 Traceability to Task 1

This capstone is derived from the workflow analysis conducted in Task 1. The Task 1 report identifies the problem from the student perspective, while the process map documents the preliminary current-state workflow and the proposed improved workflow. This lab translates those findings into implementable requirements and test cases.

The connection between the analysis and the proposed implementation is summarised below.

| Task 1 finding or design principle | Proposed capstone feature | Related test |
| Assignment information may be spread across multiple channels | Course-wise assignment dashboard with instructions, deadlines, and submission methods | T01 |
| Students need confirmation that work was received | Submission timestamp and receipt after a successful save | T03 |
| Submission methods differ across courses | Configurable submission method and explicit handling of paper or external submissions | T04 and T12, where applicable |
| Students need to distinguish submission and assessment progress | Separate submission, grading, and release statuses | T10 and T11|
| Faculty may need a course-wise overview of pending work | Filterable faculty dashboard | T01 and relevant workflow tests |
| Duplicate submissions and incomplete information can cause errors | Input validation and submission-history handling | T02, T05, and T06 |
| Marks must be visible only to authorised users | Backend role-based access controls | T07 and T08 |
| Technical failures should not produce false confirmation | Error handling and a clear recovery path | T12 |

The tests listed above are planned test cases, not evidence of successful execution. Actual outcomes will be recorded after the prototype is implemented and tested.

**Source documents:**

- Task 1 report: `report.md`
- Task 1 process maps: `process-map.md`
- Task 2 curriculum proposal: `curriculum-redesign.md`

The report and process map provide the problem context and proposed workflow. The curriculum redesign explains why this project is proposed as an applied learning activity. The capstone lab specifies the suggested implementation, acceptance criteria, and testing approach.

The student-facing observations in Task 1 are preliminary. Faculty-side responsibilities and workflow assumptions have not been confirmed unless subsequent evidence is added to the repository.

## 2. Problem Statement

Assignment instructions and submission methods may be distributed across different channels, including email, SIS announcements, WhatsApp groups, paper submissions, Google Forms or Drive, and external learning platforms.

When information is spread across these channels, students may find it difficult to confirm the correct instructions, deadline, submission method, or current status of their work. They may also need to follow up to find out whether marks or feedback have been released.

A corresponding faculty-side problem may be the effort needed to identify submissions that require review, work with no submission recorded, late submissions, and marks awaiting release. This part of the problem is a hypothesis that requires validation with faculty or another relevant process owner.

The proposed system aims to provide a consistent view of assignment and assessment status without taking academic decisions away from authorised faculty members.

## 3. Objectives

The project aims to:

1. Organise assignment details by branch, year, section, course, and assessment.
2. Display assignment instructions, deadlines, and submission methods clearly.
3. Record submissions and provide a receipt only after a successful save.
4. Distinguish late submissions from submissions recorded before the deadline.
5. Track review, grading, and feedback-release status separately.
6. Give authorised faculty a view of records requiring attention.
7. Restrict students to their own submissions and released results.
8. Validate input and handle duplicate submissions and technical failures.
9. Maintain a history of important submission and assessment actions.
10. Evaluate the prototype through documented tests and identify limitations before recommending wider use.

## 4. Proposed Users and Permissions

| User role | Permitted actions|
| Student | View relevant assignments, submit work, view their own submission history, and view their own released marks and feedback |
| Faculty member | Create and publish assignments for assigned courses or sections; view relevant submissions and statuses |
| Assigned evaluator | Review permitted submissions, enter marks and feedback, and record assessment status |
| Authorised release role | Approve the release of marks and feedback according to the configured policy |
| Technical support | Investigate technical issues without automatically receiving access to confidential marks |

These roles are proposed for the prototype. Actual institutional responsibilities, approval rules, and separation of duties would need confirmation before implementation.

## 5. Functional Requirements

### 5.1 Assignment management

An authorised faculty member should be able to:

- Create an assignment with a title, instructions, course, section, deadline, and submission method.
- Save an incomplete assignment as a draft.
- Publish an assignment only when its required fields are complete.
- View published assignments and their current status.
- Close an assignment according to its configured submission policy.
- Archive an assignment without removing its historical assessment records.

**Assignment statuses:**

- Draft
- Published
- Closed
- Archived

### 5.2 Student assignment dashboard

The student dashboard should display:

- Course and assignment name
- Instructions and deadline
- Accepted submission method
- Submission status
- Submission timestamp, where applicable
- Review or grading status
- Marks and feedback, only when released

The interface should clearly distinguish an assignment with no submission recorded from one that has been submitted.

A missing system record must not automatically be treated as proof that a student did not submit through paper or another external route.

### 5.3 Submission handling

The prototype should allow students to submit a file or a permitted submission record, depending on the implementation selected.

The system should:

- Validate required fields and file type or size, where file upload is implemented.
- Record the submission timestamp.
- Compare the timestamp with the configured deadline.
- Show a success message and receipt only after the submission has been saved successfully.
- Prevent silent overwriting of an earlier submission.
- Retain submission history when resubmission is permitted.
- Explain errors clearly when a submission fails.

Late submission and resubmission rules must be configurable rather than assumed to be the same for every course.

### 5.4 Faculty dashboard

The faculty dashboard should allow authorised faculty to filter records by branch, year, section, course, and assignment.

It should provide a summary of:

- Submissions recorded
- Late submissions
- Records with no submission recorded
- Submissions under review
- Work returned for correction
- Work graded but not yet released
- Marks and feedback released

The dashboard should help users identify work requiring attention without automatically changing grades, deadlines, or academic decisions.

### 5.5 Marks and feedback

The prototype should support the following sequence:

1. An authorised evaluator opens a permitted submission.
2. The evaluator records marks and feedback.
3. The system validates the entered marks against the assessment's maximum marks.
4. The assessment is marked as graded.
5. An authorised role releases the marks and feedback.
6. The student can view the result only after release.

The system must distinguish **Graded** from **Released**. Entered marks must not automatically become visible to students if a separate release step is required.

### 5.6 Access control and audit history

The prototype should enforce permissions on the backend, not merely hide buttons in the user interface.

It should prevent a student from accessing another student's submission, marks, or feedback. It should also prevent users from performing faculty-only actions without the required permission.

Where practical, the system should record important events such as assignment publication, submission, resubmission, marks entry, and marks release.

Audit records should contain only the information needed to understand the action and should not expose confidential data unnecessarily.

## 6. Non-Functional Requirements

The prototype should aim to meet the following requirements:

- **Usability:** Use clear labels, readable statuses, and understandable error messages.
- **Reliability:** Confirm success only after the operation has completed successfully.
- **Security:** Enforce role-based permissions and protect confidential assessment data.
- **Data integrity:** Validate input and avoid silent replacement of previous submissions.
- **Maintainability:** Use a clear project structure and document important design decisions.
- **Testability:** Keep the workflow small enough for repeatable tests.
- **Transparency:** Display when marks are released and identify records that require manual confirmation.

These are proposed requirements; compliance must be demonstrated through implementation and testing rather than claimed in advance.

## 7. Proposed Workflow

### 7.1 Assignment publication

Faculty creates an assignment → system validates required fields → faculty publishes the assignment → eligible students can view the instructions and deadline.

If required fields are missing, publication is blocked and the system identifies what needs correction.

### 7.2 Student submission

Student opens an assignment → checks the instructions and deadline → submits the required work → system validates the submission → system saves the record → system displays a receipt and status.

If saving fails, the system displays an error and does not falsely confirm that the submission was received.

### 7.3 Review and grading

Evaluator opens a permitted submission → reviews the work → records marks and feedback → system validates the values → submission is marked as graded.

### 7.4 Release of marks and feedback

An authorised release role confirms that results can be published → system marks the result as released → the student can view their own marks and feedback.

### 7.5 Paper and external submissions

The prototype does not assume automatic integration with the institution's SIS, Google Drive, WhatsApp, or external learning platforms.

If paper or external submission routes are included in the demonstration, the system should identify them explicitly. A designated authorised person may record confirmation only after checking the relevant source or process. The prototype must not imply that an external submission was independently verified when it was not.

## 8. Suggested Technical Design

The prototype can be implemented using a simple web application architecture.

**Suggested components:**

- Frontend: HTML, CSS, and JavaScript, or another suitable interface framework.
- Backend: Flask or another framework approved for the lab.
- Database: SQLite for a small prototype.
- Version control: Git and a GitHub repository.
- Testing: Unit tests for validation and permissions, plus documented workflow tests.

**Prerequisites and course dependencies:** The proposed technology stack is a recommendation for the lab, not an official prerequisite list. Students may benefit from prior exposure to programming, databases, and web development, but the required background and any formal course prerequisites should be confirmed with the instructor and official curriculum.

These are suggested technologies, not mandatory institutional requirements. The team should choose a stack that can be implemented, explained, and tested within the available time.

### 8.1 Suggested data entities

| Entity      | Example fields                                                                               |
| ----------- | -------------------------------------------------------------------------------------------- |
| User        | User ID, synthetic name, role, branch, year, section                                         |
| Course      | Course ID, course title, branch                                                              |
| Assignment  | Assignment ID, course ID, title, instructions, deadline, submission method, status           |
| Submission  | Submission ID, assignment ID, student ID, timestamp, status, version reference               |
| Assessment  | Assessment ID, submission ID, marks, maximum marks, feedback, grading status, release status |
| Audit event | Event ID, actor ID, action, record reference, timestamp                                      |

The final database design may differ. The relationships, constraints, and access rules should be documented before implementation.

Synthetic identifiers and fictional names should be used. Real student names, registration numbers, marks, credentials, or private submissions must not be placed in the demonstration dataset.

## 9. Test Plan

The following are **planned tests**. They must be marked as not run until the team actually executes them and records the results.

| Test ID | Scenario | Expected result | Evidence to record|
| T01 | Faculty publishes an assignment with all required fields | Assignment is saved and visible to the intended students | Screenshot or test output showing publication |
| T02 | Faculty attempts to publish an assignment with a missing required field | Publication is blocked and the missing field is identified | Validation message and test result |
| T03 | Student submits a valid file or permitted submission record | Submission is saved with a timestamp and receipt | Submission record and receipt |
| T04 | Student submits after the configured deadline | System applies the configured late policy and displays the correct status | Deadline, timestamp, and resulting status |
| T05 | Student attempts to submit an invalid or missing file | Submission is rejected with a clear explanation | Error message and unchanged submission record |
| T06 | Student submits twice | System follows the resubmission policy and retains the required history | Submission history and resulting status |
| T07 | Student attempts to access another student's marks | Access is denied and confidential data is not returned | Test output demonstrating denial |
| T08 | Student attempts a faculty-only action | Backend rejects the unauthorised action | Response or automated test output |
| T09 | Evaluator enters marks above the maximum allowed | Invalid marks are rejected | Validation output |
| T10 | Marks have been entered but not released | Student cannot see the marks yet | Evaluator view and student view |
| T11 | An authorised user releases marks and feedback | The relevant student can view their own released result | Release record and student view |
| T12 | Database or storage operation fails during submission | System does not show a false success message and provides an understandable recovery path | Error log or simulated failure test |

### 9.1 Recording test outcomes

For each executed test, record:

- Test ID and date
- Environment and version tested
- Input or action performed
- Expected result
- Actual result
- Pass, fail, or blocked status
- Evidence location
- Defect or corrective action, if needed

A test should be marked **Pass** only when the observed result matches the expected result. If it has not been executed, retain the status **Not run**. If the required environment or dependency is unavailable, mark it **Blocked** and explain why.

## 10. Evaluation Criteria

The project can be evaluated using the following proposed rubric.

| Assessment area                                           |   Weight |
| --------------------------------------------------------- | -------: |
| Requirements and workflow design                          |      15% |
| Functional implementation                                 |      25% |
| Database design and data integrity                        |      15% |
| Security and access control                               |      15% |
| Testing, error handling, and recovery                     |      15% |
| Documentation, demonstration, and individual contribution |      15% |
| **Total**                                                 | **100%** |

The rubric is a suggested lab assessment framework, not an official institutional grading scheme. It should be reviewed by the relevant instructor before being used for formal assessment.

## 11. Deliverables

The student or project team should submit:

1. A requirements document describing users, permissions, and expected behaviour.
2. A workflow diagram covering assignment publication, submission, review, and release.
3. A documented database design.
4. Source code for the prototype.
5. A README with setup instructions, technology choices, limitations, and test instructions.
6. A synthetic demonstration dataset.
7. A test plan with expected outcomes and actual results for tests that were run.
8. Evidence of successful and unsuccessful test cases.
9. A short demonstration showing the main student and faculty workflows.
10. An individual contribution statement for each team member, if the project is completed in a team.

The deliverables should make it possible for another student or instructor to understand the design, reproduce the demonstration, and distinguish implemented features from proposed features.

## 12. Success Criteria

The prototype will be considered to have met its core objectives when the demonstrated implementation can:

- Publish an assignment only when required information is complete.
- Record a valid submission and confirm it only after a successful save.
- Show appropriate submission and assessment statuses.
- Preserve the distinction between grading and releasing results.
- Prevent unauthorised access to another student's marks.
- Handle the documented validation and failure cases appropriately.
- Provide enough documentation and test evidence for another person to reproduce the main workflow.

These are acceptance criteria, not claims of completed functionality. Final status should be based on the implementation and recorded test results.

## 13. Limitations and Risks

- The workflow is based on preliminary student-perspective evidence; faculty-side practices require validation.
- The prototype may not integrate with existing institutional systems.
- Paper and external submissions may require manual confirmation.
- The system introduces additional maintenance, support, and data-entry work.
- Access control and test coverage in a student prototype do not automatically establish production-level security.
- A working prototype does not establish that the institution needs or should adopt the system.
- Any real deployment would require institutional approval, privacy review, operational support, and alignment with applicable academic policies.

The prototype should therefore be treated as a learning and evaluation tool rather than a ready-to-deploy replacement for existing university systems.

## 14. Connection to Task 1 and Curriculum Learning Outcomes

This lab translates the Task 1 workflow analysis into an applied project.

It can provide opportunities to practise:

- Requirements gathering and process modelling.
- Programming and web application development.
- Database design and validation.
- Role-based access control.
- Error handling and debugging.
- Software testing and defect reporting.
- Technical documentation and teamwork.
- Evaluation of whether a proposed system solves the identified problem without creating unnecessary work.

These learning outcomes can connect existing programming, database, web technology, and software engineering courses. The suggested course links are provisional mappings based on course titles and the proposed project activities, not confirmed mappings to official course learning outcomes.

No formal prerequisite relationship between the courses is claimed. Any prerequisite requirements, course dependencies, and alignment with official learning outcomes must be verified against the curriculum applicable to the relevant admission batch before being treated as official.

## 15. Next Steps

Before treating the lab as a final curriculum proposal:

1. Confirm the intended lab duration and whether it is individual or team-based.
2. Review the official syllabi to identify which course learning outcomes it supports.
3. Obtain faculty or process-owner feedback if access is available.
4. Build a minimal prototype using synthetic data.
5. Execute the planned tests and document the actual results.
6. Review security, maintenance effort, and limitations.
7. Update this document to distinguish the implemented prototype from future recommendations.

## Conclusion

The Assignment Submission and Review Management System is a proposed capstone lab that applies software engineering concepts to the assignment lifecycle analysed in Task 1. Its value lies not only in building a dashboard, but also in modelling responsibilities, validating records, protecting assessment information, testing failure cases, and documenting limitations.

The project should be evaluated on evidence of implementation and testing, not on the proposed feature list alone. Any decision to adopt the workflow institutionally would require further validation and approval.
