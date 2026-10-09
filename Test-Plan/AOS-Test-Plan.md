# AOS E-Commerce Application — Manual QA Test Plan

**Project:** Advantage Online Shopping (AOS)  
**Application Under Test:** Advantage Online Shopping Web Application  
**Role:** QA Tester — Manual Testing and Defect Reporting  
**Test Approach:** Manual functional testing  
**Document Status:** Retrospective test plan based on documented execution  
**Test Environment:** Web application accessed with Google Chrome  

---

## 1. Purpose and Overview

This document organizes the scope, approach, execution criteria, risks, and deliverables for the Advantage Online Shopping manual QA project. It is a **retrospective test plan** reconstructed from the recorded test cases and execution results; it is not presented as an approved plan written before testing began.

The project evaluated core e-commerce workflows by executing predefined manual test cases, comparing expected and actual outcomes, and documenting observed defects.

## 2. Test Objectives

- Verify login behavior with valid, blank, and incorrect credentials.
- Validate account creation and password requirements.
- Check remembered credentials, password recovery, and existing-account access.
- Validate product search, filtering, specifications, and special-offer information.
- Verify product selection, cart behavior, and shipping information.
- Exercise SafePay and credit-card checkout workflows, including saved payment information display.
- Verify footer social media navigation.
- Record results and report reproducible defects.

## 3. Scope

### In Scope

| Area | Covered test cases | Focus |
|---|---|---|
| Login and authentication | AOS001–AOS003 | Valid, blank, and incorrect credentials |
| Account management | AOS004–AOS009 | Registration, password constraints, remembered credentials, password recovery, existing account |
| Product search | AOS010–AOS012 | Partial/full searches and category search |
| Product management | AOS013–AOS017 | Product selection, price filters, special offers, specifications, color |
| Cart and shipping | AOS018–AOS019 | Cart/checkout navigation and shipping details |
| Payments | AOS020–AOS022 | SafePay, credit-card checkout, saved-card display |
| Social media navigation | AOS023 | Follow Us links |

### Outside the Documented Scope

The available execution records do not establish performance/load testing, accessibility auditing, API testing, automated testing, formal UAT, or completed post-fix regression testing. These activities are **not claimed as completed** in this project.

## 4. Test Approach and Design

- **Method:** Manual functional testing of user-facing web workflows.
- **Test basis:** Recorded test scenarios and expected results in the AOS test-case document.
- **Design techniques evident in the cases:** Positive and negative input checks (including valid/invalid login and password inputs) and workflow-based scenarios.
- **Execution:** Follow documented steps, compare actual outcomes with expected results, and mark each test PASS or FAIL.
- **Defect documentation:** Capture the related test case, observed behavior, expected behavior, reproduction steps, and a proposed severity classification where appropriate.

No automated execution or Jira system integration is asserted; the portfolio uses **Jira-style** defect-report formatting.

## 5. Test Environment and Data

| Item | Documented information |
|---|---|
| Application | Advantage Online Shopping web application |
| Browser | Google Chrome |
| Execution method | Manual interaction with the application |
| Test data | Account inputs, product searches, product options, and checkout/payment test inputs described in individual test cases |

**Data-handling note:** Public GitHub documentation should not contain real passwords, payment card numbers, CVV values, or personal account information. Use redacted examples or approved dummy data instead.

Browser version, operating-system version, device specifications, and execution dates were not consistently established in the source records and are therefore not asserted here.

## 6. Entry and Exit Criteria

The following are **retrospective planning criteria**, not independently verified pre-execution approvals.

### Suggested Entry Criteria

- The AOS application is accessible in Chrome.
- Relevant pages and features are available for testing.
- Test scenarios, expected results, and suitable test data are prepared.

### Execution Completion Criteria

- Every planned test case has a recorded execution outcome.
- Failures are documented with expected and actual behavior.
- Test execution totals and outstanding issues are summarized.

**Actual recorded outcome:** 23 executed; 18 passed; 5 failed; 0 blocked; 0 not executed. Completion of execution does not imply release approval.

## 7. Defect Management

Each failed test is cross-referenced to a Jira-style Markdown bug report. Severity classifications added to the bug reports are **proposed**, not verified as formally assigned by a development team. Priority values are retained from the original test records where available.

| Bug ID | Test case | Defect summary | Original test priority |
|---|---|---|---|
| BUG001 | AOS008 | Forgot Password link not functional | Not specified in source record |
| BUG002 | AOS015 | Special offer details missing | Medium |
| BUG003 | AOS016 | Inconsistent/misspelled specification option | Low |
| BUG004 | AOS022 | CVV value visible in payment interface | Medium |
| BUG005 | AOS023 | LinkedIn link leads to unavailable page | Low |

The original records do not confirm defect fixes, developer assignments, or completed defect retesting.

## 8. Risks and Limitations

- **Payment-data exposure:** The visible CVV observation requires investigation. The test record does not establish whether the CVV was stored or retained after authorization.
- **Account recovery:** An inoperative Forgot Password link can prevent users from initiating password reset.
- **Product information:** Missing offers and inconsistent specification labels may affect purchase decisions.
- **External navigation:** The LinkedIn destination was unavailable during testing.
- **Coverage limitations:** The 23 documented cases do not establish comprehensive security, compatibility, performance, or accessibility coverage.

## 9. Execution Results

| Metric | Result |
|---|---:|
| Total executed | 23 |
| Passed | 18 |
| Failed | 5 |
| Blocked | 0 |
| Not executed | 0 |
| Pass rate | 78.3% |
| Fail rate | 21.7% |

### Module Breakdown

| Module | Total | Passed | Failed |
|---|---:|---:|---:|
| Login and authentication (AOS001–003) | 3 | 3 | 0 |
| Account management (AOS004–009) | 6 | 5 | 1 |
| Product search (AOS010–012) | 3 | 3 | 0 |
| Product management (AOS013–017) | 5 | 3 | 2 |
| Cart and shipping (AOS018–019) | 2 | 2 | 0 |
| Payments (AOS020–022) | 3 | 2 | 1 |
| Social media navigation (AOS023) | 1 | 0 | 1 |
| **Total** | **23** | **18** | **5** |

## 10. Recommendations and Next Steps

1. Investigate the visible CVV value and review applicable payment security requirements.
2. Repair the password recovery workflow.
3. Correct missing special-offer information and inconsistent specification options.
4. Repair the LinkedIn navigation link.
5. **After fixes are available**, retest the affected defects and conduct relevant regression testing. These are recommendations, not activities claimed as already completed.
6. Reassess release readiness using defect disposition, retest evidence, and security review—not pass rate alone.

## 11. Deliverables and References

- [23 Manual Test Cases](../Test-Cases/)
- [5 Jira-Style Bug Reports](../Bug-Reports/)
- [QA Test Summary Report](../Test-Summary-Report/QA-Test-Summary-Report.md)
- [Project README](../README.md)

---

**Project outcome:** The documented manual test execution identified five failures among 23 test cases. The project demonstrates manual functional test design and execution, expected-versus-actual comparison, defect reporting, and test result communication.

