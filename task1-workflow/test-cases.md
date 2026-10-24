# Task 1 — Synthetic Test Cases

## 1. Purpose

This document defines five synthetic test cases for the proposed assignment and assessment management workflow:

1. Normal submission
2. Missing information or file
3. Duplicate submission
4. Unauthorised access to another student's marks
5. Failed upload or database/storage operation

The tests describe the expected behaviour of a future prototype. They use fictional data and do not require real student records.

**Current execution status: Planned — Not Run.** No test should be marked Pass or Fail until it has actually been executed and the observed result has been recorded.

## 2. Test Environment and Safety

- **System:** Proposed assignment and assessment management workflow.
- **Data:** Synthetic students, courses, assignments, submissions, and marks only.
- **Execution status:** Planned; prototype execution has not been confirmed.
- **Purpose:** Check expected behaviour, access boundaries, and recovery paths.
- **Safety:** Do not use real student names, IDs, submissions, marks, or private information.

## 3. Test Cases

### TC-01 — Normal Submission

**Objective:** Check that a student can submit a valid assignment and receive confirmation after the submission has been saved successfully.

**Synthetic setup:**

- Student: `STU-DEMO-01`
- Course: `COURSE-DEMO-01`
- Assignment: `ASSIGN-DEMO-01`
- File: `sample-assignment.pdf`
- Submission deadline: A fictional future date configured in the test environment.

**Steps:**

1. Sign in as the synthetic student.
2. Open the assigned course and assignment.
3. Select the valid sample file.
4. Submit the assignment.
5. Check the displayed status and submission timestamp.

**Expected result:**

- The system accepts the valid submission.
- A submission record is created only after the file and record have been saved successfully.
- The student sees a confirmation or receipt with the submission timestamp.
- The submission appears in the authorised course evaluator's view.
- The system displays the correct status according to the configured deadline and policy.

**Recovery if the test fails:**

- Do not display a success receipt if saving failed.
- Show a clear error message and provide a safe retry or approved alternative route.
- Check the application and storage logs using synthetic test identifiers.

**Execution status:** Planned — Not Run.

**Observed result:** Not recorded.

**Evidence:** None yet.

---

### TC-02 — Missing Information or File

**Objective:** Check that the system prevents an incomplete submission and explains what the student needs to correct.

**Synthetic setup:**

- Student: `STU-DEMO-02`
- Course: `COURSE-DEMO-01`
- Assignment: `ASSIGN-DEMO-02`
- Attempt: Submit without attaching a required file, or omit another required field.

**Steps:**

1. Sign in as the synthetic student.
2. Open the assignment.
3. Leave the required file or field empty.
4. Attempt to submit.
5. Check the validation message and submission status.

**Expected result:**

- The system identifies the missing required information.
- The student receives a clear message explaining what is missing.
- The incomplete attempt is not recorded as a successful submission.
- No successful-submission receipt is displayed.

**Recovery if the test fails:**

- Correct the validation rules.
- Repeat the test with the required information missing.
- Verify that a valid submission can still proceed.

**Execution status:** Planned — Not Run.

**Observed result:** Not recorded.

**Evidence:** None yet.

---

### TC-03 — Duplicate Submission

**Objective:** Check that a repeated submission does not silently overwrite work or create confusing records.

**Synthetic setup:**

- Student: `STU-DEMO-03`
- Course: `COURSE-DEMO-01`
- Assignment: `ASSIGN-DEMO-03`
- First submission: `submission-v1.pdf`
- Second attempt: The same file submitted again, or a revised file submitted according to the configured policy.

**Steps:**

1. Sign in as the synthetic student.
2. Submit the first valid file.
3. Attempt to submit the same file again.
4. Check whether the system flags the duplicate or applies the configured resubmission rule.
5. Review the submission history.

**Expected result:**

- The system identifies a possible duplicate or applies the configured resubmission policy.
- The original record is not silently overwritten.
- If resubmission is allowed, the system records the new attempt and timestamp.
- If resubmission is not allowed, the system explains the restriction.
- The student can understand which submission is currently recorded.

**Recovery if the test fails:**

- Review duplicate-detection and resubmission rules.
- Ensure the system preserves the submission history.
- Repeat the test for both an identical file and a revised file if both cases are supported.

**Execution status:** Planned — Not Run.

