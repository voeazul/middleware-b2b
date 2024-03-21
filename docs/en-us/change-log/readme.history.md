# Complete Changelog

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
