# Changelog

## [1.12.0] - 24/09/2024

### Added
- Added overrideDuFee field in the passenger array above the nationality field.
- New method to perform DU override in international reserves.
- Added adjusted field in passenger array above name.
- Added new error message for session transfer.
- Added promotionCode field in FromAttach method.
- Added Mercosur document type in the reserve creation methods.
- Added notifyContacts field in the checkout methods Order V1 and Order.Management V2.

### Updated
- Increase in the timeout of Apis.
- The method that applies the DU was modified to consider the new operation for DUI, applying a maximum of 7% of the value for each passenger.
- The booking search method has been modified to validate if the reservation is being moved.
- The booking creation method has been modified, it will be mandatory to insert the document only if the Type or the currency of the agency is selected for BRL.
- The group checkout method has been modified to allow partial payment and no limit on the amount of payment.
- The checkout methods have been modified to allow the checkout of baby reservations, provided that the minimum payment is made.

[Link to previous versions](/docs/en-us/change-log/readme.history.md)