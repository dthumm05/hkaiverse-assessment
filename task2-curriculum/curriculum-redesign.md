# Curriculum Redesign Proposal

## 1. Purpose

The purpose of this proposal is to evaluate the available curriculum against selected software-related job descriptions and identify opportunities to improve practical skill development, industry readiness, and project-based learning.

The proposal uses the academic transcript available for Semesters I–VI and ST-II, a preliminary B.Tech CSE curriculum reference, and selected publicly available job descriptions. The recommendations focus on strengthening existing courses where appropriate, introducing practical learning activities where genuine gaps are identified, and developing an integrated project based on the workflow analysis conducted in Task 1.

This is a preliminary proposal. The complete official curriculum and detailed syllabi must be verified before finalising course-level changes.

## 2. Scope and Evidence

The available transcript contains 46 recorded course entries across Semesters I–VI and ST-II, accounting for 136 recorded credits. This is a partial transcript total and does not establish the complete credit requirement for the student's B.Tech CSE programme.

A semester-wise B.Tech CSE curriculum reference has also been provided for comparison. Its version and applicability to the student's 2023–2027 admission batch have not been confirmed. It is therefore treated as a reference rather than a verified statement of the student's complete degree requirements. Ambiguous course or credit details are flagged in `credit-map.csv` rather than inferred.

The preliminary job-description comparison uses three public postings:

- **Amazon:** Software Development Engineer Intern, May 2027, Bengaluru. This posting targets 2027 graduates.
- **Cisco:** Software Engineer, Bengaluru. The posting was reported as closed when checked on 24 October 2026.
- **Wipro:** Junior .NET Software Engineer Channels, Mumbai. The posting specifies 3–5 years of experience and is therefore used as a technical comparator, not as a fresher vacancy.

These postings provide examples of software-related skills and responsibilities. They are not a representative survey of the entire software industry, and their requirements should not be treated as universal hiring criteria.

The recommendations focus on technical themes such as programming, data structures and algorithms, application development, databases, testing, integration, and cloud technologies where supported by the selected postings.

The analysis does not assume that a course lacks a topic simply because its title does not explicitly mention it. Detailed syllabi, laboratory exercises, project work, and assessment methods must be reviewed before deciding whether a topic should be added or expanded.

## 3. Proposed Curriculum Changes

### 3.1 KEEP: Core Programming and Object-Oriented Programming

**Courses:** CS101 Computer Programming and CS201 Object Oriented Programming Concepts.

**Recommendation:** Retain the existing courses and strengthen the connection between their learning outcomes.

**Reasoning:** Programming and object-oriented design provide a foundation for developing, understanding, and maintaining software. Programming and application-development responsibilities in the selected job-description sample support the relevance of these foundational skills.

**Proposed improvement:** Where not already covered, include practical exercises involving functions, classes, error handling, modular code, and small programming tasks. Later courses should build on these skills rather than repeat introductory material without additional complexity.

### 3.2 KEEP: Data Structures and Algorithms

**Courses:** CS102 Data Structures and CS203 Design and Analysis of Algorithms.

**Recommendation:** Retain both courses while improving opportunities for implementation and problem-solving practice.

**Reasoning:** Data structures and algorithmic thinking are relevant to software development and technical assessments. The transcript records these courses, but the available information does not establish the exact depth of their practical coverage.

**Proposed improvement:** Where appropriate, include implementation exercises, complexity analysis, debugging, and timed problem-solving tasks. Assess both the correctness of a solution and the reasoning behind its time and space complexity.

### 3.3 KEEP: Database Management and Software Engineering

**Courses:** CS206 Database Management Systems and CS304 Software Engineering.

**Recommendation:** Retain both courses and strengthen their connection through practical software projects.

**Reasoning:** Software applications commonly require structured data storage, requirements analysis, implementation, testing, and maintenance. These courses can provide complementary knowledge for building reliable applications.

**Proposed improvement:** Where not already covered, connect database design and queries with requirements, testing, version control, documentation, and maintainable application code. The selected job descriptions do not, by themselves, establish that either course has a coverage gap.

### 3.4 UPDATE: Web Application Development

**Course:** CS205 Web-Enabled Technologies.

**Recommendation:** Review the syllabus and expand practical application-development exercises if gaps are identified.

**Proposed activities:** Build a small web application that includes input validation, communication between the user interface and backend, database interaction, useful error messages, and basic access control.

**Reasoning:** The selected developer postings provide examples of software-development and application-integration responsibilities. Practical exercises can help students understand how individual technologies work together in a complete application.

The proposed additions should be checked against the existing syllabus before being introduced. Specific frameworks should not be made compulsory solely on the basis of this small job-description sample.

### 3.5 UPDATE: Database Practice

**Course:** CS206 Database Management Systems.

**Recommendation:** Review the balance between theoretical concepts and applied database work.

