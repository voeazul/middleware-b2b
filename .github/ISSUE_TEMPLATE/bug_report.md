---
name: Bug report
about: Create a report to help us improve
title: ''
labels: analyzing
assignees: ''

---

**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
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

__Always be careful to remove any information that is private or sensitive.__
Example of information that __shouldnot__ be included in the issue under any circumstances:

- Subscription Keys.
- Names and personal documents.
- Credit Card Information.
- Any information that violates the LGPD.

__Note:__ If any additional information is necessary, it will be requested in the issue, if the information is of a private nature, it will be requested via email to the issue author.

**Expected behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Environment**

Environment used: Stage or Production.
Source System Language: Python, PHP, C#, etc.

**Additional context**
Add any other context about the problem here.
