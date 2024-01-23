# Frequently Asked Questions (FAQ)

Here are some frequently asked questions about using B2B Middleware:

## 1. How can I start selling Azul tickets?

To start integrating with our Middleware and making our flights available at your agency, contact our commercial department to register your travel agency

## 2. How can I get access to the Middleware APIs?

To gain access to the Middleware APIs, you must first follow the guidance described in the previous topic, and after that, simply follow the steps described in the document [How to Request a Subscription Key](/docs/en-us/subscription-key /readme.md).

## 3. How can I sell airline tickets?

To sell airline tickets, you must use the Order API. For more detailed information on how to create a sales flow, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 4. Can I cancel an airline reservation?

Yes, it is possible to cancel a reservation.
To cancel airline tickets, you must use the Order Management API. For more detailed information on how to create a cancellation flow, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 5. How can I add additional services to a passenger's reservation?

To add additional services you need to use the Order Services API, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 6. How can I get information about available flights?

You can obtain flight details using the Shopping API, check the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 7. How to perform authentication on the Middleware?

You can perform authentication by first obtaining the token from the Authentication API. After obtaining the token, you can use it to authenticate through the User API.

## 8. How do I change the point of sale with my agent?

You can change the logged in user's point of sale through the User API.

## 9. How to book a reserved seat for a passenger?

To add seats you need to use the Order Seats API, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 10. How to add baggage to a passenger's reservation?

To add baggage you need to use the Order Services API, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 11. Can I add sections to a reservation?

Yes, it is possible to add sections to a reservation.
To add sections, you must use the Order Management API. For more detailed information on how to create a snippet addition flow, check out the [Basic Flows](/docs/en-us/postman/README.md) documentation.

## 12. Can I cancel sections of a reservation?

Yes, it is possible to cancel parts of a reservation.
To cancel segments, you must use the Order Management API. For more detailed information on how to create a section cancellation flow, check out the documentation [Basic Flows](/docs/en-us/postman/README.md).

## 13. What do the codes mean: AG, CF, AX, VI, MC, DI, HP, EL and TP, described in swagger's methodCode in the POST Order/payments v1 method endpoint?

The meanings are:
AG = how much value the agency has as a billing limit next to blue.
CS = shell credit, when the customer has credit for the value of the Reservation.
CF = faithful credit, when the credit is released to the customer for use on TudoAzul or for creating a new Reservation or even for use as a refund.
AX = AmericanExpress
VI = VISA
MC = MASTER
DI = DINNERS
HP = HiperCard
EL = ELO
TP = UATP, which is a virtual card that is only valid on airlines

## 14. What is the Authentication/Token service for and how long does it last per session?

The Authentication service is responsible for authenticating and identifying the systemic user of the B2B Middleware.
Obtaining the token through the Authentication service is mandatory at the beginning of each B2B Middleware session, and a token generated for a travel agent must be used until the end of that same agent's session.
The token will expire after 15 minutes of inactivity. After this time, it will be necessary to request a new token, otherwise the methods called will return the HTTP status 401: Unauthorized.

## 15. What is the validation and Go Live process?
 
The validation and go live process is detailed in the link [Process for using the Middleware in production](/docs/en-us/start-production-process/readme.md).

## 16. What should I do when I get the error: HTTP 409: Conflict, "message": "An agent is already authenticated."

In this situation, the variable must be sent in the header: User_Agent with the name: salesb2b/"Name_da_Agência", with the name of the agency being the name of your company. For more details, access the link [UsersAgent Validation](/README.en.md).


## 17. What should I do when I get the error: HTTP 409: Conflict, "message": "An agent is already authenticated."

In this situation, the variable must be sent in the header: User_Agent with the name: salesb2b/"Name_da_Agencia"

## 18. How to terminate the use of a token in use?
Answer: Just execute a Delete token in the authentication api.


## 19. How to change the user using the same token? Should we use /api/v1/organizations/:organizationCode/users/:userKey/password/reset?
Answer: Just perform a Delete logout in the users API.


## 20. What are the differences between Primary Key and Secondary Key (We are using only Primary Key in Postman)
Answer: There is no difference between the functionality of the primary and secondary key, both are created solely for security reasons, and if it is necessary to block one, the other can be used automatically. In fact, the security team suggests updating the subscription Keys used every six months.


## 21. Is there an available routes method? Should I consider the stations method for this query?
Answer: Currently the information must be consulted through the API /api/v1/stations, in the future a route method will be developed.


---

We hope these FAQs have helped clarify some common questions about using the Middleware to integrate with Navitaire. If you have additional questions or require more information, please don't hesitate to contact our support team.

Happy coding! 😊✈️