# Issue Opening Template

To open issues, in order to facilitate the analysis of the reported problem and receive faster and more assertive feedback, it is essential that the template is followed.

Here you can find the [Template](./issue-template.md) to copy and use when opening the issue, and below is the description of each point.

## Problem description

Describe here clearly and concisely the problem encountered with the middleware.

## Steps to Reproduce

List the steps required to reproduce the issue here. Include information such as API URL, parameters used, as long as they do not contain sensitive information, among other information.

1. Execute a POST to the 'api/v1/b2b/auth' API.
2. Execute a POST to the API 'api/v1/b2b/rotaexample'.
3. In the POST call to the API 'api/v1/b2b/rotaexemlo' use the following payload:
`{origin: "SDU", destination: "VCP", firstName: "*****"}`.
4. After this, the error "500 - Unexpected internal error" is returned.

__Always be careful to remove any information that is private or sensitive.__
Example of information that __shouldnot__ be included in the issue under any circumstances:

- Subscription Keys.
- Names and personal documents.
- Credit Card Information.
- Any information that violates the LGPD.

__Note:__ If any additional information is necessary, it will be requested in the issue, if the information is of a private nature, it will be requested via email to the issue author.

Examples with common routes and problems:

Example 1:

1. Execute a POST to the 'api/v1/token' API.
2. Execute a POST to the 'api/v1/authenticate' API.
3. In the POST call to the 'api/v1/airSearch' API use the following payload:
`{
     "passengers": [
         {
             "type": "ADT",
             "count": 1
         }
     ],
     "journeys": [
         {
             "origin": "POA",
             "destination": "VCP",
             "departure": "2023-09-20T00:00:00"
         }
     ],
     "criteria": {
         "promotionCode": "",
         "baggageAllowance": "All",
         "directFlightsOnly": false
     }
}`.
4. After this, the error "502 - Bad Gateway" with internal code "Navitaire.Request.Failed" is returned.

Example 2:

1. Execute a POST to the 'api/v1/token' API.
2. Execute a POST to the 'api/v1/authenticate' API.
3. Execute a POST to the 'api/v1/airSearch' API using the following payload:
`{
     "passengers": [
         {
             "type": "ADT",
             "count": 1
         }
     ],
     "journeys": [
         {
             "origin": "MVD",
             "destination": "BEL",
             "departure": "2023-09-30T00:00:00"
         }
     ],
     "criteria": {
         "promotionCode": "",
         "baggageAllowance": "All",
         "directFlightsOnly": false
     }
}`.
4. In the API POST call 'api/v1/order' using in the payload with an adult for a one-way flight.
5. After this, the error "502 - Bad Gateway" with internal code "Integration.InvalidFare" is returned.

Example 3:

1. Execute a POST to the 'api/v1/token' API.
2. Execute a POST to the 'api/v1/authenticate' API.
3. Execute a POST to the 'api/v1/airSearch' API using the following payload:
`{
     "passengers": [
         {
             "type": "ADT",
             "count": 2
         }
     ],
     "journeys": [
         {
             "origin": "MVD",
             "destination": "SDU",
             "departure": "2023-09-21T00:00:00"
         },
                 {
             "origin": "SDU",
             "destination": "MVD",
             "departure": "2023-09-29T00:00:00"
         }
     ],
     "criteria": {
         "promotionCode": "",
         "baggageAllowance": "All",
         "directFlightsOnly": false
     }
}`.
4. Execute a POST to the 'api/v1/order' API using the payload with two adults for a round trip flight.
5. Execute a GET on the 'api/v1/order' API.
6. After this, the error "502 - Bad Gateway" with internal code "RequestFailed.Unexpected" is returned.

## Environment

- Environment used: Stage or Production.
- Source System Language: Python, PHP, C#, etc.

## Additional Information

Add any additional information that might be relevant to understanding the problem, such as error messages, logs, or other details.

## Steps already tried to solve the problem

List any steps you have already tried to resolve the problem, if applicable.

## Additional Context

Provide any additional context you think is relevant to the issue.

---

Thanks for reporting this issue. We will review it and respond as soon as possible. If necessary, we will contact you to request more information.

Thanks for your collaboration!

Support Team.