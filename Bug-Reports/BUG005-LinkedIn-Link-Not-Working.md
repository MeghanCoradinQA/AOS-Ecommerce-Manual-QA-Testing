# BUG005 – LinkedIn Social Media Link Not Working

## Defect Information

| Field | Details |
|---|---|
| Bug ID | BUG005 |
| Related Test Case | AOS023 |
| Original Test Name | AOS_FollowUs |
| Test Scenario | AOS_FollowUs |
| Module | Footer / Social Media Navigation |
| Defect Type | Functional / Navigation |
| Severity | Minor (proposed) |
| Priority | Low (original test record) |
| Test Result | FAIL |
| Defect Status | Reported during testing; current resolution unverified |
| Environment | AOS Web Application / Google Chrome |
| Test Data | Facebook, Twitter, LinkedIn icons |

## Defect Summary

The LinkedIn icon in the FOLLOW US section directs the user to a page displaying a "page no longer available" message instead of a working LinkedIn destination.

## Preconditions

- Open the AOS application in Google Chrome.
- The application footer is accessible.

## Steps to Reproduce

1. Open the AOS application in Google Chrome.
2. Scroll to the bottom of any application page.
3. Locate the FOLLOW US section.
4. Select the LinkedIn icon.
5. Observe the destination page.

## Expected Result

Selecting the LinkedIn icon should open the corresponding LinkedIn destination, allowing the user to continue to the follow or login process as needed.

## Actual Result

The LinkedIn icon opened a page displaying "page no longer available."

## Impact

Users may be unable to access the company's LinkedIn presence through the website, disrupting social media navigation.

## Test Execution Result

**FAIL**

## Evidence

Original AOS023 test execution record. No screenshot attached.

## Related Test Case

AOS023 – Follow Us

## Recommended Investigation

- Verify the LinkedIn destination URL configured for the icon.
- Confirm that the intended LinkedIn page is active and accessible.
- Correct the link if necessary.
- Retest the LinkedIn icon after remediation.

## Notes

The original AOS023 test record confirms the failed LinkedIn destination and Low priority. Minor severity is a proposed classification. The exact cause of the unavailable page and the current defect resolution status have not been verified. The record does not establish that the Facebook or Twitter links failed.
