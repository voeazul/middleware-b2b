# Changelog

## [1.25.0] - 2026/09/30

### Added
- Added a new custom period type (date range) for extracting the Payment Report on the **Sales.B2B.Reports.Api**, allowing queries beyond the existing day, week, and month options.
- Released a new version (V2) of the IROP contact registration and update methods on the **Sales.B2B.Order.Api**, **Order.Management.Api**, and **Organizations.Api**.

### Changed
- Updated the Reaccommodation Report on the **Sales.B2B.Reports.Api** to no longer include GDS or Group bookings, returning only reservations within the B2B context.
- Fixed the monetary values returned in the Sales Report on the **Sales.B2B.Reports.Api**, which were being displayed without the correct decimal places; added the organization code and organization name fields and reorganized the field display order.
- Fixed the Segment Report search on the **Sales.B2B.Reports.Api** to consider all agents within the requesting agency, rather than only the agent who generated the request; added the booking creation date field and reorganized the field display order.
- Changed the organization lookup permission on the **Sales.B2B.Organizations.Api**, allowing internal integrations to retrieve organization data without requiring a link to a commercial group.
- Fixed the passenger name change verification response on the **Sales.B2B.Order.Passengers.Api**, so it now correctly indicates which passengers have already had their name changed on bookings with multiple travelers.
- Excluded bookings created by Portal Grupos from the booking search (SearchBy) on the **Sales.B2B.Order.Management.Api**, keeping only bookings within the B2B context in the results.
- Made the IROP contact (IropContact) mandatory on the **Sales.B2B.Order.Api**, with the phone number now provided as three separate fields (country code, area code, and number).
- Added unruly passenger validation to the **Sales.B2B.Order.Api** and **Sales.B2B.Order.Management.Api**, preventing reservations containing this type of passenger from being confirmed through checkout. For passengers with **BR** nationality, providing a **CPF** document will be mandatory. This validation is independent of the existing BPE blocking rules and will apply exclusively to 100% domestic flights. International flights or itineraries involving an international connection will not be subject to this validation.

[Link to previous versions](/docs/en-us/change-log/readme.history.md)