# AI-Assisted Curriculum Exercises

**Assessment:** HKAIVERSE — Task 2  
**Date:** 24 October 2026  
**AI tool:** ChatGPT  
**Model label:** GPT-6  
**Verification status:** Pending for all five exercises

## 1. Purpose and methodology

These exercises document how AI can assist in generating practical curriculum-improvement ideas for five courses listed in my B.Tech CSE transcript.

The exercises focus on applied learning, assessment evidence, reproducibility, and practical problem-solving. They are intended to support curriculum review, not to establish that the existing curriculum is deficient.

The available transcript provides course titles and credits, but the complete official syllabus, laboratory manuals, and assessment methods for my admission batch have not yet been verified. Therefore, each exercise remains a **proposal pending human verification**.

The output summaries below are concise summaries of the AI-assisted suggestions, not claims that the proposed activities have been implemented or approved by the institution.

## 2. Exercise 1: CS102 — Data Structures

### Prompt used

> I am reviewing a B.Tech CSE curriculum. My transcript lists CS102 Data Structures as a 4-credit course, but I have not verified the complete official syllabus or lab manual for my admission batch. Suggest a practical exercise that tests students' ability to select data structures, explain their choices, and analyse performance. Do not claim that the current course is missing these topics.

### AI-generated output summary

Create a small campus assignment tracker. Students store assignments and their statuses, search by course or deadline, update submission statuses, explain their data-structure choices, analyse time complexity, and test normal and edge cases.

### Proposed learning outcome

Students should be able to select suitable data structures for a small application, justify their choices, and explain the performance implications of relevant operations.

### Suggested assessment evidence

- Working implementation of the assignment tracker.
- Explanation of the selected data structures.
- Time-complexity analysis of relevant operations.
- Test cases covering normal inputs and edge cases.

### Human verification

- **Official syllabus checked:** Pending.
- **Evidence and access date:** To be recorded after checking the official course documents.
- **What to verify:** Existing coverage of data-structure selection, searching, updating, complexity analysis, implementation, and testing.
- **Result:** Pending.
- **Proposed decision:** Use as an applied exercise if it complements existing practical work rather than duplicating it.

## 3. Exercise 2: CS206 — Database Management Systems

### Prompt used

> For a B.Tech CSE course listed as CS206 Database Management Systems (4 credits), propose a small database lab based on an assignment-submission system. Include entities, integrity rules, useful queries, and a way to test access boundaries. Do not assume any topic is absent from the current course.

### AI-generated output summary

Design a relational database for an assignment-submission system using entities such as Student, Course, Assignment, Submission, and Assessment.

Students define primary and foreign keys, apply suitable constraints, query submissions by assignment and status, handle duplicate or invalid records, explain transaction behaviour, and test whether users can access only the marks they are authorized to see.

The exercise should distinguish database integrity from application-level authorization: a well-designed schema alone does not guarantee secure access.

### Proposed learning outcome

Students should be able to design a relational schema, enforce data integrity, write useful queries, and explain how database controls differ from application-level access controls.

### Suggested assessment evidence

- Entity-relationship diagram and relational schema.
- SQL table definitions, constraints, and queries.
- Test cases for duplicate, invalid, and inconsistent records.
- A documented test of access boundaries and an explanation of the limitations of database-only controls.

### Human verification

- **Official syllabus checked:** Pending.
- **Evidence and access date:** To be recorded after checking the official course documents.
- **What to verify:** Existing coverage of relational modelling, SQL, constraints, transactions, and database/application security.
- **Result:** Pending.
- **Proposed decision:** Consider an applied integration lab if it adds useful practice beyond existing DBMS exercises.

## 4. Exercise 3: CS304 — Software Engineering

### Prompt used

> Suggest a small Software Engineering team project for a B.Tech CSE course listed as CS304 Software Engineering (3 credits). Use an assignment-submission and feedback workflow. Include requirements, defect handling, testing evidence, documentation, and individual contribution evidence. Do not claim that the current course lacks these activities.

### AI-generated output summary

Teams create a requirements and test package for an **Assignment Submission and Review Management System**.

Suggested deliverables include:

- User stories and acceptance criteria.
- A workflow diagram covering publishing, submission, review, grading, and feedback release.
- A prioritized defect log.
- Test cases with expected results and recorded outcomes.
- A code-review checklist.
- A README documenting setup, limitations, and individual contributions.

Students must distinguish planned tests from executed tests. A test should be marked passed or failed only after it has actually been run and its outcome recorded.

### Proposed learning outcome

Students should be able to translate requirements into testable acceptance criteria, document defects, plan and execute tests, and communicate their individual contributions to a team project.

### Suggested assessment evidence

- Requirements and workflow documentation.
- Defect log with severity, priority, and resolution status.
- Test cases with execution evidence.
- Code-review records where applicable.
- Setup instructions, limitations, and individual contribution statements.

### Human verification

- **Official syllabus checked:** Pending.
- **Evidence and access date:** To be recorded after checking the official course documents.
- **What to verify:** Existing coverage of requirements, design, testing, defect tracking, documentation, version control, and teamwork.
- **Result:** Pending.
- **Proposed decision:** Use as an integrated project if it fits the course learning outcomes and workload.

## 5. Exercise 4: DS304 — Machine Learning

### Prompt used

> Suggest a small, reproducible Machine Learning lab for a B.Tech CSE course listed as DS304 Machine Learning (4 credits). Focus on data splitting, baseline comparison, suitable evaluation metrics, and error analysis. Do not assume the official course omits these topics, and do not invent experimental results.

