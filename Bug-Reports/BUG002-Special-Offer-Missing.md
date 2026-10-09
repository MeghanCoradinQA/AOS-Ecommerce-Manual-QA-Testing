# BUG002 – Special Offer Information Missing

## Defect Information

| Field | Details |
|---|---|
| Bug ID | BUG002 |
| Related Test Case | AOS015 |
| Original Test Name | AOS_ProductsSpecialOffer |
| Module | Product Special Offers |
| Defect Type | Functional / Product Information |
| Severity | Moderate (proposed) |
| Priority | Medium (original test record) |
| Test Result | FAIL |
| Defect Status | Reported during testing; current resolution unverified |
| Environment | AOS Web Application / Google Chrome |

## Defect Summary

When a user selects See Offer from the Special Offer section, the product information displays without the corresponding special offer details.

## Preconditions

- Open the AOS application in Google Chrome.
- The Special Offer section is accessible.

## Steps to Reproduce

1. Open the AOS website using Google Chrome.
2. Select the Special Offer tab.
3. Click See Offer.
4. Review the displayed product information and special offer details.

## Expected Result

The selected product should display its associated special offer details.

## Actual Result

The product information was displayed without any special offer information.

## Impact

Customers may be unable to review promotional details before deciding whether to purchase the product.

## Test Execution Result

**FAIL**

## Evidence

## Screenshot Evidence

[View BUG002 – Special Offer Screenshot (PDF)](../Screenshots/BUG%20REPORT%202%20SCREENSHOT.pdf)

## Related Test Case

AOS015 – Products Special Offer

## Notes

The defect behavior and Medium priority are supported by the original AOS015 test record. Severity is a proposed classification. Current defect resolution status has not been verified.
