# Task 2 — Curriculum-to-Career Alignment

## 1. Objective

The objective of this analysis is to examine the relationship between the B.Tech in Computer Science and Engineering curriculum, the skills described in software-industry job postings, and possible improvements to practical learning. The analysis identifies courses and skills to retain, update, or supplement and proposes a curriculum-linked practical project.

## 2. Sources and Methodology

This analysis uses three types of evidence:

1. **Academic transcript:** My transcript records courses, grades, and credits through Semester VI, together with Summer Term II (ST-II), including Internship-I.
2. **Published programme structure:** The B.Tech CSE curriculum text available for this analysis provides a semester-wise reference, including later-semester internship, thesis, and elective components. The current public IFHE programme pages provide additional context about the published programme structure and related programmes.
3. **Job descriptions:** Three India-based software-industry job postings from Amazon, Cisco, and Wipro are used to identify technical skills, software-development practices, and expectations relevant to curriculum planning.

The sources serve different purposes and are not treated as interchangeable. The transcript documents my recorded academic history, while the published curriculum is used as a reference for comparison. Job postings indicate employer requirements for the particular roles and hiring periods reviewed; they do not represent every software-engineering job.

The comparison is qualitative. A course title alone does not establish its complete syllabus, learning outcomes, or practical depth. Where detailed course outlines, official batch-specific regulations, or reliable credit values were unavailable, the analysis records the limitation rather than assuming the missing information.

A semester-wise B.Tech CSE curriculum reference has also been provided for comparison. Its applicability to the 2023–2027 admission batch has not been confirmed, so it is treated as a reference rather than a verified statement of the complete degree requirements.

## 3. Curriculum Source and Limitation

The official curriculum and regulations specifically applicable to my 2023–2027 admission batch have not yet been independently confirmed. I therefore used my academic transcript to record completed or recorded courses and credits, and the curriculum text available to me as a separate reference for comparing course codes, titles, semester placement, and programme components.

The supplied curriculum text contains formatting and OCR ambiguities, particularly in some early-semester credit values and the later-semester layout. Consequently, only curriculum credit values that could be read with reasonable confidence have been entered in `credit-map.csv`. Ambiguous values are left blank, and possible course mismatches are flagged for verification.

The current public IFHE programme pages may represent a different curriculum version. Differences between the transcript and the reference structure should not automatically be interpreted as curricular changes or errors. They may require confirmation using the original batch handbook, official course outlines, or information from the academic office.

The analysis is therefore a provisional curriculum comparison, not a verified audit of the complete 2023–2027 degree requirements.

## 4. Transcript-Based Credit Map

The file `credit-map.csv` records the courses and credits available from my transcript through Semester VI and ST-II. It preserves the transcript course codes, titles, credits, and grades separately from the corresponding entries in the reference curriculum.

The transcript contains **136 recorded credits** across the semesters currently documented, including ST-II. This figure describes the available transcript records only; it is not the total credit requirement for graduation.

The CSV also records possible matches, differences in course wording or placement, elective-group mappings requiring confirmation, and curriculum entries whose credit values could not be read reliably. Semester VII information is incomplete or ambiguous in the supplied curriculum text, and a reliable Semester VIII structure has not been established from the material available.

For these reasons, the 136-credit figure must not be used as the denominator for a final 20–25% whole-degree redesign calculation. That calculation requires a justified programme-credit baseline and confirmation of the relevant curriculum requirements.

## 5. Programme Structure Comparison

The published IFHE programme pages for B.Tech, B.Sc, and BCA provide a high-level comparison of programme structures and areas of study. This comparison is intended to identify broad differences in programme focus and flexibility, not to claim that the programmes have identical course requirements or that their current structures applied to my admission batch.

The B.Tech CSE analysis focuses on the relationship between computing foundations, programming, databases, software engineering, systems, AI/data-related subjects, and practical project work. B.Sc and BCA structures are used as contextual comparisons where supported by the respective published programme pages.

Any statement about a specific course, credit, elective, or prerequisite should be checked against the relevant official structure or course outline before being treated as a confirmed requirement.

## 6. Job Description Analysis

