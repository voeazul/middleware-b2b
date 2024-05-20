# API Versioning Support

## Overview
Our Middleware supports versioning to ensure backwards compatibility and allow controlled API evolution. In this documentation, we will provide information about how we handle API versioning, how long we maintain support for previous versions and how we notify users about updates and changes.

## Route Versioning
To ensure the stability and compatibility of APIs, we follow a route versioning scheme. Each API route is versioned using the version number as part of the URI.

- Route version example: `/api/v1/endpoint`

The version number in the route indicates the specific version of that route. As the API is updated and new versions of routes are introduced, the version number in the route may be incremented.

## Route Version Number Changes
The version number on a route can change on the following occasions:

1. **Incompatible Changes**: When changes are made that are not compatible with the previous version of the route. This may include breaking changes to the structure of the response, required or optional parameters, or underlying logic. These changes may affect the route's integration with the previous version and require client-side updates.

2. **Addition of Features**: When new features are added to the route without changing compatibility with the previous version. This often includes introducing new optional parameters, additional responses, or extra functionality that does not affect the route's existing logic. Customers who wish to use these new features can upgrade to the latest version of the route.

3. **Bug Fixes**: When bug fixes are made to the route, without changing the main functionality or compatibility with the previous version. These fixes are intended to resolve specific issues and do not require client-side changes.

## Support for Previous Versions
We guarantee support for previous versions for a set period of time, allowing users to transition to the latest versions. The length of support for a specific version may vary, but in general, we follow a policy of maintaining support for __12 months__.

## APIs with New Versions
|Method                                                                                                    |API                              |Version |Support Deadline         |
|----------------------------------------------------------------------------------------------------------|---------------------------------|--------|-------------------------|
|`POST` `/api/v1/airSearch`                                                                                |Sales.B2B.Shopping.Api           | 1.0    | 25/04/2025              |
|`POST` `/api/v1/quote`                                                                                    |Sales.B2B.Shopping.Api           | 1.0    | 25/04/2025              |
|`GET` `/api/v1/order`                                                                                     |Sales.B2B.Order.Api              | 1.0    | 25/04/2025              |
|`GET` `/api/v1/order`                                                                                     |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`GET` `/api/v1/order/{recordLocator}`                                                                     |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`POST` `/api/v1/order/{recordLocator}/checkout`                                                           |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`POST` `/api/v1/order/{recordLocator}/calculate`                                                          |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`PUT` `/api/v1/order/{recordLocator}/fees/organization`                                                   |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`POST` `/api/v1/order/{recordLocator}/journeys`                                                           |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`DELETE` `/api/v1/order/{recordLocator}/journeys/{journeyKey}`                                            |Sales.B2B.Order.Management.Api   | 1.0    | 21/05/2025              |
|`POST` `/api/v1/order/segments/{segmentKey}/passengers/{passengerKey}/seats/{unitKey}`                    |Sales.B2B.Order.Seats.Api        | 1.0    | 21/05/2025              |
|`DELETE` `/api/v1/order/segments/{segmentKey}/passengers/{passengerKey}/seats/{unitKey}`                  |Sales.B2B.Order.Seats.Api        | 1.0    | 21/05/2025              |
|`PUT` `/api/v1/order/{recordLocator}/journeys/{journeyKey}/passengers/{passengerKey}/baggage`             |Sales.B2B.Order.Services.Api     | 1.0    | 21/05/2025              |
|`DELETE` `/api/v1/order/{recordLocator}/journeys/{journeyKey}/passengers/{passengerKey}/baggage`          |Sales.B2B.Order.Services.Api     | 1.0    | 21/05/2025              |
|`POST` `/api/v1/order/{recordLocator}/journeys/{journeyKey}/passengers/{passengerKey}/services`           |Sales.B2B.Order.Services.Api     | 1.0    | 21/05/2025              |
|`DELETE` `/api/v1/order/{recordLocator}/journeys/{journeyKey}/passengers/{passengerKey}/services/{code}`  |Sales.B2B.Order.Services.Api     | 1.0    | 21/05/2025              |

After the support deadline for a version, we strongly recommend that users migrate to the latest version to continue receiving support and enjoy of the latest functionalities.

## Version Notifications
When a new version of the API is released or an old version reaches its support end date, we will notify users via email and our Github account. Email notifications will be sent to the email address associated with the API subscription key and the agency's primary contact.

Notifications will include information about the new version available, the changes and improvements introduced, and the support end date for previous versions. We will also provide additional guidance and resources to help users migrate to the latest version.

## Contact Us
If you have questions about API versioning or require additional support, please contact our technical support team through the following channels:

- Github
- Email: support.b2b@voeazul.com.br

We are ready to help you with any questions or queries related to API versions.
