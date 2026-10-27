# Changelog

## [1.26.0] - YYYY/MM/DD

### Added
- Added the _GET InstallmentsCalculate_ method (V1) on the **Sales.B2B.Order.Payments.Api**, allowing installment conditions to be simulated without a previously created booking (Order in State), using only the data provided in the request (amount, taxes and, optionally, the card BIN and domestic/international market). When the BIN is provided, the installment plan matching the card is returned; when neither BIN nor market is provided, all four installment options are returned (Azul and Regular, domestic and international). The returned values are a preliminary estimate and may change after the booking is created and validated; for final values, the _GET Installments_ method must be used, which remains available without changes. No installment options are returned for currencies other than BRL.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Method: `GET /api/v1/order/payments/installmentscalculate`

- Added a method to change the data of Infant passengers on the **Sales.B2B.Order.Passengers.Api**, extending to Infants the changes already allowed for adult and child passengers. The change covers the Infant's nationality, gender, date of birth, and travel documents.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Method: `PATCH /api/v1/order/{recordLocator}/passengers/{Key}/infant`

- Added the _OrganizationGroup_ search criterion to the booking search on the **Sales.B2B.Order.Management.Api**, allowing bookings to be searched by organizational group. Also fixed the organization and agent information sent in Navitaire queries, ensuring the search runs in the context of the queried organization, and removed the requirement for the _FirstName_ field. Existing search criteria remain unchanged.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Management.Api`
    - Method: `GET /api/v1/orders/searchBy/:type`

### Updated
- Fixed the organizational credits lookup on the **Sales.B2B.Order.Payments.Api**, which was interrupted when the booking had a document type not mapped by the B2B middleware. These bookings are now processed normally, following the same behavior already adopted on the **Sales.B2B.Order.Management.Api**; already mapped documents continue to be processed without changes.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Method: `GET /api/v1/order/payments/credits/:type`

- Fixed the discrepancy in the reaccommodation information returned by the _Get Summary_ and _Get Summary Details_ methods on the **Sales.B2B.Order.Reaccommodation.Api**, ensuring that totals are consistent with the details and that segments actually changed are returned as reaccommodated.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Reaccommodation.Api`
    - Method: `GET /api/v1/orders/reaccommodations/summary`
    - Method: `GET /api/v1/orders/reaccommodations/summary/Details`

- Included the request's UserAgent in the comment automatically recorded when a booking is created through the **Sales.B2B.Order.Api**, making it possible to identify the channel, application, or integration responsible for creating the booking. When the UserAgent is not sent, the comment records "Não informado" (not provided), without impacting booking creation.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Api`

- Updated the documentation of the _MethodCode_ field on the **Sales.B2B.Order.Payments.Api** and the _methodCode_ attribute on the **Sales.B2B.Order.Management.Api**, detailing the meaning of each payment method code: AG (Agency Account), CF (Credit File), AX (American Express), VI (Visa), MC (MasterCard), DI (Diners Club), HP (Hipercard), and EL (Elo). Documentation-only change, with no functional impact.

  **Affected artifacts:**
  - API: `Sales.B2B.Order.Payments.Api`
  - API: `Sales.B2B.Order.Management.Api`

[Link to previous versions](/docs/en-us/change-log/readme.history.md)
