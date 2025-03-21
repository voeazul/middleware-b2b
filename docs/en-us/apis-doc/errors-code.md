# Error Codes and Messages

Our Middleware has several rules and procedures to guarantee the integrity of the flow. All HTTP response codes, possible error codes and their respective error messages are mapped below:

## General Errors

|	 HTTP Code       	|	 Internal Code   	|	 Error Message                               	|
|	 ----------------- 	|	 -------------- 	|	 ---------------------------------------------- 	|
| 400 Bad Request | Agent.NoOrganizationGroup | The Agent must be in a organization group when 'OrderCriteria.Type' is equal to 'OrganizationGroup'. |
| 400 Bad Request | Agent.NotAuthorized | Agent is not allowed to assign seat. |
| 400 Bad Request | AgentOrder.NotAuthorized | Agent is not authorized to commit order with invalid price status without requesting to override restrictions. |
| 400 Bad Request | Alerts.Authentication.Invalid | Invalid Authentication. |
| 400 Bad Request | AlreadyExists.Username | The 'Username' entered already exists in this or another organization. |
| 400 Bad Request | AuthorizationFailed.Credentials | Username or password is incorrect. |
| 400 Bad Request | B2b.OrderManagementRequest.Failed | The request failed. |
| 400 Bad Request | B2bHttp.CustomBadRequest | The token is invalid. |
| 400 Bad Request | B2b.Request.Failed | The request failed. |
| 400 Bad Request | B2b.User.Failed | The request failed. |
| 400 Bad Request | BirthCountry.NotFound | The 'BirthCountry' was not found. |
| 400 Bad Request | Change.Hold.Information | The hold date has changed from {0} to {1}. |
| 400 Bad Request | Change.Hold.NotAllowed | Unable to update hold date. Check the given date. |
| 400 Bad Request | ChangeCancel.NotFound | No ChangeCancel session found. |
| 400 Bad Request | Checkout.V2.Blocked | This method is not compatible with retrieve order in V1. |
| 400 Bad Request | Codeshare.Departure.LessThan24Hours | It is not allowed to create an order with codeshare when the journey departure date is less than 24 hours. |
| 400 Bad Request | Contact.AddressLine.Required | The 'AddressLine1' is required. |
| 400 Bad Request | Contact.Duplicate | The 'TypeCode' is duplicated. |
| 400 Bad Request | Contact.LastName.Required | The 'LastNameRequired' is required. |
| 400 Bad Request | CustomerProgram.NotAllowed | This user profile cannot categorize customers. |
| 400 Bad Request | CustomProgram.NotMatch | Passenger name does not match within informed Customer Program. |
| 400 Bad Request | Dates.Range.OverMaximum | The difference in days between 'DepartureBegin' and 'DepartureEnd' cannot be greater than {0} days. |
| 400 Bad Request | DiscountPayment.TudoAzul | A discount have been applied to your order for using a TudoAzul card. |
| 400 Bad Request | Email.NotFound | User has no email assigned. |
| 400 Bad Request | FlexibleDays.Disabled | Unable to get flexible days because this feature is disabled. |
| 400 Bad Request | Error.OverrideDuFee | Fee override is higher than the maximum amount allowed {0}%. | 
| 400 Bad Request | Infant.NotNull | There is already a infant in the order for this passenger. |
| 400 Bad Request | Infant.Request.Failed | There was an error sending the passenger document. |
| 400 Bad Request | Integration.EnterpriseStation | An error occurred while returning the stations. |
| 400 Bad Request | Integration.Error | ServiceBus connection error! |
| 400 Bad Request | InvalidField.Account | The 'Account' is invalid. |
| 400 Bad Request | InvalidField.Account.Length | The 'Account' has a maximum length of 16 characters. |
| 400 Bad Request | InvalidField.Address.City | The 'Address.City' has a maximum of 32 characters. |
| 400 Bad Request | InvalidField.Address.Country | The 'Address.CountryCode' has a maximum of 2 characters. |
| 400 Bad Request | InvalidField.Address.LineOne | The 'Address.LineOne' has a maximum of 128 characters. |
| 400 Bad Request | InvalidField.Address.LineThree | The 'Address.LineThree' has a maximum of 128 characters. |
| 400 Bad Request | InvalidField.Address.LineTwo | The 'Address.LineTwo' has a maximum of 128 characters. |
| 400 Bad Request | InvalidField.Address.PostalCode | The 'Address.PostalCode' has a maximum of 10 characters. |
| 400 Bad Request | InvalidField.Address.ProvinceState | The 'Address.ProvinceState' has a maximum of 3 characters. |
| 400 Bad Request | InvalidField.Amount | The 'Amount' value must be equal or greater than zero. |
| 400 Bad Request | InvalidField.AssistanceArray | The minimum count of 'Assistances' array is 1. |
| 400 Bad Request | InvalidField.AssistanceCode | The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. |
| 400 Bad Request | InvalidField.AssistancesCount | The 'Assistances.Count' must be greather than 0. |
| 400 Bad Request | InvalidField.Authorization | The 'PaymentCriteria.Authorization' has a maximum of 20 characters. |
| 400 Bad Request | InvalidField.BaggageAllowance | The 'BaggageAllowance' must be a valid Enum. |
| 400 Bad Request | InvalidField.Bin | The 'BIN' is not a valid number. |
| 400 Bad Request | InvalidField.Bin.Length | The 'BIN' must be of 6 characters. |
| 400 Bad Request | InvalidField.CardEnd | The 'PaymentCriteria.CardEnd' has a maximum of 4 characters. |
| 400 Bad Request | InvalidField.ChangeType | The 'ChangeType' must be a valid Enum. |
| 400 Bad Request | InvalidField.Code | The 'Code' must have a maximum length of 10 characters. |
| 400 Bad Request | InvalidField.Codes | The minimum count of 'Codes' array is 1. |
| 400 Bad Request | InvalidField.Contact.AddressCity | The 'Contact.Address.City' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.Contact.CompanyName | The 'Contact.CompanyName' has a maximum of 64 characters. |
| 400 Bad Request | InvalidField.Contact.Email | The 'Contact.Email' is invalid. |
| 400 Bad Request | InvalidField.Contact.FirstName | The 'Name.First' has a maximum of 32 characters. |
| 400 Bad Request | InvalidField.Contact.LastName | The 'Name.Last' has a maximum of 32 characters. |
| 400 Bad Request | InvalidField.ContactAddress.LineOne | The 'Contact.Address.LineOne' has a maximum length 52 characters. |
| 400 Bad Request | InvalidField.ContactAddress.LineThree | The 'Contact.Address.LineThree' has a maximum length 52 characters. |
| 400 Bad Request | InvalidField.ContactAddress.LineTwo | The 'Contact.Address.LineTwo' has a maximum length 52 characters. |
| 400 Bad Request | InvalidField.ContactAddress.PostalCode | The 'Contact.Address.PostalCode' has a maximum length 10 characters. |
| 400 Bad Request | InvalidField.ContactAddress.ProviceState | The 'Contact.Address.ProvinceState' has a maximum length 3 characters. |
| 400 Bad Request | InvalidField.ContactAddressLineCountry | The 'Contact.Address.Country' has a maximum length 2 characters. |
| 400 Bad Request | InvalidField.ContactName.First | The 'Contact.Name.First' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Last | The 'Contact.Name.Last' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Middle | The 'Contact.Name.Middle' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Suffix | The 'Contact.Name.Suffix' must be a valid enum. |
| 400 Bad Request | InvalidField.ContactNameT.itle | The 'Contact.Name.Title' must be a valid enum. |
| 400 Bad Request | InvalidField.ContactPhones.Number | The 'Contact.Phones.Number' has a maximum length 20 characters. |
| 400 Bad Request | InvalidField.ContactPhones.Type | The 'Contact.Phones.Type' must be a valid enum. |
| 400 Bad Request | InvalidField.Count.Infant | The 'ADT' type passenger count must be greater than 'INF' type passenger count. |
| 400 Bad Request | InvalidField.Count.OverMaximum | The sum of 'Passengers.Count' of type ADT and CHD must be less than or equal to {0} passengers. |
| 400 Bad Request | InvalidField.Count.UnderMinimum | The minimum value of 'Passengers.Count' is 1. |
| 400 Bad Request | InvalidField.CountryCode | The 'CountryCode' must have 2 characters. |
| 400 Bad Request | InvalidField.CreatedBy | The 'OrderCriteria.CreatedBy' has a maximum of 20 characters. |
| 400 Bad Request | InvalidField.CreditAmount.Empty | The 'CreditAmount' value must be greater than zero. |
| 400 Bad Request | InvalidField.CriteriaType | The 'CriteriaType' must be an valid Enum. |
| 400 Bad Request | InvalidField.customerProgram.number | Alphabetic characters are not allowed. |
| 400 Bad Request | InvalidField.CustomerProgram.Number | The 'Passengers.CustomerProgram.Number' has a maximum lenght of 20 characters. |
| 400 Bad Request | InvalidField.DateOfBirth | The agent must be at least {0} years old. |
| 400 Bad Request | InvalidField.Day | the 'PeriodCriteria.Day' can only be informed if the 'PeriodCriteria.Type' is equal to 'Day'. |
| 400 Bad Request | InvalidField.Departure | The 'Departure' must be greater than or equal today's date. |
| 400 Bad Request | InvalidField.DepartureBegin | The 'DepartureBegin' must be greater than today's date. |
| 400 Bad Request | InvalidField.DepartureEnd | The 'DepartureBegin' must be greater than 'DepartureEnd'. |
| 400 Bad Request | InvalidField.Destination.Length | The 'Destination' station code has a maximum length of 3 characters. |
| 400 Bad Request | InvalidField.Email | The 'Email' provided is invalid. |
| 400 Bad Request | InvalidField.EquipmentCode | The 'EquipmentCode' must have a maximum of 3 characters. |
| 400 Bad Request | InvalidField.ExpirationDate | Invalid credit card expiration date. |
| 400 Bad Request | InvalidField.ExpirationMonth | The 'ExpirationMonth' must be empty when MethodCode is {0} |
| 400 Bad Request | InvalidField.ExpirationYear | The 'ExpirationYear' must be empty when MethodCode is {0} |
| 400 Bad Request | InvalidField.FareKey | The 'FareAvailabilityKey' is invalid! |
| 400 Bad Request | InvalidField.FeeCode | The 'FeeCode' must have a maximum of 6 characters. |
| 400 Bad Request | InvalidField.Filter | Can only be filtered by 'Username' or 'FirstName'. |
| 400 Bad Request | InvalidField.FirstName | The 'FirstName' must be a string with a maximum length of 32. |
| 400 Bad Request | InvalidField.FirstName.Length | The 'FirstName' must be a string with a maximum length of 128. |
| 400 Bad Request | InvalidField.FirstNameMatching | The 'FirstNameMatching' cannot be entered with 'Username'. |
| 400 Bad Request | InvalidField.FlexibleDays.Ahead | The minimum value of 'FlexibleDays.Ahead' is {0}. |
| 400 Bad Request | InvalidField.FlexibleDays.Behind | The minimum value of 'FlexibleDays.Behind' is {0}. |
| 400 Bad Request | InvalidField.FlightNumber | Some segments for the Journey '{0}-{1} - {2}' do not support the assistance '{3}'. Please contact the customer service to complete the special assistance process. |
| 400 Bad Request | InvalidField.Gender | The 'TravelDocuments.Gender' must be a valid Enum. |
| 400 Bad Request | InvalidField.GovId | The 'GovId' is invalid. |
| 400 Bad Request | InvalidField.GovId.Length | The 'GovId' has a maximum length of 11 characters. |
| 400 Bad Request | InvalidField.HolderName | The 'HolderName' must be empty when MethodCode is {0} |
| 400 Bad Request | InvalidField.HolderName.Length | The 'HolderName' has a maximum length of 255 characters. |
| 400 Bad Request | InvalidField.Identifier | The Identifier cannot be more than 20 digits. |
| 400 Bad Request | InvalidField.Infant.DateOfBirth | The 'Infant.DateOfBirth' is invalid. |
| 400 Bad Request | InvalidField.Infant.Nationality | The 'Infant.Nationality' has a maximum of 2 characters. |
| 400 Bad Request | InvalidField.Installments | The 'Installments' cannot be zero or null. |
| 400 Bad Request | InvalidField.IropContact.Email | The 'Passengers.IropContact.Email' has a maximum length 128 characters. |
| 400 Bad Request | InvalidField.IropContact.Mobile | The 'Passengers.IropContact.Mobile' cannot be informed when Passengers.IropContact.Refused is True. |
| 400 Bad Request | InvalidField.Jorneys.Departure | Departure of each JourneyKey must be greater than or equal to the current date. |
| 400 Bad Request | InvalidField.Journey | The Journey.Key '{0}' is duplicated. |
| 400 Bad Request | InvalidField.Journey.Key | One or more journeyKeys informed in the request does not exist for the order informed. |
| 400 Bad Request | InvalidField.Journeys | The minimum count of 'Journeys' array is 1. |
| 400 Bad Request | InvalidField.Journeys.Count | The maximum number of Journeys allowed in a order is {0}. |
| 400 Bad Request | InvalidField.Journeys.OverMaximum | The number of 'Journeys' must be less than {0}. |
| 400 Bad Request | InvalidField.Journeys.UnderMinimum | The number of 'Journeys' must be greater than {0}. |
| 400 Bad Request | InvalidField.Keys | The key '{0}' cannot be accepted. |
| 400 Bad Request | InvalidField.Keys.UnderMinimum | The number of 'Keys' must be greater than 1. |
| 400 Bad Request | InvalidField.LastName | The 'LastName' cannot be entered with 'Username'. |
| 400 Bad Request | InvalidField.LastName.Length | The 'OrganizationCode' must be a string with a maximum length of 64. |
| 400 Bad Request | InvalidField.LiableRecordLocator | The 'LiableRecordLocator' must have 6 characters. |
| 400 Bad Request | InvalidField.LiableRecordLocator | 'LiableRecordLocator' is invalid. |
| 400 Bad Request | InvalidField.Method | The 'PaymentCriteria.Method' must be a valid Enum. |
| 400 Bad Request | InvalidField.MethodCode | The 'MethodCode' must be equals to {0}, {1}. |
| 400 Bad Request | InvalidField.MethodCode.Length | The 'MethodCode' must be 2 characters. |
| 400 Bad Request | InvalidField.MiddleName | The 'MiddleName' must be a string with a maximum length of 32. |
| 400 Bad Request | InvalidField.MiddleName.Length | The 'Name.Middle' has a maximum of 32 characters. |
| 400 Bad Request | InvalidField.Month | The 'PeriodCriteria.Month' must be between 1 and 12. |
| 400 Bad Request | InvalidField.Name.First | The 'Name.First' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.Name.Last | The 'Name.Last' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.Name.Length | The 'Username' must be a string with a maximum length of 64. |
| 400 Bad Request | InvalidField.Name.Suffix | The 'Name.Sufix' must be a valid Enum. |
| 400 Bad Request | InvalidField.Name.Title | The 'Name.Title' must be a valid Enum. |
| 400 Bad Request | InvalidField.Nationality.Length | The 'Nationality' has a maximum length 2 characters. |
| 400 Bad Request | InvalidField.NewPassword | The 'NewPassword' must be different from the 'CurrentPassword'. |
| 400 Bad Request | InvalidField.NoFilter | Filter by 'Username' or 'FirstName'. |
| 400 Bad Request | InvalidField.Offers | The minimum count of 'Offers' array is 1. |
| 400 Bad Request | InvalidField.Offers.CurrentJourneyKey | One or more CurrentJourneyKey informed in the request does not exist for the order informed. |
| 400 Bad Request | InvalidField.Offers.OverMaximum | The maximum count of 'offer' array is 4 |
| 400 Bad Request | InvalidField.Offers.UnderMinimum | The minimum count of 'offer' array is 1. |
| 400 Bad Request | InvalidField.OrderCriteria.Status | The 'OrderCriteria.Status' must be a valid Enum. |
| 400 Bad Request | InvalidField.OrderCriteria.Type | The 'OrderCriteria.Type' must be a valid Enum. |
| 400 Bad Request | InvalidField.OrganizationCode | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. |
| 400 Bad Request | InvalidField.OrganizationCode.Length | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. |
| 400 Bad Request | InvalidField.OrganizationCriteria.Type | The 'OrganizationCriteria.Type' must be a valid Enum. |
| 400 Bad Request | InvalidField.OrganizationFeeOverride.Amount | The 'Amount' value must be equal or greater than zero. |
| 400 Bad Request | InvalidField.OrganizationGroupCode | The 'organizationGroupCode' must be 3 characters in length. |
| 400 Bad Request | InvalidField.Origin.Length | The 'Origin' station code has a maximum length of 3 characters. |
| 400 Bad Request | InvalidField.Page | The 'Page' must be greather than or equal to 1. |
| 400 Bad Request | InvalidField.PageNumber | The 'Page' number must be between {0} and {1}. |
| 400 Bad Request | InvalidField.PageSize | The 'PageSize' number must be between {0} and {1}. |
| 400 Bad Request | InvalidField.Passenger | The minimum count of 'passengers' array is 1. |
| 400 Bad Request | InvalidField.Passenger.Email | The 'Passenger.Email' is invalid. |
| 400 Bad Request | InvalidField.Passenger.IssuingCountry | The 'InvalidField.Passenger.IssuingCountry' has a maximum of 2 characters. |
| 400 Bad Request | InvalidField.Passenger.Name | The 'Passengers.Name' is required. |
| 400 Bad Request | InvalidField.Passenger.Nationality | The 'Passenger.Nationality' has a maximum of 2 characters. |
| 400 Bad Request | InvalidField.Passenger.OverMaximum | The maximum count of 'Passenger' array is 3. |
| 400 Bad Request | InvalidField.Passenger.Phone | The 'PassengerAddress.Phone' has a maximum of 20 characters. |
| 400 Bad Request | InvalidField.Passenger.Type | The 'PassengerRequest.PassengerTypeCode' has a maximum of 3 characters. |
| 400 Bad Request | InvalidField.Passenger.UnderMinimum | The minimum count of 'Passenger' array is 1. |
| 400 Bad Request | InvalidField.PassengerAddress.CultureCode | The 'PassengerAddress.CultureCode' has a maximum of 17 characters. |
| 400 Bad Request | InvalidField.PassengerAddress.StationCode | The 'PassengerAddress.StationCode' has a minimum of 3 and a maximum of 3 characters. |
| 400 Bad Request | InvalidField.PassengerCount.UnderMinimum | The 'Passengers.Count' must be greater than 0. |
| 400 Bad Request | InvalidField.PassengerKeys.Empty | The 'PassengerKeys' array cannot contain empty values. |
| 400 Bad Request | InvalidField.PassengerType | The 'Passengers.Type' must be equal to 'ADT', 'CHD' or 'INF'. |
| 400 Bad Request | InvalidField.PassengerType.Length | The 'Passengers.Type' has a maximum length of 3 characters. |
| 400 Bad Request | InvalidField.PassengerType.Repeated | Must only have one 'Passenger.Type' of type ADT. |
| 400 Bad Request | InvalidField.Password | The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. |
| 400 Bad Request | InvalidField.Period | The 'PeriodCriteria.Period' must be a valid Enum. |
| 400 Bad Request | InvalidField.PeriodCriteria.Type | The 'PeriodCriteria.Type' must be a valid Enum. |
| 400 Bad Request | InvalidField.Phone | The 'Phone' provided is invalid. |
| 400 Bad Request | InvalidField.ProductClass | The 'ProductClass' must have a maximum of 2 character. |
| 400 Bad Request | InvalidField.ProgramNumber | The 'ProgramNumber' has a maximum lenght of 20 characters. |
| 400 Bad Request | InvalidField.Promotion.Code | The 'PromotionCode' is invalid. |
| 400 Bad Request | InvalidField.PromotionCode | The 'PromotionCode' is invalid! |
| 400 Bad Request | InvalidField.PromotionCode.Length | The 'PromotionCode' has a maximum length of 8 characters. |
| 400 Bad Request | InvalidField.ProviderType | The 'ProviderType' must be a valid Enum. |
| 400 Bad Request | InvalidField.RecordLocator | The 'RecordLocator' must have 6 characters. |
| 400 Bad Request | InvalidField.RefundType | The 'RefundType' must be a valid Enum. |
| 400 Bad Request | InvalidField.ReportId | The informed 'ReportId' is invalid. |
| 400 Bad Request | InvalidField.Role.User | The 'Role' for user informed is invalid. |
| 400 Bad Request | InvalidField.ServicesCount | The 'Services.Count' must be greather than 0. |
| 400 Bad Request | InvalidField.StationCode | The 'StationCode' must be 3 characters. |
| 400 Bad Request | InvalidField.Suffix | The 'Suffix' must be a valid Enum. |
| 400 Bad Request | InvalidField.TaxAmount | The 'TaxAmount' must be greater than or equal to 0. |
| 400 Bad Request | InvalidField.Title | The 'Title' must be a valid Enum. |
| 400 Bad Request | InvalidField.Transaction | The 'PaymentCriteria.Transaction' must be a valid Enum. |
| 400 Bad Request | InvalidField.TravelDocument.BirthCountry | The 'TravelDocuments.BirthCountry' has a maximum length 2 characters. |
| 400 Bad Request | InvalidField.TravelDocument.IssuingCountry | The 'TravelDocuments.IssuingCountry' has a maximum length 2 characters. |
| 400 Bad Request | InvalidField.TravelDocument.Number | The 'TravelDocuments.Number' has a maximum length 35 characters. |
| 400 Bad Request | InvalidField.TravelDocument.Type | The 'TravelDocuments.Type' must be a valid Enum. |
| 400 Bad Request | InvalidField.TravelDocuments.IssuingCountry | The 'TravelDocuments.IssuingCountry' has a maximum length 3 characters. |
| 400 Bad Request | InvalidField.TravelDocuments.Type | The 'TravelDocuments.Type' has a maximum of 4 characters. |
| 400 Bad Request | InvalidField.Type | The 'Type' must be an valid Enum. |
| 400 Bad Request | InvalidField.Username | The 'Username' is invalid. Must be a valid CPF. |
| 400 Bad Request | InvalidField.Username.Length | The 'Username' must be a string with a maximum length of 128. |
| 400 Bad Request | InvalidField.UsernameMatching | The 'UsernameMatching' cannot be entered with 'FirstName'. |
| 400 Bad Request | InvalidField.VerificationCode | The 'VerificationCode' is invalid. |
| 400 Bad Request | InvalidField.VerificationCode.Length | The 'VerificationCode' has a maximum length of 4 characters. |
| 400 Bad Request | InvalidField.Week | the 'PeriodCriteria.Week' can only be informed if the 'PeriodCriteria.Type' is equal to 'Week'. |
| 400 Bad Request | InvalidField.Year | The 'PeriodCriteria.Year' must be equal to or before than the current year. |
| 400 Bad Request | IssuingCountry.NotFound | The 'IssuingCountry' was not found. |
| 400 Bad Request | Journey.DepartureDate.Passed | It is not possible to remove a journey whose departure date has already passed. |
| 400 Bad Request | Journey.Fare.SoldOut | The informed 'fareKey' is sold out. |
| 400 Bad Request | Journey.FareKey | The 'FareKey' is invalid or is sold out. |
| 400 Bad Request | JourneyKey.Decoding.Error | An error occurred while decoding a JourneyKey. |
| 400 Bad Request | JourneyKey.NotFound | The 'JourneyKey' not found. |
| 400 Bad Request | Journeys.DepartureTimeLimit | Sent JourneyKey is too close to it's deaparture time. |
| 400 Bad Request | Journeys.Duplicated | Leg already existing in the offer. |
| 400 Bad Request | Journeys.Overlap | The times of informed journeys overlaps. |
| 400 Bad Request | LiableRecordLocator.UnaccompaniedMinor.Issuing | The 'LiableRecordLocator' can only be informed for issuing an order with unaccompanied minors. |
| 400 Bad Request | Loyalty.Authentication.Invalid | Invalid Authentication. |
| 400 Bad Request | Loyalty.Customer.NotFound | The customer not found. |
| 400 Bad Request | Loyalty.InvalidToken.Expired | Token is invalid or expired. |
| 400 Bad Request | Loyalty.Request.Failed | The Loyalty request failed. |
| 400 Bad Request | Loyalty.Tier.NotFound | The customer tier not found. |
| 400 Bad Request | Market.NotAvailable | The set of stations requested do not have an available market yet. |
| 400 Bad Request | Market.Unavailable | The informed origin/destination market are currently unavailable for low fare estimate search. |
| 400 Bad Request | Name.AlreadyChanged | This passenger name has already been changed, You are not allowed to change the passenger's name again. |
| 400 Bad Request | Name.NotUpdated | This passenger name is the same to the one filled in this booking, Please check the name's change and try again. |
| 400 Bad Request | Name.NotUpdatedLimit | This passenger's name has a limit of 4 characters when changing the name. |
| 400 Bad Request | Nationality.NotFound | The 'Nationality' was not found. |
| 400 Bad Request | Navitaire.SeatCreate.Failed | The request failed to assign seat. |
| 400 Bad Request | NotAvailable.Credit | The informed 'RecordLocator' has no credit available. |
| 400 Bad Request | NotChange.Password | Attempt to modify password was not successful. Please check if new password is different from the current or if it's different from the last 5 used passwords. |
| 400 Bad Request | Offer.UnaccompaniedMinor.AdditionalFees | Unaccompanied minor may incur additional fee, according to company policy. |
| 400 Bad Request | Order.Calculation.NotPending | The order in the state has no calculations to be done. |
| 400 Bad Request | Order.Calculation.Pending | Order details can only be retrieved after calculation of its changes. If you are changing journeys, please finish desired changes and do a calculate before retrieving. |
| 400 Bad Request | Orders.Group.Error | You are not allowed to see Orders Groups in this method. |
| 400 Bad Request | Orders.Group.Error | You are not allowed to add baggages to Orders Groups in this method.|
| 400 Bad Request | Orders.Group.Error | You are not allowed to add services to Orders Groups in this method.|
| 400 Bad Request | Order.Journeys.Count | The maximum number of Journeys allowed in a order is {0}. |
| 400 Bad Request | Order.NoChildren | The informed order does not have any children record locator associated. |
| 400 Bad Request | Order.NoJourneys | The informed order has no journeys to be managed. |
| 400 Bad Request | Order.Passengers.NoDateOfBirth | It is not possible to divide orders without all passengers having their date of birth informed in the order. |
| 400 Bad Request | Order.PendingCalculation | There are pending calculations to be performed. Call the order calculate method before confirming your order changes. |
| 400 Bad Request | Order.Reaccommodation.Pending | It is not possible manage an order with pending reaccommodation. |
| 400 Bad Request | Order.RefundType.NotAllowed | The 'RefundType' field can only be entered when 'Cancel' is true. |
| 400 Bad Request | Order.Retrieve.V1.Conflict | This method is not compatible with retrieve order in V1. |
| 400 Bad Request | Order.Retrieve.V2.Conflict | This method is not compatible with retrieve order in V2. |
| 400 Bad Request | Order.State.Timeout | The state time for this order has expired. Please retrieve the order again with the GET Order method. |
| 400 Bad Request | Order.Quarantine.payment | This order is in payment quarantine. |
| 400 Bad Request | OrderDivide.BalanceDue.Underpaid | Underpaid orders cannot be divided. |
| 400 Bad Request | OrderDivide.CreditAmount.invalid | The informed 'creditAmount' is invalid because it's greater than the amount available in the informed order. |
| 400 Bad Request | OrderDivide.DivideCredit.Failed | An error occurred while dividing the order credit. Credit values have not been divided or changed, remaining entirely in the parent order. |
| 400 Bad Request | OrderDivide.PassengerKeys.InvalidAmount | The number of 'passengerKeys' in the request must be less than the number of passengers in the informed order. |
| 400 Bad Request | OrderDivide.Pending.Service | It is not possible to perform order divide after a service addition/change. Please confirm changes to your order before splitting it, or split it first before making changes. |
| 400 Bad Request | OrderDivide.Unaccompanied.NotAllowed | It's not allowed to divide an order when it will result in orders where there are only unaccompanied minors (under {0} years old). Both involved orders must contain at least one adult passenger (ADT) over {0} years of age at the end of the division. |
| 400 Bad Request | Orders.Fares.Error | You are not allowed to see others fares in this method. |
| 400 Bad Request | Organization.AlreadyIntoGroup | The informed OrganizationCode is already inserted in this organization group. |
| 400 Bad Request | Organization.AuthorizationFailed | The agent does not have access to the finder organization, either on its own or by a group. |
| 400 Bad Request | Organization.CNPJ.Invalid | The point of sale organization does not have a valid CNPJ. |
| 400 Bad Request | Organization.Conflict | You are not allowed to delete your own point of sale from a group. |
| 400 Bad Request | Organization.Email | Your organization doesn't have a valid email. Please contact Azul's comercial team. |
| 400 Bad Request | Organization.Request.Failed | The Organization request failed. |
| 400 Bad Request | OrganizationAccount.NotFound | Organization has no account. |
| 400 Bad Request | OrganizationGroup.Invalid | OrganizationGroup already exists or invalid. |
| 400 Bad Request | Passenger.AssignedSeat | Seat already assigned to the passenger. |
| 400 Bad Request | Passenger.DocumentType.Confict | Document already informed to the passenger of the order. |
| 400 Bad Request | Passenger.DocumentTypeMatch.NotAllowed | Multiple Passengers with the same Travel Document Type and Number are not allowed, including Infants. |
| 400 Bad Request | Passenger.InvalidAge | Passenger under 12 years old on the departure date cannot be considered an adult (ADT). |
| 400 Bad Request | Passenger.NameMatch.NotAllowed | Multiple Passengers with exactly the same First Name, Middle Name, Last Name and Suffix are not allowed, including Infants. |
| 400 Bad Request | Passenger.TraveDocument.Expired | Informed travel document will be expired on the departure date. |
| 400 Bad Request | Passenger.Unaccompanied.InvalidAge | Minors must be over 8 years old to travel unaccompanied. |
| 400 Bad Request | PassengerFeeKey.NotFound | The 'PassengerFeeKey' not found. |
| 400 Bad Request | Payments.Credit.Failed | An error occurred while using the credit. |
| 400 Bad Request | Payments.MinimumRequired | Payments must contemplate all journey fares, travel fees and taxes. |
| 400 Bad Request | Payments.ValidationError | Checkout validation error. Payments amount does not match the total cost of the order. |
| 400 Bad Request | Profile.HoldPermission | Your current profile does not allow hold creation. |
| 400 Bad Request | Quote.UnaccompaniedMinor.NotAllowed | The 'JourneyKeys' {0} does not allow unaccompanied minors. |
| 400 Bad Request | Reaccommodation.InProcess | Reaccommodation is in process. Wait 24 hours for it to be updated. |
| 400 Bad Request | Refund.Fare.SoldOut | The requested class of service is sold out. |
| 400 Bad Request | RecordLocator.NotFound | The given 'RecordLocator' was not found. |
| 400 Bad Request | RefundAuthentication.Request.Failed | The request failed. |
| 400 Bad Request | Refund.Override.InvalidValue | No increase in value is allowed in an Override operation. |
| 400 Bad Request | RefundOrder.Fare.NotAvailable | Fare not available. |
| 400 Bad Request | RefundType.CreditShell.CannotBeApplied | It is not possible to make the refund via credit shell. |
| 400 Bad Request | RefundType.Payments.CannotBeApplied | There are no amounts to be refunded. |
| 400 Bad Request | Report.AlreadyExists | There is already an existing report for the informed 'OrderCriteria' and 'PeriodCriteria'. |
| 400 Bad Request | Report.InProcess | The report cannot be changed while it is being processed. |
| 400 Bad Request | Report.PendingCreation | The requested report is not available for download yet, as it has not been created. |
| 400 Bad Request | Report.RetrieveError | An unexpected error occurred while retrieving the report file. |
| 400 Bad Request | Request.Failed | The Refund request failed. |
| 400 Bad Request | RequestFailed.CreditCard.Expired | Expired credit card. |
| 400 Bad Request | RequestFailed.Enterprise | An error occurred while validating order passengers names. |
| 400 Bad Request | RequestFailed.International.Required | The organization fee override is only allowed for orders with international journeys. |
| 400 Bad Request | RequestFailed.Journeys.NotAllowed | The organization fee override is only allowed while adding new journeys to the order and execute the calculate. |
| 400 Bad Request | RequestFailed.PassengerMinor.NotAllowedInfants | Passengers under 18 years old are not allowed to have infants. |
| 400 Bad Request | RequestFailed.Passengers.WithoutFee | No passengers in this order have organization fees charged. |
| 400 Bad Request | RequestFailed.TudoAzul.Retrieve | An error occurred while retrieving the TudoAzul program. |
| 400 Bad Request | RequestFailed.Unexpected | An unexpected error has occurred. |
| 400 Bad Request | Required.RefundType | The 'RefundType' is required. |
| 400 Bad Request | RequiredField.Account | The 'Account' is required. |
| 400 Bad Request | RequiredField.Amount | The 'Amount' is required. |
| 400 Bad Request | RequiredField.AssistanceArray | The 'Assistances' array is required. |
| 400 Bad Request | RequiredField.AssistancesCount | The 'Assistances.Count' is required. |
| 400 Bad Request | RequiredField.AssistancesKey | The 'Assistances.Key' is required. |
| 400 Bad Request | RequiredField.ChangeType | The 'ChangeType' is required. |
| 400 Bad Request | RequiredField.Code | The 'Code' is required. |
| 400 Bad Request | RequiredField.Contact.FirstName | The 'Contact.FirstName' is required. |
| 400 Bad Request | RequiredField.Contact.LastName | The 'Contact.LastName' is required. |
| 400 Bad Request | RequiredField.Contact.Phones | The 'Contact.Phones' is required. |
| 400 Bad Request | RequiredField.ContactAddress.LineOne | The 'Contact.Address.LineOne' is required. |
| 400 Bad Request | RequiredField.ContactName | The 'Contact.Name' object is required. |
| 400 Bad Request | RequiredField.ContactName.First | The 'Contact.Name.First' is required. |
| 400 Bad Request | RequiredField.ContactName.Last | The 'Contact.Name.Last' is required. |
| 400 Bad Request | RequiredField.ContactPhones.Number | The 'Contact.Phones.Number' is required. |
| 400 Bad Request | RequiredField.ContactPhones.Type | The 'Contact.Phones.Type' is required. |
| 400 Bad Request | RequiredField.ContactPhonesHome | The 'Contact.Phones' a home object is required. |
| 400 Bad Request | RequiredField.CreditCard.ExpirationMonth | The 'ExpirationMonth' is required. |
| 400 Bad Request | RequiredField.CreditCard.ExpirationYear | The 'ExpirationYear' is required. |
| 400 Bad Request | RequiredField.CreditCard.GovId | The 'GovId' is required for this method code due to the currency code of the order. |
| 400 Bad Request | RequiredField.CreditCard.HolderName | The 'HolderName' is required. |
| 400 Bad Request | RequiredField.CreditCard.MethodCode | The 'MethodCode' is required. |
| 400 Bad Request | RequiredField.CreditCard.Type | The 'CreditCard.Type' is required |
| 400 Bad Request | RequiredField.CreditCard.VerificationCode | The 'VerificationCode' is required. |
| 400 Bad Request | RequiredField.Criteria | The 'Criteria' is only required for 'CriteriaType': 'Phone', 'Email', 'DocumentNumber', 'CardNumber' and 'CustomerNumber'. |
| 400 Bad Request | Customer.AlreadyCategorized | This passenger has already been categorized, You are not allowed to change the passenger's name. |
| 400 Bad Request | RequiredField.CriteriaType | The 'CriteriaType' is only required for 'Type': 'Organization'. |
| 400 Bad Request | RequiredField.CurrencyCode | The 'CurrencyCode' is required. |
| 400 Bad Request | RequiredField.CurrentPassword | User not authenticated. The field 'Username' is required. |
| 400 Bad Request | RequiredField.DateOfBirth | The 'DateOfBirth' is required. |
| 400 Bad Request | RequiredField.Day | The 'PeriodCriteria.Day' is required. |
| 400 Bad Request | RequiredField.Departure | The 'Departure' is required. |
| 400 Bad Request | RequiredField.DepartureBegin | The 'DepartureBegin' is required. |
| 400 Bad Request | RequiredField.DepartureDate | The 'Departure' is required. |
| 400 Bad Request | RequiredField.DepartureEnd | The 'DepartureEnd' is required. |
| 400 Bad Request | RequiredField.Destination | The 'Destination' is required. |
| 400 Bad Request | RequiredField.Document.Type | The 'Infant.Document.Type' CPF, RNE or PASSPORT is required. |
| 400 Bad Request | RequiredField.DocumentType | The 'DocumentType' is required for the informed 'CriteriaType'. |
| 400 Bad Request | RequiredField.Email | The 'Email' is required. |
| 400 Bad Request | RequiredField.FareKey | The 'FareKey' is required. |
| 400 Bad Request | RequiredField.FirstName | The 'FirstName' is required for the 'FirstNameMatching' field. |
| 400 Bad Request | RequiredField.FirstNameMatching | The 'FirstNameMatching' is required for the 'FirstName' field. |
| 400 Bad Request | RequiredField.Gender | The 'Gender' must be a valid Enum. |
| 400 Bad Request | RequiredField.Identifier | The 'Identifier' is required. |
| 400 Bad Request | RequiredField.Infant.FirstName | The 'Infant.FirstName' is required. |
| 400 Bad Request | RequiredField.Infant.Gender | The 'Infant:Gender' is required. |
| 400 Bad Request | RequiredField.Infant.LastName | The 'Infant.LastName' is required. |
| 400 Bad Request | RequiredField.IropContact | The 'Passengers.IropContact' is required. |
| 400 Bad Request | RequiredField.IropContact.EmailMobile | The 'Passengers.IropContact.Email' or 'Passengers.IropContact.Mobile is required. |
| 400 Bad Request | RequiredField.IropContact.Refused | The 'Passengers.IropContact.Refused' is required. |
| 400 Bad Request | RequiredField.JourneyKey | The 'JourneyKey' is required. |
| 400 Bad Request | RequiredField.Journeys | The 'Journeys' array is required. |
| 400 Bad Request | RequiredField.Journeys.Departure | The 'Departure' is required. |
| 400 Bad Request | RequiredField.Journeys.Key | The 'Journey.Key' is required. |
| 400 Bad Request | RequiredField.Key | The 'Key' is required. |
| 400 Bad Request | RequiredField.Keys | The 'Keys' array is required. |
| 400 Bad Request | RequiredField.LastName | The 'LastName' is required. |
| 400 Bad Request | RequiredField.Month | The 'PeriodCriteria.Month' is required. |
| 400 Bad Request | RequiredField.Name | The 'Name' is required. |
| 400 Bad Request | RequiredField.Name.First | The 'Name.First' is required. |
| 400 Bad Request | RequiredField.Name.Last | The 'Name.Last' is required. |
| 400 Bad Request | RequiredField.Name.Middle | The 'Name.Middle' is required. |
| 400 Bad Request | RequiredField.NameToChange | The 'NameToChange' is required. |
| 400 Bad Request | RequiredField.Nationality | The 'Nationality' is required. |
| 400 Bad Request | RequiredField.NewName | The 'NewName' is required. |
| 400 Bad Request | RequiredField.NewPassword | The 'NewPassword' is required. |
| 400 Bad Request | RequiredField.Offers | The 'Offers' array is required. |
| 400 Bad Request | RequiredField.Offers.CurrentJourneyKey | The 'CurrentJourneyKey' is required. |
| 400 Bad Request | RequiredField.Offers.FareKey | The 'Offers.FareKey' is required. |
| 400 Bad Request | RequiredField.Offers.JourneyKey | The 'Offers.JouneyKey' is required. |
| 400 Bad Request | RequiredField.Offers.NewFareKey | The 'NewFareKey' is required. |
| 400 Bad Request | RequiredField.Offers.NewJourneyKey | The 'NewJourneyKey' is required. |
| 400 Bad Request | RequiredField.OrderCriteria | The 'OrderCriteria' is required. |
| 400 Bad Request | RequiredField.OrderCriteria.Status | The 'OrderCriteria.Status' is required. |
| 400 Bad Request | RequiredField.OrderCriteria.Type | The 'OrderCriteria.Type' is required. |
| 400 Bad Request | RequiredField.OrganizationCode | The 'OrganizationCode' is required. |
| 400 Bad Request | RequiredField.OrganizationCriteria | The 'OrganizationCriteria' is required. |
| 400 Bad Request | RequiredField.OrganizationCriteria.Type | The 'OrganizationCriteria.Type' is required. |
| 400 Bad Request | RequiredField.OrganizationGroupCode | The 'OrganizationGroupCode' is required. |
| 400 Bad Request | RequiredField.Origin | The 'Origin' is required. |
| 400 Bad Request | RequiredField.Passenger | The 'Passenger' is required. |
| 400 Bad Request | RequiredField.Passenger.DateOfBirth | The 'Passenger.DateOfBirth' is required. |
| 400 Bad Request | RequiredField.Passenger.Gender | The 'Passenger.Gender' is required. |
| 400 Bad Request | RequiredField.Passenger.Key | The 'PassengerKey' is required. |
| 400 Bad Request | RequiredField.PassengerKeyRequired | The 'PassengerKeyRequired' is required.|
| 400 Bad Request | RequiredField.Passenger.PhoneEmail | The 'Passengers.Phone' or  'Passengers.Email' is required. |
| 400 Bad Request | RequiredField.Passenger.Type | The 'Passengers.Type' is required. |
| 400 Bad Request | RequiredField.PassengerKey | The 'PassengerKey' is required. |
| 400 Bad Request | RequiredField.PassengerKeys | The 'passengerKeys' informed in the request does not exist in the informed order. |
| 400 Bad Request | RequiredField.Passengers | The 'Passengers' array is required. |
| 400 Bad Request | RequiredField.PassengerType | The 'Passenger.Type' is required. |
| 400 Bad Request | RequiredField.PassengerType.Adult | The 'Passengers.Type' a ADT value is required. |
| 400 Bad Request | RequiredField.Password | The 'Password' is required. |
| 400 Bad Request | RequiredField.PaymentCriteria | The 'PaymentCriteria' is required. |
| 400 Bad Request | RequiredField.Period | The 'PeriodCriteria.Period' is required. |
| 400 Bad Request | RequiredField.PeriodCriteria.Type | The 'PeriodCriteria.Type' is required. |
| 400 Bad Request | RequiredField.Phone | The 'Phone' is required. |
| 400 Bad Request | RequiredField.PhonesNumber | The 'Phones.Number' is required. |
| 400 Bad Request | RequiredField.PhonesType | The 'Phones.Type' is required. |
| 400 Bad Request | RequiredField.Profile | The 'Profile' is required. |
| 400 Bad Request | RequiredField.ProgramNumber | The 'ProgramNumber' is required. |
| 400 Bad Request | RequiredField.ProviderType | The 'ProviderType' is required. |
| 400 Bad Request | RequiredField.RecordLocator | The 'RecordLocator' is required. |
| 400 Bad Request | RequiredField.ReportId | The 'ReportId' is required. |
| 400 Bad Request | RequiredField.SegmentKey | The 'segmentkey' is required. |
| 400 Bad Request | RequiredField.Services | The 'Services' list is required. |
| 400 Bad Request | RequiredField.ServicesCount | The 'Services.Count' is required. |
| 400 Bad Request | RequiredField.ServicesKey | The 'Services.Key' is required. |
| 400 Bad Request | RequiredField.SessionContext | The 'SessionContext' is required. |
| 400 Bad Request | RequiredField.Status | The 'Status' is required. |
| 400 Bad Request | RequiredField.TravelDocument | The minimum count of 'TravelDocument' array is 1. |
| 400 Bad Request | RequiredField.TravelDocument.ExpirationDate | The 'TravelDocuments.ExpirationDate' is required. |
| 400 Bad Request | RequiredField.TravelDocument.Number | The 'TravelDocuments.Number' is required. |
| 400 Bad Request | RequiredField.TravelDocument.Type | The 'TravelDocuments.Type' CPF, RNE or PASSPORT is required. |
| 400 Bad Request | RequiredField.TravelDocuments.IssuingCountry | The 'TravelDocuments.IssuingCountry' is required. |
| 400 Bad Request | RequiredField.TravelDocuments.Type | The 'TravelDocuments.Type' is required. |
| 400 Bad Request | RequiredField.Type | The 'Type' is required. |
| 400 Bad Request | RequiredField.UnitKey | The 'unitkey' is required. |
| 400 Bad Request | RequiredField.UserKey | The 'UserKey' is required. |
| 400 Bad Request | RequiredField.Username | The 'Username' is required. |
| 400 Bad Request | RequiredField.Week | The 'PeriodCriteria.Week' is required. |
| 400 Bad Request | RequiredField.Year | The 'PeriodCriteria.Year' is required. |
| 400 Bad Request | Retrieve.NoActions | There are no more journeys waiting for agent actions on this order. |
| 400 Bad Request | Roles.NotAllowed | Cannot edit the user that belongs to WebService roles. |
| 400 Bad Request | Seat.Unavailable | Seat already assigned to another passenger. |
| 400 Bad Request | Service.Quantity.Restricted | This service is restricted to one occurence per passenger and leg. |
| 400 Bad Request | Shopping.Request.Failed | The Shopping request failed. |
| 400 Bad Request | Stations.NotAllowed | These requested stations are invalid: |
| 400 Bad Request | Token.InvalidDecodeJwtBadRequest | Error decoding token. |
| 400 Bad Request | Token.InvalidReadJwtBadRequest | Error reading token. |
| 400 Bad Request | Token.FailedBadRequest | It is not possible to generate token without group DL. |
| 400 Bad Request | Token.InvalidSignatureBadRequest | Invalid Token Signature. |
| 400 Bad Request | Token.ExpiredBadRequest | The token has expired. |
| 400 Bad Request | TudoAzul.Categorization.Failed | There was a failure in the categorization of TudoAzul of 'passengers.customerProgram.number': {0}. Try categorize again after the order creation (before assigning seats or adding baggages to ensure all potential benefits). |
| 400 Bad Request | UnitKey.Invalid | The 'UnitKey' is invalid. |
| 400 Bad Request | User.CannotBeUnlocked | Only API users can be unlocked. |
| 400 Bad Request | User.NoGroup | The user must be in an Organization Group when the ‘Type’ is Group. |
| 400 Bad Request | User.NotEditable | Deleted user cannot be edited. |
| 400 Bad Request | User.Password.Expired | Expired password, user must change password. |
| 400 Bad Request | Warning.OrganizationFeeOverride | Organization fee override is not applicable for this order. |
| 400 Bad Request | Duplicate.Organization | The informed organization code already exists. |
| 400 Bad Request | InvalidField.Address.City | The 'City' must be 32 characters in length. |
| 400 Bad Request | InvalidField.Address.CompanyName | The 'CompanyName' must be 128 characters in length. |
| 400 Bad Request | InvalidField.Address.CountryCode | The 'CountryCode' must be 2 characters in length. |
| 400 Bad Request | InvalidField.Address.LineOne | The 'LineOne' must be 128 characters in length. |
| 400 Bad Request | InvalidField.Address.LineTwo | The 'LineTwo' must be 128 characters in length. |
| 400 Bad Request | InvalidField.Address.PostalCode | The 'PostalCode' must be 10 characters in length. |
| 400 Bad Request | InvalidField.Address.ProvinceState | The 'ProvinceState' must be 2 characters in length. |
| 400 Bad Request | InvalidField.Company.EmailAdress | The 'EmailAdress' must be a valid. |
| 400 Bad Request | InvalidField.CompanyPhones.Number | The 'Company.Phones.Number' has a maximum length 20 characters. |
| 400 Bad Request | InvalidField.CompanyPhones.Type | The 'Company.Phones.Type' must be a valid enum. |
| 400 Bad Request | InvalidField.ContactName.First | The 'Contact.Name.First' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Last | The 'Contact.Name.Last' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Middle | The 'Contact.Name.Middle' has a maximum length 32 characters. |
| 400 Bad Request | InvalidField.ContactName.Suffix | The 'Contact.Name.Suffix' must be a valid enum. |
| 400 Bad Request | InvalidField.ContactName.Title | The 'Contact.Name.Title' must be a valid enum. |
| 400 Bad Request | InvalidField.ContactPhones.Number | The 'Contact.Phones.Number' has a maximum length 20 characters. |
| 400 Bad Request | InvalidField.ContactPhones.Type | The 'Contact.Phones.Type' must be a valid enum. |
| 400 Bad Request | InvalidField.IataCode | The 'IataCodeLength' must be 8 characters in length. |
| 400 Bad Request | InvalidField.LastStatementDate | The 'LastStatementDate' must be a valid. |
| 400 Bad Request | InvalidField.OverrideDuFee | The organizationFeeOverride cannot be informed when overrideDuFee was already informed. |
| 400 Bad Request | InvalidField.StatementNote | The 'StatementNote' must be 128 characters in length. |
| 400 Bad Request | InvalidField.NewName | Please check the 'NewName', it can't start with special characters and numbers. |
| 400 Bad Request | RequiredField.Company.Cnpj | The 'Company Cnpj' is required. |
| 400 Bad Request | RequiredField.CompanyPhones.Type | The 'Company.Phones.Type' is required. |
| 400 Bad Request | RequiredField.ConpanyPhones.Number | The 'Conpany.Phones.Number' is required. |
| 400 Bad Request | RequiredField.ContactPhones.Type | The 'Contact.Phones.Type' is required. |
| 400 Bad Request | RequiredField.ParentCode | The 'ParentCode' is required. |
| 400 Bad Request | NotApplied.PromotionCode | Application of promotionCode is only permitted on hold reservations.|
| 400 Bad Request | InvalidField.Promotion.Code | It is not possible to apply a promo code to reservations that contain the promo code. |
| 400 Bad Request | Invalid.TravelDocument.Type | The document type Mercosur is invalid for this IssuingCountry. |
| 400 Bad Request | Comments.NotAllowed | Comment will not be recorded as it does not meet the PS rule. | It is not possible to send comments when the user does not have the "LEMO" role, and does not meet the PS product class rule. |
| 400 Bad Request | Comments.Maximum.Lenght | The 'Comments' must be a maximum of 1024 characters. | The comment exceeds the supported character limit. |
| 400 Bad Request | Invalid.Authentication.Session | The Authentication Session is denied because the token is an Active Directory. | 
Error authenticating using an AD type token. |
| 400 Bad Request | Invalid.Authentication.Groups.Portal.Session | The Authentication Groups Portal is denied because the session must be an Active Directory. | Error authenticating to the groups portal using a token other than AD. |
| 401 Unauthorized | InvalidToken.Expired | An error occurred while performing authentication. |
| 401 Unauthorized | InvalidToken.NotAuthenticated | The Bearer Token provided is invalid or expired. |
| 401 Unauthorized | RequestFailed.Authentication | An error occurred while validating the user authentication. |
| 401 Unauthorized | InvalidToken.NotInformed | Bearer Token not informed. The token must be informed in the request header. |
| 401 Unauthorized | InvalidToken.NotAuthenticated | Not Authenticated. The Agent must be authenticated thru User API. |
| 401 Unauthorized | InvalidToken.Expired | Provided JWT is invalid or expired. |
| 403 Forbidden | Agent.MethodCode.NotAllowed | The logged agent is not allowed to make payments using this method code. |
| 403 Forbidden | Agent.NoAccess | The agent does not have access to the informed user. |
| 403 Forbidden | AssignSeat.UnitKey.Blocked | The request failed to assign the seat, because this seat is blocked by passengers rules (age, SSR or equipment). |
| 403 Forbidden | Organization.AuthorizationFailed.User | This user does not have access to the informed organization. |
| 403 Forbidden | AuthorizationFailed.InvalidRole | The agent does not have the required roles to access this method. |
| 404 Not Found | Assistance.NoMatches | This assistance does not exist or was not found. |
| 404 Not Found | Assistances.NoMatches | Unable to retrieve the assistances data. |
| 404 Not Found | AssistancesKey.NoMatches | The informed 'Assistances.Key' does not exists or does not belong to a previously retrieved 'assistance/search'. |
| 404 Not Found | Baggage.NoMatches | No 'Baggage' was found for removal. |
| 404 Not Found | BagKey.NoMatches | The informed 'Key' does not exists or does not belong to a previously retrieved 'baggage/search'. |
| 404 Not Found | Code.NoMatches | Informed Organization Code was not found. |
| 404 Not Found | Countries.NoMatches | Unable to retrieve the countries data. |
| 404 Not Found | Country.NoMatches | This country does not exist or was not found. |
| 404 Not Found | CreditNoMatches | There is no credit available for the informed type. |
| 404 Not Found | CustomerNumber.NoMatches | The 'CustomerProgram' not found. |
| 404 Not Found | CustomerProgram.NoMatches | The Customer Program was not found. |
| 404 Not Found | Equipment.NoMatches | This equipament does not exist or was not found. |
| 404 Not Found | Fare.NoMatches | This fare does not exist or was not found. |
| 404 Not Found | Fares.NoMatches | Unable to retrieve the fares data. |
| 404 Not Found | Fee.NoMatches | This fee does not exist or was not found. |
| 404 Not Found | Fees.NoMatches | Unable to retrieve the fees data. |
| 404 Not Found | InvalidField.JourneyKey | The 'JourneyKey' is invalid. |
| 404 Not Found | JourneyKey.NoMatches | The 'JourneyKey' is invalid or does not exists in the current state. |
| 404 Not Found | NoMatches | The informed user does not exist or was not found. |
| 404 Not Found | Order.NoMatches | The requested order was not found or does not exist. |
| 404 Not Found | OrderCache.NoMatches | An order must be attached. |
| 404 Not Found | OrderSearch.NoMatches | No orders found for the informed search filters. |
| 404 Not Found | Organization.NoMatches | The informed organization does not exist or was not found. |
| 404 Not Found | OrganizationCode.NoMatches | The informed 'OrganizationCode' doesn't exists or doesn't belong to the same organization as your current Point of Sale. |
| 404 Not Found | OrganizationGroup.NoMatches | The informed organization group does not exist or was not found. |
| 404 Not Found | OrganizationGroupCode.NoMatches | The 'OrganizationGroupCode does not exist or was not found. |
| 404 Not Found | PassengerKey.NoMatches | The informed 'PassengerKey' does not match within those on the order in state. |
| 404 Not Found | PassengerName.NoMatches | The Passenger name does not match within informed Customer Program. |
| 404 Not Found | Payments.NoMatches | No payments were found for the order in state. |
| 404 Not Found | RecordLocator.NoMatches | Your order must be created to use its credits. |
| 404 Not Found | RefundOrder.NoMatches | Order not found. Retrieve the order. |
| 404 Not Found | ReportId.NoMatches | The informed 'ReportId' does not exists or was not found. |
| 404 Not Found | Seat.NoMatches | Seat not found. |
| 404 Not Found | SeatMap.NoMatches | No matching seats. |
| 404 Not Found | SegmentKey.NoMatches | The 'SegmentKey' is invalid or does not exists in the current state. |
| 404 Not Found | Service.NoMatches | Service not found in the specified Journey. |
| 404 Not Found | ServiceKey.NoMatches | The informed 'Services.Key' does not exists or does not belong to a previously retrieved 'service/search'. |
| 404 Not Found | SessionContextToken.NoMatches | No sessions found for the given provider. |
| 404 Not Found | Station.NoMatches | This station does not exist or was not found. |
| 404 Not Found | Stations.NoMatches | Unable to retrieve the stations data. |
| 404 Not Found | TudoAzul.NoMatches | The informed 'passengers.customerProgram.number': {0} does not exists or was not found. |
| 404 Not Found | TudoAzulNames.NoMatches | The names of the informed 'passengers.customerProgram.number': {0} do not match those registered in TudoAzul. |
| 404 Not Found | UnitKey.NoMatches | The 'UnitKey' is invalid or does not exists in the current state. |
| 404 Not Found | User.NoMatches | The informed user does not exist or was not found. |
| 404 Not Found | UserKey.NoMatches | The informed 'UserKey' does not exist or was not found. |
| 404 Not Found | Username.NoMatches | The 'Username' user does not exist or was not found. |
| 406 Not Acceptable | Retrieve.Order.InvalidProductClass | It is not possible retrieve orders in v2 with the product class contained in the requested order. |
| 409 Conflict | AssignSeat.PassengerKey.Conflict | The PassengerKey does not exists in the order state. |
| 409 Conflict | AssignSeat.Seat.Conflict | Seat Already Assigned. |
| 409 Conflict | InvalidField.AssistanceCode | The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. |
| 409 Conflict | InvalidField.AssistanceLimit | The count for the 'Assistances.key' {0} is greater than the specified limit. |
| 409 Conflict | InvalidField.Assistanceskey | There are duplicated 'Assistances.key' {0}. |
| 409 Conflict | InvalidField.PassengerKeyCache | The requested service is not available for the informed passenger. |
| 409 Conflict | InvalidField.RecordLocator | The 'RecordLocator' must have 6 characters. |
| 409 Conflict | InvalidField.ServiceLimit | The count for the 'Services.key' {0} is greater than the specified limit. |
| 409 Conflict | InvalidField.Serviceskey | There are duplicated 'Services.key' {0}. |
| 409 Conflict | InvalidToken.Expired | An error occurred while performing authentication. |
| 409 Conflict | InvalidToken.NotAuthenticated | The Bearer Token provided is invalid or expired. |
| 409 Conflict | Journey.CodeShare.Restriction | Please contact partner carrier to add journeys started by a partner. |
| 409 Conflict | LiableRecordLocator.UnaccopaniedMinor.NotMatchJourneys | Liable order and unaccompanied minors order flights must match. |
| 409 Conflict | NotEmpty.State | It's not possible to attach with an order already retrieved in the current state. Please execute an order delete before the order attach. |
| 409 Conflict | Order.HasRecordLocator | This method is for orders under creation process. If you want to checkout a previously created order, please use the equivalent method in the Order.Management.Api. |
| 409 Conflict | Order.Recordlocator.Empty | This method is for previously created orders. If you want to retrieve an order under creation, please use the equivalent method in the Order.Api. |
| 409 Conflict | Order.State.Change | Removing a journey after adding journeys is not allowed. Please confirm your changes or restart the process retrieving the order again. |
| 409 Conflict | Order.State.Modified | The order in state has been externally modified. Retrieve the order again with the GET Order methods and try again. |
| 409 Conflict | Order.UnaccopaniedMinor.OperatedFligthAzul | Unaccompanied minors are allowed in Azul operated flights only. |
| 409 Conflict | Order.UnderCreationException | This method is for orders under creation process. If you want to retrieve a previously created order, please use the equivalent method in the Order.Management.Api. |
| 409 Conflict | Refund.NotApplicable | There is no amount in the order to be refunded. |
| 409 Conflict | RequestFailed.UnaccompaniedMinor.DomesticFligths | Unaccompanied minors are allowed in brazilian domestic flights only. |
| 409 Conflict | RequestFailed.UnaccopaniedMinor.OnlyDirectFlight | Unaccompanied minors are allowed in direct flights only. |
| 409 Conflict | RequiredField.LiableRecordLocator | A passenger over 18 years old is required in the liable order. |
| 409 Conflict | Organizations.CNPJ.error | You are not allowed to create Organizations to this CNPJ. |
| 409 Conflict | Retrieve.V2.NotExecuted | Get Order V2 has not been executed. |
| 422 Unprocessable Content | Assistance.SearchRequired | Retrieve a 'assistances/search' with journeyKey before execute this method. |
| 422 Unprocessable Content | Baggage.SearchRequired | Retrieve a 'baggage/search' with journeyKey before execute this method. |
| 422 Unprocessable Content | NotMatch.Name | The names sent do not match those on the attached order. |
| 422 Unprocessable Content | NotMatch.PassengerKey | An informed passenger key does not exists in the attached order or is invalid. |
| 422 Unprocessable Content | Order.RetrieveRequired | The requested order was not found or does not exist. |
| 422 Unprocessable Content | Order.State.Timeout | The state time for this order has expired. Please retrieve the order again with the GET Order method. |
| 422 Unprocessable Content | SeatMapCache.SearchRequired | No seatmap found or generated in state. Please retrieve a seatmap before trying to assign a seat. |
| 422 Unprocessable Content | Service.SearchRequired | Retrieve a 'services/search' with journeyKey before execute this method. |
| 422 Unprocessable Content | UnitKey.SearchRequired | The informed UnitKey does not belong to a previously retrieved SeatMap or the previous retrive is expired. |
| 422 Unprocessable Content | Reaccommodation.pending | The indicated booking is in reaccommodation proccess. |
| 502 Bad Gateway | Agent.DefaultEmail.NotConfigured | The informed agent does not have a configured default email. |
| 502 Bad Gateway | Agent.NotActive | The Agent is not active. |
| 502 Bad Gateway | AuthorizationFailed.Credentials | Username or password is incorrect. |
| 502 Bad Gateway | Blacklisted.Card | The used credit card is blacklisted, please select another one to pay this order. |
| 502 Bad Gateway | Comarch.RequestFailed | An error occurred while retrieving the data in the commarch. |
| 502 Bad Gateway | Integration.Error | ServiceBus connection error! |
| 502 Bad Gateway | Integration.Failed | The request failed. |
| 502 Bad Gateway | Integration.InvalidFare | There is an error within the requested fares |
| 502 Bad Gateway | Integration.InvalidField.CurrencyCode | The 'CurrencyCode' is invalid. |
| 502 Bad Gateway | InvalidField.Account | The 'Account' is invalid. |
| 502 Bad Gateway | InvalidField.Amount | The 'Amount' value must be equal or greater than zero. |
| 502 Bad Gateway | InvalidField.CountryCode | The 'CountryCode' must have 2 characters. |
| 502 Bad Gateway | InvalidField.CurrencyCode.Length | The 'CurrencyCode' has a maximum length of 3 characters. |
| 502 Bad Gateway | InvalidField.DepartureDate | Arrival date may not be before Departure date. |
| 502 Bad Gateway | InvalidField.Destination.Length | The 'Destination' station code has a maximum length of 3 characters. |
| 502 Bad Gateway | InvalidField.FareKey | The 'FareAvailabilityKey' is invalid! |
| 502 Bad Gateway | InvalidField.Installments | The 'Installments' cannot be zero or null. |
| 502 Bad Gateway | InvalidField.MethodCode.Length | The 'MethodCode' must be 2 characters. |
| 502 Bad Gateway | InvalidField.Miscelaneous.Length | Check the length of fields 'GovId, AccountHolderName and VerificationCode'. |
| 502 Bad Gateway | InvalidField.Organization | The 'Organization' is invalid! |
| 502 Bad Gateway | InvalidField.OrganizationCode | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. |
| 502 Bad Gateway | InvalidField.OrganizationCode.Length | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. |
| 502 Bad Gateway | InvalidField.PassengerType.Length | The 'Passengers.Type' has a maximum length of 3 characters. |
| 502 Bad Gateway | InvalidField.Password | The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. |
| 502 Bad Gateway | InvalidField.PromotionCode | The 'PromotionCode' is invalid! |
| 502 Bad Gateway | InvalidField.PromotionCode.Length | The 'PromotionCode' has a maximum length of 8 characters. |
| 502 Bad Gateway | Navitaire.Authenticated.NoAgentRoles | Unable to find valid role for agent. |
| 502 Bad Gateway | Navitaire.Authenticated.Session | An agent is already authenticated. |
| 502 Bad Gateway | Navitaire.GetBooking.Failed | The requested order was not found or does not exist. |
| 502 Bad Gateway | Navitaire.Request.Failed | The request failed with navitaire. |
| 502 Bad Gateway | Navitaire.SeatKey.Invalid | Invalid seat key for equipment. |
| 502 Bad Gateway | Navitaire.SegmentKey.Invalid | The 'SegmentKey' is invalid. |
| 502 Bad Gateway | Order.RequestFailed | An error has ocurred retrieving the order from state. |
| 502 Bad Gateway | Order.RequestFailed.Credits | An error occurred while searching for credit. |
| 502 Bad Gateway | Order.RequestFailed.InsufficientFunds | Not enough funds available. |
| 502 Bad Gateway | Order.RequestFailed.NoFunds | The Order in state has no funds. |
| 502 Bad Gateway | Order.RequestFailed.NotUpdated | Unable to update booking. |
| 502 Bad Gateway | Organization.AuthorizationFailed.User | This user does not have access to the informed organization. |
| 502 Bad Gateway | Organization.NotActive | The Organization is not active. |
| 502 Bad Gateway | Passengers.Count.OverMaximum | The sum of adult and child passenger must be less than or equal to 9. |
| 502 Bad Gateway | Passengers.Count.UnderMinimum | The minimum count of 'Passenger' array is 1. |
| 502 Bad Gateway | Payment.Appoval.fail | The payment flow was not finalized yet. |
| 502 Bad Gateway | RequestFailed | The request failed. |
| 502 Bad Gateway | RequestFailed.AssistanceCode.NotAllowed | The informed assistance code is invalid or cannot be added to this journey. |
| 502 Bad Gateway | RequestFailed.Authentication | An error occurred while validating the user authentication. |
| 502 Bad Gateway | RequestFailed.ChangeNotAllowed | The requested journey cannot be changed. |
| 502 Bad Gateway | RequestFailed.Comarch | An error occurred while retrieving the data in the comarch. |
| 502 Bad Gateway | RequestFailed.CompletedPayment | The amounts for this order have already been totally paid. |
| 502 Bad Gateway | RequestFailed.ContactError | Your Order request was succefully processed, but the informed booking contact has errors. |
| 502 Bad Gateway | RequestFailed.DeletingError | An error occurred when deleting the order. |
| 502 Bad Gateway | RequestFailed.GetPayment | There was an error retrieving the payment. |
| 502 Bad Gateway | RequestFailed.IncompletePayment | The Payment must include at least the total amount of the order taxes. |
| 502 Bad Gateway | RequestFailed.Installments | Installment payment available only for BRL currency code. |
| 502 Bad Gateway | RequestFailed.NotAuthenticated | An error occurred while authenticating. |
| 502 Bad Gateway | RequestFailed.Order.AlreadyExistsInState | There is already an order created in state. |
| 502 Bad Gateway | RequestFailed.OrderPayments | The order in the current state has not been checked out yet. The CreditType 'Order' only applies to created orders. |
| 502 Bad Gateway | RequestFailed.OverPayment | The informed amount is greater than the balance due for this order. |
| 502 Bad Gateway | RequestFailed.Payments | An error occurred with the order payments service. |
| 502 Bad Gateway | RequestFailed.SSR.AddNotPossible | It was not possible to add an SSR to the order. |
| 502 Bad Gateway | RequestFailed.StatusAccount | Organization account is Closed/Blocked, please contact Azul's commercial team. |
| 502 Bad Gateway | RequestFailed.UnaccompaniedMinor.Information | There are unaccompanied minors in your order, please verify possible costs and required documentations. |
| 502 Bad Gateway | RequestFailed.Unexpected | An unexpected error has occurred. |
| 502 Bad Gateway | RequiredField.Amount | The 'Amount' is required. |
| 502 Bad Gateway | RequiredField.CreditCard.MethodCode | The 'MethodCode' is required. |
| 502 Bad Gateway | RequiredField.Departure | The 'Departure' is required. |
| 502 Bad Gateway | RequiredField.FareKey | The 'FareKey' is required. |
| 502 Bad Gateway | RequiredField.JourneyKey | The 'JourneyKey' is required. |
| 502 Bad Gateway | RequiredField.OrganizationCode | The 'OrganizationCode' is required. |
| 502 Bad Gateway | RequiredField.PassengerType | The 'Passenger.Type' is required. |
| 502 Bad Gateway | Resources.RequestFailed | The Resources request failed. |
| 502 Bad Gateway | FrequentFlyer.Inconsistent | The passenger's name in the frequent flyer registration is different from the reservation system, please contact frequent flyer support. |
| 502 Bad Gateway | UserOrganization.NotAllowed | The logged user organization does not have access to the requested order. |
| 502 Bad Gateway | InternalSession.Failed | An internal error has occurred and the process is unrecoverable, please retrieve again to restart the process. |