Three India-based employer postings were selected to provide examples of technical skills and software-development practices relevant to curriculum planning. The postings differ in role type and eligibility, so they are not treated as equivalent opportunities for a fresher graduating in 2027.

### 6.1 Amazon — Software Development Engineer Intern, May 2027

- **Employer:** Amazon
- **Role:** Software Development Engineer Intern — May 2027
- **Location:** Bengaluru, India
- **Job ID:** 10513277
- **Source:** [Amazon Jobs — Software Development Engineer Intern, May 2027](https://www.amazon.jobs/en/jobs/10513277/software-development-engineer-intern-may-2027-2-month-amazon-university-talent-acquisition)
- **Relevance:** This posting explicitly targets students graduating in 2027, making it the closest match to the intended graduation year in this sample.

The role provides a useful reference for programming fundamentals, data structures and algorithms, object-oriented programming, software development, testing, debugging, code reviews, and technical documentation. Database, cloud, and version-control practice may also be relevant to preparing for software-development work, but each should be connected to explicit listing requirements or clearly identified as a broader preparation recommendation.

### 6.2 Cisco — Software Engineer

- **Employer:** Cisco
- **Role:** Software Engineer
- **Location:** Bengaluru, India
- **Source:** [Cisco Careers — Software Engineer](https://careers.cisco.com/global/en/job/2028048/Software-Engineer)
- **Eligibility information:** The listing describes a bachelor's degree with 0–2 years of experience or a master's degree with no experience.
- **Status:** The page indicated that applications were closed when checked on 24 October 2026.

The posting provides a technical reference for programming, data structures and algorithms, coding, debugging, testing, troubleshooting, software-development lifecycle practices, and scalable or cloud-related systems. Its closed application status means it should be used as a skills reference rather than presented as an open vacancy.

### 6.3 Wipro — Junior .NET Software Engineer Channels

- **Employer:** Wipro
- **Role:** Junior .NET Software Engineer Channels
- **Location:** Mumbai, India
- **Job ID:** 203309
- **Posting start date:** 26 September 2026
- **Source:** [Wipro Careers — Junior .NET Software Engineer Channels](https://careers.wipro.com/job/Junior-_NET-Software-Engineer-Channels/203309-en_US/)
- **Eligibility information:** The listing requires 3–5 years of experience.

The posting provides a technical reference for software-module development, testing, integration, validation, user acceptance testing (UAT), documentation, and collaboration. Because the experience requirement is 3–5 years, this is **not a direct fresher opportunity**. It is included only as a technical-skills comparator.

### 6.4 Common Skill Areas

The three postings provide a limited sample of employer expectations. The following comparison connects the technical areas discussed in the postings with the curriculum and proposed learning improvements.

| Skill area                                  | Job-description evidence                                                                                                | Curriculum connection                                                                          |
| ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| Programming and object-oriented programming | Relevant to Amazon and Cisco; software development is also relevant to Wipro                                            | Computer Programming, Object Oriented Programming Concepts, and programming practice           |
| Data structures and algorithms              | Relevant to Amazon and Cisco                                                                                            | Data Structures and Design and Analysis of Algorithms                                          |
| Software development and maintenance        | Relevant across the three postings, with different role-specific emphasis                                               | Software Engineering, Web-Enabled Technologies, and practical project work                     |
| Testing, debugging, and troubleshooting     | Relevant across the postings, although the exact activities differ                                                      | Software Engineering, programming laboratories, internship work, and project assessment        |
| Application integration                     | Particularly relevant to Wipro's development and integration work; also connected to the software-development lifecycle | Database Management Systems, Web-Enabled Technologies, API exercises, and integrated projects  |
| Cloud and scalability                       | Relevant to Amazon and Cisco's software-engineering context                                                             | Cloud Computing, Computer Networks, and systems-related practical work                         |
| Documentation and collaboration             | Relevant to Amazon and Wipro's development practices                                                                    | Software Engineering, internship activities, project documentation, and team-based assignments |

This table is a qualitative mapping, not a claim that every listed skill appears in every posting or is fully covered by the corresponding course. The detailed syllabus and actual learning outcomes must be reviewed before confirming the depth of coverage.

The three-posting sample is small and selected for comparison. It should not be interpreted as a representative survey of the Indian software job market.

## 7. Curriculum-to-Career Gap Analysis

The course-to-career analysis distinguishes between existing academic foundations, areas that require syllabus-level verification, practical integration opportunities, and employer-specific requirements.

- **Existing foundations:** Topics already represented in the transcript include data structures, algorithms, object-oriented programming, databases, operating systems, computer networks, software engineering, and AI/data-related courses.
- **Depth requiring syllabus review:** Areas where a course title suggests relevance but the detailed syllabus is unavailable. The title alone does not prove that a particular tool, framework, or industry practice is taught.
- **Practical integration opportunities:** Opportunities to connect programming, database design, APIs, testing, security, version control, and deployment through integrated assignments and projects.
- **Employer-specific requirements:** Skills explicitly requested in the reviewed job descriptions that may need additional practice or deeper coverage.
- **Eligibility considerations:** A posting can provide useful technical skill signals without being a suitable application target. The Amazon internship is aligned with the stated 2027 graduation year, the Cisco listing was closed when checked, and the Wipro listing requires 3–5 years of experience.

The presence of a subject in the transcript does not by itself prove mastery of every associated industry skill. Similarly, a skill not visible in a course title should not automatically be described as absent from the curriculum without checking the course outline.

The main opportunity identified by this preliminary analysis is to strengthen the connection between existing computing foundations and practical software-development workflows. This can be explored through integrated exercises involving requirements, database operations, APIs, access control, testing, debugging, and documentation, subject to syllabus review.

## 8. Curriculum Recommendations

Recommendations should be linked to the transcript, the reference curriculum, and the job-description evidence. Each recommendation should state the identified need, the evidence supporting it, the proposed change, and any dependency or verification requirement.

- **KEEP:** Retain useful computing foundations and existing subjects where the available evidence supports their relevance. Programming, object-oriented programming, data structures and algorithms, databases, and software engineering provide foundations for several technical areas identified in the reviewed postings.
- **UPDATE:** Consider strengthening practical coverage in subjects such as web technologies, databases, software engineering, systems, cloud computing, and AI/data-related courses where the reviewed job requirements or proposed project reveal a credible need. Confirm detailed syllabi before claiming a specific topic is missing.
- **REDUCE:** Do not recommend reducing a course or its credits solely because its title appears less directly connected to a selected job description. Any reduction needs evidence of redundancy, learning-outcome overlap, or a justified programme-design trade-off, and must respect official requirements.
- **ADD:** Consider integrated practical exercises or a capstone that connects requirements analysis, database design, application development, access control, testing, and deployment. Proposed additions must be evaluated against confirmed programme requirements and available credit space.

Detailed recommendations and their rationale are recorded in `recommendations.md`. The proposed Assignment Submission and Review Management System is documented in `capstone-lab.md` as a proposed learning activity, not as a completed or officially approved university project.

## 9. Credit and Redesign Calculation

A redesign target of approximately 20–25% of programme credits must be calculated using a verified or otherwise explicitly justified total programme-credit baseline. The available 136 transcript credits cover only the recorded semesters and ST-II; they do not establish the complete degree-credit total.

Until the complete applicable curriculum and its credit totals are confirmed, any proposed redesign percentage should be labelled provisional. The redesign should identify affected courses or learning components, distinguish changes to content from changes to credit allocation, preserve prerequisites, and account for applicable academic or regulatory constraints.

No final whole-degree credit calculation is claimed in this report at this stage. The transcript's 136 recorded credits are not used as the denominator for the final programme-wide redesign target.

## 10. Practical Project Proposal

The proposed Assignment Submission and Review Management System connects curriculum learning with a practical workflow. It is intended to provide a context for applying requirements analysis, database design, application logic, role-based access, testing, and deployment concepts.

The project specification identifies proposed features, acceptance criteria, and planned tests. These are design artefacts, not evidence that a working application has been implemented or that its tests have passed. Implementation status and test results must be reported only after the relevant work has actually been completed and checked.

See `capstone-lab.md` for the proposed specification and test plan.

## 11. AI-Assisted Curriculum Exercises

The repository includes five AI-assisted exercises associated with selected subjects. Each exercise should record the prompt, AI tool and model, date, output summary, verification method, evidence, and final decision.

AI-generated explanations and recommendations are treated as suggestions rather than authoritative curriculum facts. Unverified outputs must remain labelled as pending verification, and no implementation, experiment, or test should be described as completed unless it was actually performed.

See `ai-exercises.md` for the exercise records.

## 12. Feedback and Validation Limitations

Formal faculty or graduate feedback has not been established as part of this analysis. Personal observations and questions for future feedback should not be presented as formal interviews, survey results, or institutional endorsement.

The recommendations are provisional and would benefit from faculty review, confirmation of official course outlines, and feedback from graduates or recruiters. The proposed project also requires implementation and testing before claims can be made about its effectiveness.

See `feedback.md` for the recorded feedback limitations and questions for future validation.

## 13. Limitations

This analysis covers the transcript entries currently available through Semester VI and ST-II, recording 136 credits. These figures represent the available transcript records only and do not establish the total credit requirement for the complete B.Tech CSE programme.

A semester-wise B.Tech CSE curriculum reference is available, but its applicability to the 2023–2027 admission batch has not been confirmed. Some semester, course, and credit details in the supplied reference are ambiguous and require verification against the applicable official curriculum.

The job-description sample contains three selected postings and is not representative of the entire Indian software job market. The postings have different eligibility conditions: the Amazon internship targets 2027 graduates, the Cisco listing was closed when checked on 24 October 2026, and the Wipro role requires 3–5 years of experience. The Cisco and Wipro listings are therefore used as technical comparisons rather than confirmed, currently open opportunities suitable for this graduate profile.

Course-to-job mappings are preliminary interpretations of public employer descriptions and transcript course titles, not verified syllabus-level matches. Course titles alone cannot establish the depth of practical coverage, duplication between subjects, or the need to remove credits.

The recommendations are proposals for further review, not confirmed faculty decisions. No formal faculty or graduate feedback was obtained for this analysis. Any future feedback should be documented accurately and distinguished from the author's own observations.

## 14. Sources

The following employer pages were used as the job-description references for this report. Listing details and availability may change, so the original pages should be rechecked before final submission.

1. **Amazon Jobs — Software Development Engineer Intern, May 2027**, Job ID 10513277.  
   https://www.amazon.jobs/en/jobs/10513277/software-development-engineer-intern-may-2027-2-month-amazon-university-talent-acquisition

2. **Cisco Careers — Software Engineer**, Bengaluru.  
   https://careers.cisco.com/global/en/job/2028048/Software-Engineer  
   The page indicated that applications were closed when checked on 24 October 2026.

3. **Wipro Careers — Junior .NET Software Engineer Channels**, Job ID 203309.  
   https://careers.wipro.com/job/Junior-_NET-Software-Engineer-Channels/203309-en_US/  
   The listing states a requirement of 3–5 years of experience and is included as a technical-skills comparator.

The academic evidence consists of the available student transcript, the supplied semester-wise curriculum reference, and public IFHE programme information. The transcript and reference curriculum are kept separate because the applicable curriculum version and complete programme-credit total have not yet been confirmed.

**Access date for employer postings:** 24 October 2026.

## 15. Conclusion

The available evidence supports a preliminary comparison between recorded coursework, a published curriculum reference, and skills requested in selected job descriptions. It also supports proposing an integrated practical project to connect several computing subjects.

The main limitations are the unconfirmed applicability of the reference curriculum to the 2023–2027 batch, ambiguities in the supplied curriculum text, incomplete later-semester credit information, and the limited number and scope of job postings. The sample also includes postings with different eligibility conditions, so technical relevance should not be confused with application eligibility.

The next validation steps are to confirm the applicable batch curriculum and complete credit totals, verify course-level learning outcomes, recheck the dated job-description evidence, and execute the proposed project tests before reporting implementation results. A final 20–25% programme-wide redesign calculation should be made only after the applicable total programme-credit baseline has been verified.
