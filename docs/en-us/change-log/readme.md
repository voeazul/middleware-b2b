# Changelog

## [1.25.0] - 2026/09/30

### Added
- Added a new custom period type (date range) for extracting the Payment Report on the **Sales.B2B.Reports.Api**, allowing queries beyond the existing day, week, and month options.
- Released a new version (V2) of the IROP contact registration and update methods on the **Sales.B2B.Order.Api**, **Order.Management.Api**, and **Organizations.Api**.

  **Affected artifacts:**
  - API: `Sales.B2B.Reports.Api`
    - Método: `POST /api/v1/orders/reports/payments`

### Updated
- Updated the Reaccommodation Report on the **Sales.B2B.Reports.Api** to no longer include GDS or Group bookings, returning only reservations within the B2B context.

  **Affected artifacts:**
  - API: `Sales.B2B.Reports.Api`

- Fixed the monetary values returned in the Sales Report on the **Sales.B2B.Reports.Api**, which were being displayed without the correct decimal places; added the organization code and organization name fields and reorganized the field display order.

  **Affected artifacts:**
  - API: `Sales.B2B.Reports.Api`

- Fixed the Segment Report search on the **Sales.B2B.Reports.Api** to consider all agents within the requesting agency, rather than only the agent who generated the request; added the booking creation date field and reorganized the field display order.

  **Affected artifacts:**
  - API: `Sales.B2B.Reports.Api`

- Changed the organization lookup permission on the **Sales.B2B.Organizations.Api**, allowing internal integrations to retrieve organization data without requiring a link to a commercial group.

  **Affected artifacts:**
  - API: `Sales.B2B.Organizations.Api`
    - Method: `GET api/private/v1/organizations/{organizationCode}`

- Fixed the passenger name change verification response on the **Sales.B2B.Order.Passengers.Api**, so it now correctly indicates which passengers have already had their name changed on bookings with multiple travelers.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Method: `PATCH api/v1/order/{recordLocator}/passengers/{passengerKey}/name`
    - Method: `PATCH api/v1/order/{recordLocator}/passengers/name/confirm`

- Excluded bookings created by Portal Grupos from the booking search (SearchBy) on the **Sales.B2B.Order.Management.Api**, keeping only bookings within the B2B context in the results.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Management.Api`
    - Method: `SearchBy`

- Made the IROP contact (IropContact) mandatory on the **Sales.B2B.Order.Api**, with the phone number now provided as three separate fields (country code, area code, and number).

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Method: `PUT api/v1/order/{recordLocator}/passengers/{passengerKey}`
  - API: `Sales.B2B.Order.Management.Api`
    - Method: `PATCH api/v1/order/{recordLocator}/contact`
  - API: `Sales.B2B.Organizations.Api`
    - Method: `POST api/v1/organizations/{organizationCode}/users`
    - Method: `POST api/v1/organizations/parent/{organizationCode}`

- Added unruly passenger validation to the **Sales.B2B.Order.Api** and **Sales.B2B.Order.Management.Api**, preventing reservations containing this type of passenger from being confirmed through checkout. For passengers with **BR** nationality, providing a **CPF** document will be mandatory. This validation is independent of the existing BPE blocking rules and will apply exclusively to 100% domestic flights. International flights or itineraries involving an international connection will not be subject to this validation.
- Adjusted document validations when creating a reservation: removed the mandatory block tied to BPe, keeping only the travel document validation required by Resolution 800, based on the passenger's nationality. Also changed the contact's GovId validation, which now only checks whether the field was filled in, regardless of country or nationality, automatically validating the format as a CPF (11 characters) or CNPJ (14 characters) when applicable.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Api`
    - Method: `POST /sales/b2b/order/api/v1/order`

- Changed the passenger travel document nationality validation, replacing the `issuingCountry` field with `birthCountry`, correctly reflecting that the information represents the passenger's country of birth.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Method: `PUT /api/v1/order/{recordLocator}/passengers/{passengerKey}`
    - Method: `PATCH /api/v1/order/{recordLocator}/passengers/:passengerKey`
  - API: `Sales.B2B.Order.Payments.Api`
    - Method: `POST /api/v1/order/payments`

- Removed the nationality validation based on the `country` field of the Customer contact's address when creating a reservation, keeping only the requirement to fill in the GovId.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Method: `POST /api/v1/order/payments`

- Removed the CPF requirement for foreign passengers residing in Brazil, allowing the Customer contact to be registered with valid documents from their country of origin; Brazilian passengers continue to follow the current rules. Also expanded the fields accepted when updating the Customer contact, including company name and full address (line 1, line 2, state, city, and postal code).

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Management.Api`
    - Method: `POST /api/v1/order/{recordLocator}/contact/customer`
    - Method: `PATCH /api/v1/order/{recordLocator}/contact`

[Link to previous versions](/docs/en-us/change-log/readme.history.md)
