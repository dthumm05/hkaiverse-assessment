# HKAIVERSE Assessment

## Project overview

This repository contains two assessment tasks:

- **Task 1 — Student assignment and assessment workflow:** documents the current student experience, separates observations from estimates, maps a proposed workflow, and defines synthetic tests and a transparent time-saving calculation.
- **Task 2 — Curriculum-to-career alignment:** compares selected curriculum examples with public software job listings and uses B.Sc/BCA programme structures for a focused comparison. The `credit-map.csv` file records transcript courses, credits, grades, and verification notes. It contains 136 recorded credits across Semesters I–VI and ST-II, but this is a partial transcript total, not the complete degree-credit requirement for the user's 2023–2027 batch.

## Personal contribution

I selected the Task 1 problem based on my own experience as a student: assignment announcements and submission instructions can appear in different places, and it can take follow-up to understand whether marks have been released and what they refer to. I organised these observations into an as-is workflow, identified points where students can get stuck, and designed a possible improvement with basic access controls and fallback handling.

The evidence in Task 1 is intentionally modest and is based primarily on my personal observations. It is not based on a formal student survey or faculty interview. Any time figures and scenario inputs are labelled as estimates or assumptions.

## Limitations

- This is a student-led process proposal, not an official ICFAI Tech system or policy statement.
- The current workflow has not been formally validated with faculty or administrative staff.
- The number and representativeness of students who shared feedback are not independently verified.
- Time-saving scenarios are illustrative and should not be treated as measured results.
- No live SIS, Google Drive, AWS Academy, or Springboard integration is claimed.
- The available public programme pages may not match the exact 2023–2027 batch curriculum. The curriculum reference, total graduation-credit requirement, course-code/title associations, and ambiguous semester details still require verification against official batch records.
- `credit-map.csv` contains 136 recorded credits across Semesters I–VI and ST-II. This is a partial transcript total, not the complete degree-credit requirement. Zero-credit courses are retained but excluded from the credit-bearing total. Job-description evidence is documented separately in `job-descriptions.md` and does not prove actual syllabus coverage.

## Repository structure

```text
HKAIVERSE-ASSESSMENT/
├── README.md
├── AI-USE.md
├── task1-workflow/
│   ├── calculations.md
│   ├── evidence-log.md
│   ├── process-map.md
│   ├── report.md
│   └── test-cases.md
└── task2-curriculum/
    ├── calculator/
    │   └── index.html
    ├── ai-exercises.md
    ├── capstone-lab.md
    ├── credit-map.csv
    ├── curriculum-redesign.md
    ├── feedback.md
    ├── job-descriptions.md
    ├── recommendations.md
    └── report.md
```

## Submission metadata

- **Release:** https://github.com/dthumm05/hkaiverse-assessment/releases/tag/v1.0
- **Full commit URL:** https://github.com/dthumm05/hkaiverse-assessment/commit/ba1881ded9ad245e5cd01623599bbe5eb452d2bb
- **Repository URL**: https://github.com/dthumm05/hkaiverse-assessment
