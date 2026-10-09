# BUG004 – Saved Credit Card CVV Displayed in Plain Text

## Defect Information

| Field | Details |
|---|---|
| Bug ID | BUG004 |
| Related Test Case | AOS022 |
| Original Test Name | AOS_CartPaymentSaveCreditcard |
| Module | Shopping Cart / Checkout / Payment |
| Defect Type | Security / Sensitive Data Exposure |
| Severity | High (proposed) |
| Priority | Medium (original test record) |
| Test Result | FAIL |
| Defect Status | Reported during testing; current resolution unverified |
| Environment | AOS Web Application / Google Chrome |

## Defect Summary

During checkout, the saved credit card payment information displays the actual CVV value instead of leaving the CVV field empty.

## Preconditions

- Open the AOS application using Google Chrome.
- A product is available to add to the shopping cart.
- Saved payment information is available for review during checkout.

## Steps to Reproduce

1. Open the AOS application in Google Chrome.
2. Select a product and add it to the shopping cart.
3. Proceed to checkout.
4. Select the mailing address.
5. Review the displayed credit card payment information.
6. Check whether the card number is masked and the CVV field is empty.

## Expected Result

The credit card number should be masked with security asterisks, and the CVV field should be empty.

## Actual Result

The CVV field displayed the actual CVV number during testing.

## Impact

Displaying a CVV value can expose sensitive payment information to anyone able to view the checkout screen. This behavior warrants investigation of payment-data handling and applicable security requirements.

## Test Execution Result

**FAIL**

## Evidence

Original test execution record: AOS022.

## Screenshot Evidence

[View BUG004 – CVV Field Defect Screenshot (PDF)](../Screenshots/BUG%20REPORT%204%20SCREENSHOT.pdf)

## Related Test Case

AOS022 – Cart Payment Save Credit Card

## Recommended Investigation

- Verify why the CVV value is displayed during checkout.
- Confirm whether CVV data is retained after authorization.
- Review the payment workflow against applicable PCI DSS requirements.
- Retest with approved dummy payment data after remediation.

## Notes

The CVV exposure, Medium priority, and FAIL result are taken from the original AOS022 test record. High severity is proposed based on potential security impact. The original test does not establish whether CVV data was stored or how long it remained available. The current resolution status is unverified.