**Proposed activities:** If these topics are not sufficiently covered, add exercises involving relational schema design, SQL queries, constraints, transactions, data validation, and access permissions.

**Reasoning:** Application development requires more than knowledge of database terminology. Students should be able to design, query, validate, and troubleshoot stored data.

These activities are proposed syllabus-review options, not evidence that the existing course lacks database practice.

### 3.6 UPDATE: Software Testing and Maintenance

**Course:** CS304 Software Engineering.

**Recommendation:** Strengthen practical testing and debugging activities where necessary.

**Proposed activities:** Include test-case design, defect reproduction, regression testing, debugging, code review, version control, and clear documentation of defects and fixes.

**Reasoning:** Reliable software requires systematic verification and maintenance. These activities also provide evidence of a student's ability to investigate problems rather than only produce a working demonstration.

### 3.7 UPDATE: Cloud and Network Integration

**Courses:** CS307 Cloud Computing and CS306 Computer Networks.

**Recommendation:** Review the practical components and introduce integrated exercises if the existing coverage is insufficient.

**Proposed activities:** A small application could communicate with a backend service, handle failed requests, validate responses, and demonstrate basic deployment or configuration troubleshooting.

**Reasoning:** The selected job-description sample includes software-development and integration-related responsibilities. Connecting networking and cloud concepts to an application may help students understand practical system behaviour.

The proposal does not assume that cloud deployment or service integration is absent from the current courses. This requires syllabus verification.

### 3.8 UPDATE: AI and Data Science Practical Work

**Courses:** DS101 Introduction to AI and DS, DS203 Data Science, DS304 Machine Learning, DS307 Big Data Systems, and DS201 Artificial Intelligence.

**Recommendation:** Review these courses collectively to identify unnecessary repetition and opportunities for progressive practical learning.

**Proposed activities:** Where relevant, emphasise data preparation, experiment design, model evaluation, reproducibility, interpretation of results, and documentation of limitations.

**Reasoning:** The available course list includes several AI- and data-related subjects. Reviewing their sequence could help ensure that students build on earlier knowledge and apply it to increasingly complex problems.

The selected software job descriptions do not establish that advanced AI or machine learning is required for every role. These recommendations are based primarily on the recorded course structure and the objective of improving practical learning.

The course-code and title association for DS201 must be verified against the official curriculum before any course-level change is finalised.

### 3.9 UPDATE: Internship and Special Project Assessment

**Courses:** IP201 Internship-I and SP301 Special Project.

**Recommendation:** Review how practical work and individual contributions are documented and assessed.

**Proposed evidence:** Students could submit a concise project report, contribution log, test evidence, technical documentation, and a demonstration of the work completed.

**Reasoning:** A project outcome alone may not show which parts each student completed or how problems were investigated. Clear assessment evidence can improve transparency and help students explain their work during interviews.

The assessment criteria should remain consistent with institutional rules and the official course requirements.

### 3.10 ADD: Short API Integration and Debugging Lab

**Proposal:** Introduce a short practical lab if equivalent learning outcomes are not already covered in existing courses.

**Content:** Students would connect a simple frontend to a backend API, validate input, handle unsuccessful responses, investigate communication failures, and record the steps used to diagnose a problem.

**Reasoning:** This lab would connect programming, web development, databases, and debugging in one manageable exercise.

**Implementation:** The lab could be delivered as a module within an existing course rather than as a new credit-bearing subject, subject to faculty approval.

### 3.11 ADD: Integrated Team Project Based on Task 1

**Proposal:** Develop an integrated project based on the assignment announcement, submission, review, and marks-release workflow analysed in Task 1.

**Suggested project title:** Assignment Submission and Review Management System.

**Core features:**

- Organise courses and assignments by branch, year, section, and course.
- Allow authorised faculty members to publish assignment instructions, deadlines, and submission methods.
- Record submission timestamps and provide a receipt only after a submission is successfully saved.
- Display clear submission statuses, such as submitted, submitted late, under review, graded, and feedback released.
- Provide faculty with a view of submissions and records for which no submission has been recorded.
- Support marks and feedback entry with appropriate access controls.
- Handle duplicate submissions, missing files, failed uploads, and storage errors.
- Maintain an audit trail for important actions.
- Use synthetic student and assignment data during development and testing.

**Reasoning:** This project would combine requirements analysis, programming, database design, interface development, testing, and documentation. It also builds directly on the process analysis completed in Task 1.

The system is a proposed prototype, not a claim that the institution currently needs or has approved a replacement for its existing processes. Any real deployment would require consultation with relevant faculty and institutional stakeholders.

**Detailed lab specification:** See `capstone-lab.md` for the proposed users, functional requirements, technical design, test plan, acceptance criteria, and deliverables for the Assignment Submission and Review Management System.

### 3.12 ADD: Professional and Collaborative Development Activities

**Proposal:** Review whether existing courses adequately assess technical documentation, presentation, teamwork, code review, and communication of technical decisions.

