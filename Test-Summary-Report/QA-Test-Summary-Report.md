QA Test Summary Report
Project: Advantage Online Shopping (AOS)
Application Under Test: Advantage Online Shopping Web Application
Test Type: Functional Testing / Manual QA Testing
Environment: Web Application
Test Execution Status: Completed
Executive Summary
A total of 23 functional test cases were executed across key application modules including Login, Account Management, Product Search, Product Management, Shopping Cart, Checkout/Payments, and Social Media Links.
Overall, the application performed well for its core e-commerce functionality such as user authentication, account creation, product searching, shopping cart management, and payment processing. However, several defects were identified that affect usability, security, and user experience.

Test Execution Summary
Metric
Result
Total Test Cases Executed
23
Passed
18
Failed
5
Blocked
0
Not Executed
0
Pass Rate
78.3%
Fail Rate
21.7%


Module Summary
Module
Total
Passed
Failed
Login
3
3
0
Account Management
6
5
1
Search Functionality
3
3
0
Products
5
2
3
Cart & Shipping
2
2
0
Payment
3
2
1
Follow Us Links
1
0
1


Failed Test Cases
Test Case ID
Test Case
Severity
Issue
AOS008
Forgot Password
High
Forgot Password link is not functional. User cannot initiate password reset.
AOS015
Product Special Offer
Medium
Product page displays product information but no special offer details.
AOS016
Product Specifications
Low
Wireless Technology filter contains duplicate/inconsistent options. One option is misspelled as "bluetooh."
AOS022
Save Credit Card
Medium
Saved credit card displays actual CVV instead of leaving the field blank, creating a security concern.
AOS023
Follow Us - LinkedIn
Low
LinkedIn icon redirects to a page that is no longer available.


Major Findings
Functional Areas Performing Well
User login validation
Account creation
Password validation
Remember credentials
Existing account login
Product search
Product filtering
Shopping cart functionality
Shipping information
SafePay checkout
Credit card checkout
Order completion
Issues Identified
Password recovery functionality is broken.
Promotional offers are not displaying correctly.
Product specification filter contains inconsistent values and a spelling error.
Sensitive payment information (CVV) remains visible after saving a credit card.
LinkedIn social media link is broken.

Severity Breakdown
Severity Count
Count
High
1
Medium
2
Low
2


Defect Categories
Category
Count
Functional Defects
2
UI/Content Defects
2
Security Defects
1


Recommendations
Fix the Forgot Password workflow immediately, as it prevents users from recovering access to their accounts.
Update the credit card save functionality to mask the card number and ensure the CVV field is always blank after saving, following payment security best practices.
Restore or update the LinkedIn social media link to a valid page.
Correct the product filter spelling ("Bluetooth") and remove duplicate or obsolete specification options.
Verify that special offer information is correctly associated with eligible products and displayed on the product page.

Overall Assessment
The Advantage Online Shopping application passed 18 of 23 executed manual functional test cases, achieving a 78.3% pass rate. Core shopping, authentication, and checkout workflows generally performed as expected within the documented test scope. Five defects were identified, including an account recovery failure and a potentially significant payment security issue involving visible CVV information.
Release approval is not recommended until the CVV exposure is investigated, security requirements are verified, and the identified defects are appropriately triaged. Following remediation, defect retesting and regression testing should be performed before a final release-readiness decision.