**Observed result:** Not recorded.

**Evidence:** None yet.

---

### TC-04 — Unauthorised Access to Another Student's Marks

**Objective:** Check that a student cannot access another student's private marks or feedback.

**Synthetic setup:**

- Student A: `STU-DEMO-04`
- Student B: `STU-DEMO-05`
- Course: `COURSE-DEMO-01`
- A fictional mark and feedback record exists for Student B.

**Steps:**

1. Sign in as Student A.
2. Open Student A's own results and verify the normal access path.
3. Attempt to access Student B's marks through a direct URL, altered record identifier, or other available test interface.
4. Check the response and any relevant security log.

**Expected result:**

- Student A can access only their own authorised results.
- The attempt to access Student B's marks is denied.
- Student B's marks and feedback are not disclosed in the response.
- The system records the denied attempt where appropriate.
- Access control is enforced on the server, not only by hiding information in the user interface.

**Recovery if the test fails:**

- Treat the failure as a security issue.
- Restrict access to the affected records.
- Review server-side authorisation checks and record ownership validation.
- Repeat the test before considering the access-control requirement satisfied.

**Execution status:** Planned — Not Run.

**Observed result:** Not recorded.

**Evidence:** None yet.

---

### TC-05 — Upload or Database/Storage Failure

**Objective:** Check that the system handles a technical failure without falsely claiming that a submission was saved.

**Synthetic setup:**

- Student: `STU-DEMO-06`
- Course: `COURSE-DEMO-01`
- Assignment: `ASSIGN-DEMO-05`
- A controlled test condition causes the upload or database/storage operation to fail.

**Steps:**

1. Sign in as the synthetic student.
2. Open the assignment and select a valid sample file.
3. Trigger a controlled upload or storage failure in the test environment.
4. Check the displayed message and submission record.
5. Restore the test service and retry using the approved recovery path.

**Expected result:**

- The system displays a clear failure message.
- No success receipt is issued unless the submission has actually been saved.
- The system does not silently lose the submission or create a misleading status.
- The student receives a safe retry instruction or an approved alternative submission route.
- After the service is restored, a successful retry creates a valid record and receipt.
- The system avoids creating duplicate records if the outcome of the first attempt was uncertain.

**Recovery if the test fails:**

- Check application and storage logs using synthetic identifiers.
- Verify that failed transactions do not leave misleading or partial submission records.
- Implement or correct safe retry and duplicate-prevention handling.
- Repeat the test after the fix.

**Execution status:** Planned — Not Run.

**Observed result:** Not recorded.

**Evidence:** None yet.

## 4. Results Summary

| Test ID | Scenario                        | Expected outcome defined? | Execution status  | Result       |
| ------- | ------------------------------- | ------------------------- | ----------------- | ------------ |
| TC-01   | Normal submission               | Yes                       | Planned — Not Run | Not recorded |
| TC-02   | Missing information or file     | Yes                       | Planned — Not Run | Not recorded |
| TC-03   | Duplicate submission            | Yes                       | Planned — Not Run | Not recorded |
| TC-04   | Unauthorised marks access       | Yes                       | Planned — Not Run | Not recorded |
| TC-05   | Upload/database/storage failure | Yes                       | Planned — Not Run | Not recorded |

## 5. How to Record Actual Results Later

When a prototype is available and a test can be executed safely:

1. Record the test date and the version or commit of the code tested.
2. Run the steps using synthetic data only.
3. Record the actual observed result.
4. Mark the test **Pass** only if the observed result meets the expected outcome.
5. Mark it **Fail** if the expected behaviour is not met.
6. Record the issue, fix, and retest result if a test fails.
7. Keep evidence free of real student data and credentials.

Do not change a test to Pass based only on reading the expected result or reviewing the code without executing it.

## 6. Limitations

- These test cases define expected behaviour; they do not prove the proposed system works.
- Prototype execution has not been confirmed.
- No live university system has been accessed or tested.
- No real student records or marks are required.
- Institutional rules for deadlines, resubmissions, paper submissions, and marks release must be confirmed before implementation.

## 7. Conclusion

The five cases cover a normal workflow, incomplete input, duplicate handling, access control, and technical failure. They provide a basic validation plan for a future prototype. Actual reliability and security can only be assessed after the cases are executed and their results are documented.
