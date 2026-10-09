# QA Test Summary Report

**Project:** Advantage Online Shopping (AOS)  
**Application Under Test:** Advantage Online Shopping Web Application  
**Test Type:** Functional Testing / Manual QA Testing  
**Environment:** Web Application / Google Chrome  
**Test Execution Status:** Completed

---

## Executive Summary

A total of **23 functional test cases** were executed across key application modules, including Login, Account Management, Product Search, Product Management, Shopping Cart, Checkout/Payments, and Social Media Links.

The application successfully completed 18 test cases, covering core e-commerce workflows such as user authentication, account creation, product searching, cart management, and checkout. Five defects were identified involving account recovery, product information, filtering, payment security, and social media navigation.

---

## Test Execution Summary

| Metric | Result |
|---|---:|
| Total Test Cases Executed | **23** |
| Passed | **18** |
| Failed | **5** |
| Blocked | **0** |
| Not Executed | **0** |
| Pass Rate | **78.3%** |
| Fail Rate | **21.7%** |

---

## Module Summary

| Module | Total | Passed | Failed |
|---|---:|---:|---:|
| Login & Authentication (AOS001–003) | 3 | 3 | 0 |
| Account Management (AOS004–009) | 6 | 5 | 1 |
| Product Search (AOS010–012) | 3 | 3 | 0 |
| Product Management (AOS013–017) | 5 | 3 | 2 |
| Cart & Shipping (AOS018–019) | 2 | 2 | 0 |
| Payment (AOS020–022) | 3 | 2 | 1 |
| Social Media Links (AOS023) | 1 | 0 | 1 |
| **Total** | **23** | **18** | **5** |

---

## Failed Test Cases

| Test Case ID | Test Case | Issue |
|---|---|---|
| **AOS008** | Forgot Password | Forgot Password link is not functional. |
| **AOS015** | Product Special Offer | Product information displays without special offer details. |
| **AOS016** | Product Specifications | Technology filter contains inconsistent options, including the misspelled "bluetooh" option. |
| **AOS022** | Save Credit Card | CVV field displays the actual CVV value instead of remaining empty. |
| **AOS023** | Follow Us – LinkedIn | LinkedIn icon opens a page that is no longer available. |

---

## Major Findings

### Functional Areas Performing Well

- User login validation
- Account creation
- Password validation
- Remember credentials
- Existing account login
- Product search and filtering
- Shopping cart functionality
- Shipping information
- SafePay checkout
- Credit card checkout
- Order completion

### Issues Identified

- Password recovery functionality is not working.
- Promotional offer details are missing.
- Product specification options contain inconsistent labels.
- CVV information is visible in the payment interface.
- The LinkedIn social media link is unavailable.

---

## Defect Priority Breakdown

The following priorities are taken from the original test records where documented. Proposed bug-report severity classifications are tracked separately.

| Priority | Count |
|---|---:|
| High | 0 |
| Medium | 2 |
| Low | 2 |
| Not specified in original record | 1 |
| **Total** | **5** |

---

## Defect Categories

| Category | Count |
|---|---:|
| Functional / Navigation | 2 |
| UI / Content / Data Quality | 2 |
| Security-Related | 1 |
| **Total** | **5** |

---

## Recommendations

1. **Investigate the CVV exposure:** Confirm payment-data handling and applicable security requirements. Ensure CVV values are not improperly retained or exposed.
2. **Repair password recovery:** Restore the Forgot Password workflow so users can initiate account recovery.
3. **Correct special offer information:** Ensure promotional details are displayed with eligible products.
4. **Review product specification filters:** Correct the Bluetooth spelling and investigate inconsistent or duplicate options.
5. **Repair the LinkedIn link:** Update the destination to a valid company page.
6. **Perform regression testing:** Retest corrected defects and related functionality before considering release approval.

---

## Overall Assessment

The Advantage Online Shopping application passed **18 of 23 executed manual functional test cases**, achieving a **78.3% pass rate**.

Core e-commerce workflows generally performed as expected within the documented test scope. However, five defects were identified, including a password recovery failure and a potentially significant payment security issue involving visible CVV information.

**Release approval is not recommended** until the CVV exposure has been investigated, applicable security requirements have been verified, and the identified defects have been appropriately triaged.

Following remediation, defect retesting and regression testing should be completed before a final release-readiness decision.

---

## Supporting Documentation

- [Manual Test Cases](../Test-Cases/)
- [Bug Reports](../Bug-Reports/)
