# Complete Changelog

## [1.11.0] - 09/12/2024

### Updated
- Increase in the timeout of Apis.
- Cleaning the state after the division of the order.
- Validation of special characters for the fields "first", "middle" and "last" in the creation and modification of the order.

## [1.10.0] - 13/08/2024

### Added
- Methods for get and checkout of group order.
- Added new error messages for locked credit cards.

### Updated
- Adjust the AirSearch ordering for flights with stopover and connection.
- Permission to access the reports methods for agents with the FinancialAgent profile.

## [1.9.0] - 16/07/2024

### Added
- Flow for removing the TAIC10 promocode if the payment with the Tudo Azul card is declined.
- Method for adding promocode to already created orders on hold.

### Updated
- Permission to access the reports methods for agents with the WebServiceAgent profile.
- Returning imported date information in the retrieve reaccommodations method.
- Indication that the order is in payment quarantine in the retrieve order methods.
- Return of the refund fee amount to be applied in the Calculate v2.

## [1.8.0] - 28/06/2024

### Added
- CodeShare orders record locators informations

### Updated
- Adjustments and restrictions on the availability of baggage and services on CodeShare segments
- Block unaccompanied minor passengers on CodeShare orders
- Block creation of CodeShare orders with segments with a departure date less than 24 hours away

## [1.7.0] - 17/06/2024

### Added
- New payment refund option in order checkout
- Search for the credit available to an organization without the need to previously retrieve an order
- Added "No Show" fares in the get fares method
- Return of cabin type information when performing AirSerch, Quote and get Order

### Updated
- Adjustment to the Tudo Azul card discount, now the discount is only applied to fully paid orders
- Return the informed card identification in the payment and installments methods
- Return information about expiration date and the card holder's name in the payments object in get order methods

### Fixed
- Error when informing a passport as travel document for infants in order creation

## [1.6.1] - 16/05/2024

### Added
- New method to search for lowfares

## [1.6.0] - 04/25/2024

### Added
- New method to search for children record locators
- Show promotional discounts applied on charge objects

### Fixed
- Paginations of reaccommodation summaries
- Adjustment in the mapping of agency phone numbers in the generated order contacts

## [1.5.0] - 02/27/2024

### Added
- Shopping
    - Fix the property "productClass" on Offer Quote method.
- Payments
    - Remove GovId as mandatory field for credit card payments with BRL currency
    - Adjusts on interests fee
- Reaccommodations
    - New queues mapped
- Keep Alive
    - New error messages
    - Dynamic calculation of keep alive time according to Navitaire iddleTimeout

## [1.4.0] - 01/31/2024

### Added
- Payments with interest
- Flow improvements
    - Division
        - Hold
        - Cancellation
    - Itaucard discount
        - Including discount on fuel tax
    - Performance of the authentication flow
    - TudoAzul Categorization
        - Fix of names with namematch
    - Handling error messages
        - Fare sold out
        - Agency account blocked
    - Hold calculation correction
    - Adjust Password Regex
    - Economy Prime seats
    - API documentation

## [1.3.0] - 01/04/2024

### Added

- Releasing reaccommodation features

## [1.2.0] - 12/26/2023

### Added

- Releasing report features
	- Payments reports
	- Sales reports
	- Segments reports

## [1.1.0] - 11/16/2023

### Added

- Releasing passagers management features
	- Add an infant in already created orders
	- Customer program categorization (TudoAzul) in already created orders

- Releasing asynchronous sells of ancillaries features

- General improvments of seat map
	- Mapping SkySofa
	- Mapping emergency exits

- General improvments on cancel and change flows
	- Block get from state with pending calculate
	- Block DUFEE manual adjustment with pending calculate
	- Block order division with changed journeys
	
- Improvments on agent management
	- User Search
	- Extra informations on Authentication response

## [1.0.1] - 09/28/2023

### Updated

- General improvments on Loyality API
	- New Comarch API

## [1.0.0] - 08/01/2023

### Added

- Releasing initial version from middleware B2B in production environment
