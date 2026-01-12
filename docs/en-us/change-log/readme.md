# Changelog

## [1.18.0] - 03/11/2025

### Added
- Added method to change the promotion code of a reservation in Hold.
- Added field for sending booking itinerary (Agency, None and All).
- Added field to send comments on booking.
- Added method to update data of the Agency and Customer contacts from a reservation in Hold.
- Added method to return valid routes.
- Added method to remove Promotion Code during creation.
- Added method to remove Promotion Code for reservations in Hold.
- Addition of RE travel document for exclusive use by Azul in the issuance of reservations.
- Addition of RE travel document for exclusive use of Azul in changing passenger data.

### Updated
- Improvement in the error message if Installments API unavailability occurs.
- The 'OrganizationFeeOverride' is disabled, the value sent will not overwrite the OrganizationFee during the creation of the Order.
- Released the option of requesting a refund via CreditShell for reservations in re-accommodation.
- Added Reallocation report in the Reports ApI.
- Block the search, creation and modification of codeshare (G3) reservations with more than 4 passengers.
- Improvements in validations and unavailability of the installment api.
- Removed DU change method of international reservations.
- Added the option to generate reports per month for Payments and Segments reports.
- Return of total baggage for the new tiers Diamante Unique and Azul One.
- Restriction of issuance of reservations CodeShare (G3) by IATA.
- Restriction of addition of segment CodeShare (G3) by IATA blocked.
- Flight search restriction CodeShare (G3) by IATA blocked.

[Link to previous versions](/docs/en-us/change-log/readme.history.md)