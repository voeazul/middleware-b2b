# Documentation of APIs and Reservation Flow

Welcome to the Middleware APIs centralized documentation and reservation flow guide! Here you will find information about the available APIs and how to perform reservation, change and other main flows.

## Security

Due to security validation, to complement the API access, it will be necessary to send a header User-Agent, with the value salesb2b/agency_name in addition to the subscription key header in STG and PRD environment. Example: - salesb2b/xpto_travels.

## API Summary

Here is the list of available APIs and a brief description of the available APIs:

| API | Description |
|-------|---------------------------------------------------|
| [Authentication](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Authentication.Api) | The Authentication service is responsible for authenticating the B2B Middleware systemic user. Obtaining the token through the Authentication service is mandatory at the beginning of each B2B Middleware session. |
| [User](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.User.Api) | The User service is responsible for managing travel agent information logged into the B2B Middleware. |
| [Resources](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Resources.Api) | The Resources service is responsible for providing methods to query information and details of the various resources used in the B2B Middleware flows. |
| [Shopping](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Shopping.Api) | The Shopping service is responsible for providing flight offer search methods through the B2B Middleware and providing all information regarding available offers. |
| [Organization](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Organizations.Api) | The Organizations service is responsible for providing relevant information to agencies (organizations) that use B2B Middleware. |
| [Order](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Api) | The Order service provides the methods responsible for creating, consulting and managing reservations made through the B2B Middleware. |
| [Order Management](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Management.Api) | The OrderManagement service is responsible for providing methods via B2B Middleware to manage reservation resources. |
| [Order Group Management](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Group.Management.Api) | The OrderGroupManagement service is responsible for providing methods via B2B Middleware to query and manage group reservations. |
| [Order Passengers](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Passengers.Api) | The OrderPassengers service is responsible for providing methods via B2B Middleware to manage reservation passengers|
| [Order Group Passengers](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Passengers.Api) | The OrderPassengers service is responsible for providing methods via B2B Middleware to manage passengers of group reservations. |
| [Order Payments](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Payments.Api) | The OrderPayments service is responsible for adding, consulting and managing all payments related to reservations made through the B2B Middleware. |
| [Order Reaccommodation](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Reaccommodation.Api) | The OrderReaccommodation service is responsible for providing methods via B2B Middleware to manage reservation re-accommodations.|
| [Order Seats](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Seats.Api) | The OrderSeats service is responsible for providing methods via B2B Middleware to manage seat map resources. |
| [Order Services](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Services.Api) | This service offers methods that handle requests for special services, luggage and assistance. |
| [Reports](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Reports.Api) | The Reports service is responsible for providing reports through the B2B Middleware. |

## How to Make a Reservation Flow

For detailed information about reservation flows, which APIs to call for reservation change, creation and manipulation, see some flow examples from our postman in the [Basic Flows](/docs/en-us/postman/README.md) section.

## List of API Error Codes

If you encounter any errors when using the APIs, see the [API Error Code List](/docs/pt-br/apis-doc/errors-code.md) for information about error codes, HTTP response and corresponding error messages.

---

Explore the topics above for more information about APIs and booking flows. If you have any questions or suggestions, don't hesitate to contact us!

Happy coding! 😊
