# Changelog

## [1.23.0] - 08/11/2026

### Added
- Added the _PATCH Passenger_ method to allow passenger data updates, providing the mechanism to update traveler documents in the **Sales.B2B.Order.Passengers.Api**.
- Added the _POST Contact_ method to allow the registration and completion of required contact information when a booking does not have a _Customer_ contact in the **Order.Management.Api**.

### Updated
- Updated and enforced a restriction preventing reservation payments when required travel documents are missing, according to the traveler's nationality.
- Updated the reservation creation flow by adding the new **GOVID** field and nationality validation in the **Order.Api**.
  If the govId is not provided, a warning will be displayed, but this will not affect the creation of the reservation. The notification will remain active until the permanent block is applied, after the deadline set by Azul business unit.
- Updated the reservation contact change flow by adding the new **GOVID** field and nationality validation in the **Order.Management.Api**.

[Link to previous versions](/docs/en-us/change-log/readme.history.md)