**Recommendation:** If gaps are identified, integrate these activities into existing labs, team projects, or project assessments rather than automatically adding a separate subject.

**Reasoning:** Technical work must often be explained, reviewed, tested, and maintained collaboratively. Integrating these activities into existing assessments could strengthen practical learning without unnecessarily increasing the credit load.

The transcript includes Professional Communication and Power Skills courses, but their exact assessed outcomes are not available in this analysis. Their syllabi should be reviewed before recommending additional activities.

## 4. REDUCE: Evidence Required Before Reducing Credits

No specific course is recommended for removal or credit reduction at this stage.

The available transcript and selected job descriptions do not provide sufficient evidence to conclude that a particular course is unnecessary or duplicates another course. A course should not be reduced merely because its relevance is not obvious from its title or because it is not mentioned in the selected job descriptions.

Before proposing a reduction, the complete official curriculum and syllabi should be compared to identify substantial duplication, overlapping learning outcomes, or content that could be integrated more effectively.

Any proposed reduction must also respect prerequisite relationships, programme requirements, applicable academic regulations, and the required total credits.

## 5. Provisional Credit Calculation

The available transcript records 136 credits across Semesters I–VI and ST-II. This is a partial transcript total and does not establish the total number of credits required to complete the B.Tech CSE programme.

A B.Tech CSE curriculum reference is available for comparison, but its applicability to the student's 2023–2027 admission batch has not been confirmed. Some semester and credit details in the supplied text are ambiguous, and the complete programme credit total remains unverified.

The 20–25% redesign target will be calculated only after the applicable official curriculum and its total credit requirement have been verified. The calculation will identify the specific courses or learning components affected and distinguish changes to course content from changes to credit allocation.

No final programme-wide redesign percentage is claimed in this version. The partial transcript total of 136 credits will not be used as the denominator for the final calculation, and credits will not be double-counted across overlapping changes.

Once the remaining semester details and the applicable official curriculum are obtained, the final proposal will identify the courses or learning components affected, their credit values, and whether each change involves retaining, updating, reducing, adding, or replacing curriculum content.

Where an update can be incorporated into an existing course without changing its credit value, it will be distinguished from a change that affects the number of credits in the curriculum. Adding a practical activity within an existing course does not automatically mean that additional programme credits are required.

## 6. Implementation Priorities

The proposed changes should be considered in the following order:

1. **Verify the official curriculum:** Confirm the admission-batch curriculum, full semester structure, course codes, titles, credit values, prerequisites, and relevant academic rules.
2. **Review current syllabi:** Determine which proposed practical activities are already covered and identify genuine gaps.
3. **Prioritise improvements within existing courses:** Update labs and assessments before introducing new credit-bearing courses where existing courses can accommodate the learning outcomes.
4. **Develop the integrated project:** Build a small prototype of the Assignment Submission and Review Management System using synthetic data.
5. **Test the project:** Document test cases, expected outcomes, actual outcomes, and unresolved defects. Do not report proposed tests as completed tests.
6. **Seek stakeholder feedback:** Where access is available, request voluntary feedback from faculty members or graduates. If access is unavailable, document this limitation rather than implying that consultation occurred.
7. **Finalise the credit calculation:** Calculate the redesign percentage using the verified full programme credit total and the clearly identified credits affected by the proposal.

## 7. Limitations

This proposal has several limitations:

- The available transcript records courses through Semesters I–VI and ST-II; it does not establish the complete degree-credit total.
- A B.Tech CSE curriculum reference is available, but its applicability to the student's 2023–2027 admission batch remains unconfirmed. Some semester and credit details in the supplied text are ambiguous.
- Course titles and transcript credit values do not establish the full syllabus or actual depth of practical coverage.
- The job-description comparison uses a small selection of public postings and is not representative of the entire software industry.
- The selected postings have different eligibility and experience requirements. The Amazon posting targets 2027 graduates, the Cisco posting was reported closed when checked on 24 October 2026, and the Wipro posting specifies 3–5 years of experience.
- Faculty-side workflow assumptions in the Task 1 analysis require confirmation from relevant process owners.
- The proposed project and curriculum changes have not been approved by the institution.
- The proposed activities and their feasibility remain subject to syllabus review, institutional requirements, faculty approval, and available resources.

These limitations will be revisited when further curriculum documents, syllabus details, and stakeholder feedback become available.

## 8. Conclusion

The preliminary proposal prioritises retaining foundational courses, strengthening practical work in programming and application development, improving integration and testing activities where genuine gaps exist, and using an integrated project to connect multiple learning outcomes.

No course is recommended for credit reduction without evidence of overlap or a verified curriculum review. The final redesign will be based on the applicable official curriculum, detailed syllabi, relevant academic requirements, and a recalculated 20–25% target using the verified programme-wide credit total.

The available curriculum reference and selected job descriptions provide a starting point for comparison, but further verification is required before the redesign can be treated as a complete degree-level proposal.
