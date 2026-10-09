# AOS002 – Invalid Login (Blank Fields)

## Test Case Information

| Field | Details |
|---|---|
| Test Case ID | AOS002 |
| Module | Login / Authentication |
| Test Type | Functional / Negative Testing |
| Execution Status | PASS |

## Test Objective
Verify that the AOS application prevents users from logging in when the username and password fields are left blank and displays an appropriate validation message.

## Preconditions
- The AOS application is accessible.
- The user is logged out.
- The login form is available.

## Test Steps

| Step | Test Action | Expected Result |
|---|---|---|
| 1 | Navigate to the AOS website | Homepage loads successfully |
| 2 | Click the user/account icon | Login form appears |
| 3 | Leave the username field blank | Username remains empty |
| 4 | Leave the password field blank | Password remains empty |
| 5 | Click Sign In | Login is rejected and a required-fields validation message appears |

## Expected Result
The application should prevent login when both fields are blank and display an appropriate error message indicating that a username and password are required.

## Actual Result
The application prevented login and displayed the message: "username/password is required".

## Test Execution Result
**PASS**

## Defect ID
N/A – No defect identified.
