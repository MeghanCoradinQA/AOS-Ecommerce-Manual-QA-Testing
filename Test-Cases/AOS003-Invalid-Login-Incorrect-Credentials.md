# AOS003 – Invalid Login (Incorrect Credentials)

## Test Case Information

| Field | Details |
|---|---|
| Test Case ID | AOS003 |
| Module | Login / Authentication |
| Test Type | Functional / Negative Testing |
| Execution Status | PASS |

## Test Objective
Verify that the Advantage Online Shopping (AOS) application prevents users from logging in with invalid credentials and displays an appropriate error message.

## Preconditions
- The AOS application is accessible.
- The user is logged out.
- The login form is available.

## Test Data
- Username: Invalid test username
- Password: Invalid test password

## Test Steps

| Step | Test Action | Expected Result |
|---|---|---|
| 1 | Navigate to the AOS website | Homepage loads successfully |
| 2 | Click the user/account icon | Login form appears |
| 3 | Enter an invalid username | Username is entered into the field |
| 4 | Enter an invalid password | Password is entered into the field |
| 5 | Click Sign In | Login is rejected and an error message appears |

## Expected Result
The application should reject invalid login credentials, display an appropriate error message, and prevent unauthorized account access.

## Actual Result
The application rejected the invalid credentials and displayed the error message:

"username/password are not correct"

The user was not logged in.

## Test Execution Result
**PASS**

## Defect ID
N/A – No defect identified.
