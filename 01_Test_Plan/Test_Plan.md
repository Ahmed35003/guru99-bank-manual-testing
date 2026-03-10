# Test Plan — Guru99 Bank

**Document Version:** 1.0  
**Date:** 2025  
**Prepared By:** [Your Name]  
**SRS Reference:** Guru99 Bank SRS v2.0

---

## 1. Introduction

This Test Plan defines the strategy, scope, resources, and schedule for manual testing of the **Guru99 Bank** web application. It is based on the Software Requirements Specification (SRS) v2.0 approved on 19/11/2013.

---

## 2. Test Objectives

- Verify all functional requirements defined in SRS v2.0
- Validate all field-level technical validations (T1–T110)
- Validate all functional business rules (F1–F49)
- Confirm correct role-based access for Manager and Customer
- Ensure the application behaves correctly for both valid and invalid inputs

---

## 3. Scope

### 3.1 In Scope

| Area                        | Details                                      |
|-----------------------------|----------------------------------------------|
| Functional Testing          | All 14 modules for both Manager and Customer |
| Field Validation Testing    | All T1–T110 technical requirements           |
| Business Rules Testing      | All F1–F49 functional validations            |
| Role-Based Access Testing   | Manager vs Customer permissions              |
| Positive Testing            | Valid inputs and expected happy paths        |
| Negative Testing            | Invalid inputs, boundary violations          |
| UI Field Verification       | Correct fields present per module            |

### 3.2 Out of Scope

| Area                        | Reason                                         |
|-----------------------------|------------------------------------------------|
| Performance / Stress Testing | Explicitly excluded in SRS section 1.2        |
| Automation Testing           | Explicitly excluded in SRS section 1.2        |
| Security / Penetration Testing | Not mentioned in SRS                        |
| Mobile / Cross-Browser Testing | SRS specifies Chrome 27+ only              |
| API Testing                  | No API interfaces defined in SRS             |

---

## 4. Test Approach

Testing will be **manual and black-box**. Test cases are derived directly from SRS requirements and organized by module.

### 4.1 Test Types

| Test Type            | Description                                                    |
|----------------------|----------------------------------------------------------------|
| Smoke Testing        | Verify the application loads and login works before full run   |
| Functional Testing   | Validate each module against SRS requirements                  |
| Positive Testing     | Valid data inputs should produce correct expected results      |
| Negative Testing     | Invalid/boundary data should produce correct error messages    |
| Role-Based Testing   | Verify Manager and Customer access restrictions               |

---

## 5. Test Environment

| Component       | Details                        |
|-----------------|-------------------------------|
| Application URL | https://www.guru99.com/live-selenium-project.html |
| Browser         | Google Chrome 27+             |
| OS              | Windows / macOS               |
| Test Data       | Manually created per test case |

---

## 6. Roles & Responsibilities

| Role            | Responsibility                                               |
|-----------------|--------------------------------------------------------------|
| QA Engineer     | Write test cases, execute tests, log defects                |
| (Manager Role)  | Accessible — Manager module tests will be executed          |
| (Customer Role) | Not accessible — TCs designed, marked Not Executed          |

---

## 7. Test Deliverables

| Deliverable                      | Location                            |
|----------------------------------|-------------------------------------|
| Test Plan                        | `01_Test_Plan/Test_Plan.md`         |
| Test Cases (14 files)            | `02_Test_Cases/`                    |
| Requirements Traceability Matrix | `03_RTM/Requirements_Traceability_Matrix.md` |
| Bug Reports                      | `04_Bug_Reports/`                   |
| Test Summary Report              | `05_Test_Summary_Report/Test_Summary_Report.md` |

---

## 8. Entry Criteria

- SRS v2.0 reviewed and understood
- Test environment (browser + URL) is accessible
- Test cases are written and reviewed
- Manager credentials are available

## 9. Exit Criteria

- All Manager test cases executed
- All critical and high-severity defects resolved or documented
- RTM updated with execution results
- Test Summary Report completed

---

## 10. Suspension & Resumption Criteria

| Condition                              | Action                          |
|----------------------------------------|---------------------------------|
| Application is completely inaccessible | Suspend testing, notify team    |
| Login feature is broken                | Suspend — all tests depend on it|
| Environment restored                   | Resume from last executed TC    |

---

## 11. Risks & Mitigations

| Risk                                    | Mitigation                                          |
|-----------------------------------------|-----------------------------------------------------|
| Customer portal not accessible          | TCs designed from SRS; marked Not Executed          |
| Demo site may be reset between sessions | Re-create test data at the start of each session   |
| Demo site may be unavailable            | Document date/time of any downtime                 |
| SRS has minor typos / ambiguities       | Interpreted based on context; noted in test cases  |

---

## 12. Test Schedule

| Activity                  | Status       |
|---------------------------|-------------|
| SRS Review                | ✅ Complete  |
| Test Plan Creation        | ✅ Complete  |
| Test Case Writing         | ✅ Complete  |
| RTM Creation              | ✅ Complete  |
| Test Execution (Manager)  | ⬜ Pending   |
| Test Execution (Customer) | ⬜ Not Accessible |
| Bug Reporting             | ⬜ Pending   |
| Test Summary Report       | ⬜ Pending   |