### AI-generated output summary

Students select a documented dataset, define a prediction task, establish a simple baseline, create a reproducible train/test split, train a model, and evaluate its performance.

They then inspect errors and explain limitations. Their report records the dataset source, preprocessing, split strategy, model settings, metric definitions, and random seed where applicable.

For imbalanced datasets, students explain whether precision, recall, F1-score, a confusion matrix, or other metrics provide more information than accuracy alone.

No numerical result should be reported until the experiment has actually been run.

### Proposed learning outcome

Students should be able to construct a reproducible ML experiment, compare a model against a baseline, select suitable evaluation metrics, and interpret errors and limitations.

### Suggested assessment evidence

- Dataset source and description.
- Documented preprocessing and train/test split.
- Baseline and model configuration.
- Actual metric results from a completed experiment.
- Error analysis and a discussion of limitations.

### Human verification

- **Official syllabus checked:** Pending.
- **Evidence and access date:** To be recorded after checking the official course documents.
- **What to verify:** Existing coverage of data preparation, evaluation, baselines, metrics, reproducibility, and error analysis.
- **Result:** Pending.
- **Proposed decision:** Strengthen this practical only if the verified syllabus and assessments show a relevant gap.

## 6. Exercise 5: CS307 — Cloud Computing

### Prompt used

> Suggest a small Cloud Computing lab for a B.Tech CSE course listed as CS307 Cloud Computing (4 credits). Cover deployment planning, configuration, logs, failure diagnosis, and safe handling of credentials. Assume I have not verified the official syllabus or available lab infrastructure. Do not require paid cloud resources or claim that a deployment has been performed.

### AI-generated output summary

Students deploy a small sample web application in an instructor-approved environment. A local container or sandbox may be used if cloud accounts or paid resources are unavailable.

Students document the architecture, deployment steps, configuration, health checks, logs, a controlled configuration failure, diagnostic steps, recovery, and cleanup.

They keep credentials out of source control and explain relevant security and cost considerations. The platform should be selected only after confirming the available infrastructure and course requirements.

### Proposed learning outcome

Students should be able to document a deployment, inspect logs, diagnose a controlled configuration failure, and explain basic credential-security and resource-cost considerations.

### Suggested assessment evidence

- Architecture and deployment notes.
- Configuration and health-check evidence.
- Logs and a description of the simulated failure.
- Recorded diagnostic and recovery steps.
- Evidence of safe credential handling and resource cleanup.

### Human verification

- **Official syllabus checked:** Pending.
- **Evidence and access date:** To be recorded after checking the official course documents.
- **What to verify:** Existing coverage of deployment, configuration, monitoring, logging, troubleshooting, security, and cost awareness.
- **Result:** Pending.
- **Proposed decision:** Consider this lab only if it is feasible with approved tools and complements existing practical work.

## 7. Cross-exercise reflection and curriculum implications

The five suggestions share a focus on practical evidence: working artefacts, design explanations, tests, reproducible experiments, troubleshooting, and documentation.

This is an AI-generated design pattern, not evidence that the current curriculum is deficient.

The proposed activities could support the following curriculum-review areas:

| Course                              | Proposed area for review                         | Potential contribution                                      |
| ----------------------------------- | ------------------------------------------------ | ----------------------------------------------------------- |
| CS102 — Data Structures             | Applied data-structure selection and analysis    | Justified implementation and complexity analysis            |
| CS206 — Database Management Systems | Integrated database design and integrity testing | Schema, SQL queries, constraints, and access-boundary tests |
| CS304 — Software Engineering        | Requirements, defect handling, and test evidence | A structured team-project evidence package                  |
| DS304 — Machine Learning            | Reproducible experimentation and error analysis  | Baseline comparison, metrics, and documented results        |
| CS307 — Cloud Computing             | Deployment and troubleshooting                   | Configuration, logs, recovery, and security evidence        |

CS102 and CS206 could contribute data-structure and database knowledge to the Assignment Submission and Review Management System proposed in Task 1. CS304 could contribute requirements, testing, and project documentation.

The Machine Learning and Cloud Computing exercises are separate examples and should not be forced into the capstone unless their learning outcomes justify that connection.

These proposals should be compared with the verified syllabus and existing assessments before deciding whether to keep, update, add, or remove any curriculum activity.

## 8. Human verification checklist

- [ ] Locate the official syllabus for the correct programme, branch, admission batch, and curriculum version.
- [ ] Check relevant laboratory manuals and assessment methods.
- [ ] Record each source's title, exact URL, and access date.
- [ ] Compare each suggestion with existing learning outcomes and practical work.
- [ ] Record whether each element is already covered, partially covered, absent, or impossible to determine.
- [ ] Remove or revise suggestions that conflict with official requirements, prerequisites, workload, or available infrastructure.
- [ ] Update each verification result and proposed decision using the evidence.
- [ ] Keep AI suggestions separate from verified institutional facts and personal recommendations.
- [ ] Record actual implementation and test evidence only after the work has been completed.

## 9. Limitations

- The available transcript does not establish the complete official batch-specific syllabus.
- The exercise outputs are AI-generated suggestions and have not been independently validated against course documents.
- All five syllabus-verification results remain pending.
- No faculty member or graduate is represented as endorsing these suggestions.
- No implementation, experiment, or test result is claimed.
- The Semester VI transcript mapping for DS201 Artificial Intelligence should be checked against the official transcript or curriculum before relying on it elsewhere.
- These exercises do not establish that a course is missing a topic or that a proposed change is required. Such conclusions depend on official syllabus and assessment evidence.
