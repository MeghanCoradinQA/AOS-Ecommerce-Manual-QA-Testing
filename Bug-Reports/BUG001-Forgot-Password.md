# BUG001 – Forgot Password Link Not Functioning

## Defect Information

| Field | Details |
|---|---|
| Bug ID | BUG001 |
| Related Test Case | AOS008 |
| Module | Login / Account Recovery |
| Defect Type | Functional |
| Severity | Major (proposed) |
| Priority | High (proposed) |
| Status | Open at time of testing; current status unverified |
| Environment | Google Chrome / AOS Web Application |

## Defect Summary

The Forgot Password link does not function, preventing users from proceeding to the password recovery process.

## Preconditions

- The AOS application is accessible.
- The user is logged out.
- The login interface is available.

## Steps to Reproduce

1. Open the AOS application in Google Chrome.
2. Click the user/account icon.
3. Select Sign In.
4. Click Forgot your password.

## Expected Result

The user should be directed to the password recovery interface, where they can enter their registered email address to request a password reset link.

## Actual Result

The Forgot Password link was not functional during testing. The user could not proceed to the password recovery process.

## Impact

Users who forget their passwords may be unable to recover access to their accounts using the available recovery link.

## Evidence

No screenshot attached. Add original test evidence if available.

## Related Test Case

AOS008 – Forgot Password

## Notes

Defect behavior is based on the original AOS008 execution record. Severity and priority are proposed for portfolio presentation. Current resolution status has not been verified.
