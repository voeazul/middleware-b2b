# Error Codes and Messages

Our Middleware has several rules and procedures to guarantee the integrity of the flow. All HTTP response codes, possible error codes and their respective error messages are mapped below:

## General Errors

|	 HTTP Code       	|	 Internal Code   	|	 Error Message                               	|
|	 ----------------- 	|	 -------------- 	|	 ---------------------------------------------- 	|
|	 400 Bad Request 	|	 AgentOrder.NotAuthorized 	|	 Agent is not authorized to commit order with invalid price status without requesting to override restrictions. 	|
|	 400 Bad Request 	|	 AuthorizationFailed.Credentials 	|	 An error occurred while authenticating. 	|
|	 400 Bad Request 	|	 CustomProgram.NotMatch 	|	 Passenger name does not match within informed Customer Program. 	|
|	 400 Bad Request 	|	 Dates.Range.OverMaximum 	|	 The difference in days between 'DepartureBegin' and 'DepartureEnd' cannot be greater than {0} days. 	|
|	 400 Bad Request 	|	 DiscountPayment.TudoAzul 	|	 A discount have been applied to your order for using a TudoAzul card. 	|
|	 400 Bad Request 	|	 FlexibleDays.Disabled 	|	 Unable to get flexible days because this feature is disabled. 	|
|	 400 Bad Request 	|	 Infant.Request.Failed 	|	 There was an error sending the passenger document. 	|
|	 400 Bad Request 	|	 Integration.EnterpriseStation 	|	 An error occurred while returning the stations. 	|
|	 400 Bad Request 	|	 Integration.Error 	|	 The informed 'RecordLocator' is invalid! 	|
|	 400 Bad Request 	|	 InvalidField.Account 	|	 The 'Account' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.Account.Length 	|	 The 'Account' has a maximum length of 16 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.City 	|	 The 'Address.City' has a maximum of 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.Country 	|	 The 'Address.CountryCode' has a maximum of 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.LineOne 	|	 The 'Address.LineOne' has a maximum of 128 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.LineThree 	|	 The 'Address.LineThree' has a maximum of 128 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.LineTwo 	|	 The 'Address.LineTwo' has a maximum of 128 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.PostalCode 	|	 The 'Address.PostalCode' has a maximum of 10 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Address.ProvinceState 	|	 The 'Address.ProvinceState' has a maximum of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Amount 	|	 The 'Amount' value must be equal or greater than zero. 	|
|	 400 Bad Request 	|	 InvalidField.AssistanceArray 	|	 The minimum count of 'Assistances' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.AssistanceCode 	|	 The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. 	|
|	 400 Bad Request 	|	 InvalidField.AssistancesCount 	|	 The 'Assistances.Count' must be greather than 0. 	|
|	 400 Bad Request 	|	 InvalidField.BaggageAllowance 	|	 The 'BaggageAllowance' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.Bin 	|	 The 'BIN' is not a valid number. 	|
|	 400 Bad Request 	|	 InvalidField.Bin.Length 	|	 The 'BIN' must be of 6 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Code 	|	 The 'Code' must have a maximum of 4 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Codes 	|	 The minimum count of 'Codes' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.Contact.AddressCity 	|	 The 'Contact.Address.City' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Contact.CompanyName 	|	 The 'Contact.CompanyName' has a maximum of 64 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Contact.Email 	|	 The 'Contact.Email' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.Contact.FirstName 	|	 The 'Name.First' has a maximum of 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Contact.LastName 	|	 The 'Name.Last' has a maximum of 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddress.LineOne 	|	 The 'Contact.Address.LineOne' has a maximum length 52 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddress.LineThree 	|	 The 'Contact.Address.LineThree' has a maximum length 52 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddress.LineTwo 	|	 The 'Contact.Address.LineTwo' has a maximum length 52 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddress.PostalCode 	|	 The 'Contact.Address.PostalCode' has a maximum length 10 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddress.ProviceState 	|	 The 'Contact.Address.ProvinceState' has a maximum length 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactAddressLineCountry 	|	 The 'Contact.Address.Country' has a maximum length 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactName.First 	|	 The 'Contact.Name.First' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactName.Last 	|	 The 'Contact.Name.Last' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactName.Middle 	|	 The 'Contact.Name.Middle' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactName.Suffix 	|	 The 'Contact.Name.Suffix' must be a valid enum. 	|
|	 400 Bad Request 	|	 InvalidField.ContactNameT.itle 	|	 The 'Contact.Name.Title' must be a valid enum. 	|
|	 400 Bad Request 	|	 InvalidField.ContactPhones.Number 	|	 The 'Contact.Phones.Number' has a maximum length 20 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ContactPhones.Type 	|	 The 'Contact.Phones.Type' must be a valid enum. 	|
|	 400 Bad Request 	|	 InvalidField.Count.Infant 	|	 The 'ADT' type passenger count must be greater than 'INF' type passenger count. 	|
|	 400 Bad Request 	|	 InvalidField.Count.OverMaximum 	|	 The sum of 'Passengers.Count' of type ADT and CHD must be less than or equal to {0} passengers. 	|
|	 400 Bad Request 	|	 InvalidField.Count.UnderMinimum 	|	 The minimum value of 'Passengers.Count' is 1. 	|
|	 400 Bad Request 	|	 InvalidField.CountryCode 	|	 An error occurred while requesting order. 	|
|	 400 Bad Request 	|	 InvalidField.CreditAmount.Empty 	|	 The 'CreditAmount' value must be greater than zero. 	|
|	 400 Bad Request 	|	 InvalidField.CriteriaType 	|	 The 'CriteriaType' must be an valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.customerProgram.number 	|	 Letters are not allowed. 	|
|	 400 Bad Request 	|	 InvalidField.CustomerProgram.Number 	|	 The 'Passengers.CustomerProgram.Number' has a maximum lenght of 20 characters. 	|
|	 400 Bad Request 	|	 InvalidField.DateOfBirth 	|	 Passengers under 18 years old are not allowed with infant. 	|
|	 400 Bad Request 	|	 InvalidField.DepartureBegin 	|	 The 'DepartureBegin' must be greater than today's date. 	|
|	 400 Bad Request 	|	 InvalidField.DepartureEnd 	|	 The 'DepartureBegin' must be greater than 'DepartureEnd'. 	|
|	 400 Bad Request 	|	 InvalidField.Destination.Length 	|	 The 'Destination' station code has a maximum length of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.EquipmentCode 	|	 The 'EquipmentCode' must have a maximum of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ExpirationDate 	|	 Invalid credit card expiration date. 	|
|	 400 Bad Request 	|	 InvalidField.ExpirationMonth 	|	 The 'ExpirationMonth' must be empty when MethodCode is {0} 	|
|	 400 Bad Request 	|	 InvalidField.ExpirationYear 	|	 The 'ExpirationYear' must be empty when MethodCode is {0} 	|
|	 400 Bad Request 	|	 InvalidField.FareKey 	|	 The 'FareKey' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.FeeCode 	|	 The 'FeeCode' must have a maximum of 6 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Filter 	|	 Can only be filtered by 'Username' or 'FirstName'. 	|
|	 400 Bad Request 	|	 InvalidField.FirstName.Length 	|	 The 'FirstName' must be a string with a maximum length of 128. 	|
|	 400 Bad Request 	|	 InvalidField.FirstNameMatching 	|	 The 'FirstNameMatching' cannot be entered with 'Username'. 	|
|	 400 Bad Request 	|	 InvalidField.FlexibleDays.Ahead 	|	 The minimum value of 'FlexibleDays.Ahead' is {0}. 	|
|	 400 Bad Request 	|	 InvalidField.FlexibleDays.Behind 	|	 The minimum value of 'FlexibleDays.Behind' is {0}. 	|
|	 400 Bad Request 	|	 InvalidField.FlightNumber 	|	 Some segments for the Journey '{0}-{1} - {2}' do not support the assistance '{3}'. Please contact the customer service to complete the special assistance process. 	|
|	 400 Bad Request 	|	 InvalidField.GovId 	|	 The 'GovId' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.GovId.Length 	|	 The 'GovId' has a maximum length of 11 characters. 	|
|	 400 Bad Request 	|	 InvalidField.HolderName 	|	 The 'HolderName' must be empty when MethodCode is {0} 	|
|	 400 Bad Request 	|	 InvalidField.HolderName.Length 	|	 The 'HolderName' has a maximum length of 255 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Infant.DateOfBirth 	|	 The 'Infant.DateOfBirth' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.Infant.Nationality 	|	 The 'Infant.Nationality' has a maximum of 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Installments 	|	 The 'Installments' cannot be zero or null. 	|
|	 400 Bad Request 	|	 InvalidField.IropContact.Email 	|	 The 'Passengers.IropContact.Email' has a maximum length 128 characters. 	|
|	 400 Bad Request 	|	 InvalidField.IropContact.Mobile 	|	 The 'Passengers.IropContact.Mobile' cannot be informed when Passengers.IropContact.Refused is True. 	|
|	 400 Bad Request 	|	 InvalidField.Journey 	|	 The Journey.Key '{0}' is duplicated. 	|
|	 400 Bad Request 	|	 InvalidField.Journeys 	|	 The minimum count of 'Journeys' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.Journeys.Count 	|	 The maximum number of Journeys allowed in a order is {0}. 	|
|	 400 Bad Request 	|	 InvalidField.Journeys.OverMaximum 	|	 The number of 'Journeys' must be less than {0}. 	|
|	 400 Bad Request 	|	 InvalidField.Journeys.UnderMinimum 	|	 The number of 'Journeys' must be greater than {0}. 	|
|	 400 Bad Request 	|	 InvalidField.LastName 	|	 The 'LastName' cannot be entered with 'Username'. 	|
|	 400 Bad Request 	|	 InvalidField.LastName.Length 	|	 The 'OrganizationCode' must be a string with a maximum length of 64. 	|
|	 400 Bad Request 	|	 InvalidField.LiableRecordLocator 	|	 The 'LiableRecordLocator' must have 6 characters. 	|
|	 400 Bad Request 	|	 InvalidField.MethodCode 	|	 The 'MethodCode' must be equals to {0}, {1}. 	|
|	 400 Bad Request 	|	 InvalidField.MethodCode.Length 	|	 The 'MethodCode' must be 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.MiddleName.Length 	|	 The 'Name.Middle' has a maximum of 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Name.First 	|	 The 'Name.First' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Name.Last 	|	 The 'Name.Last' has a maximum length 32 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Name.Suffix 	|	 The 'Name.Sufix' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.Name.Title 	|	 The 'Name.Title' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.Nationality.Length 	|	 The 'Nationality' has a maximum length 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.NewPassword 	|	 The 'NewPassword' must be different from the 'CurrentPassword'. 	|
|	 400 Bad Request 	|	 InvalidField.NoFilter 	|	 Filter by 'Username' or 'FirstName'. 	|
|	 400 Bad Request 	|	 InvalidField.Offers 	|	 The minimum count of 'Offers' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.Offers.OverMaximum 	|	 The maximum count of 'offer' array is 4 	|
|	 400 Bad Request 	|	 InvalidField.Offers.UnderMinimum 	|	 The minimum count of 'offer' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.OrganizationCode 	|	 The 'OrganizationCode' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.OrganizationCode.Length 	|	 The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. 	|
|	 400 Bad Request 	|	 InvalidField.OrganizationFeeOverride.Amount 	|	 The 'Amount' value must be equal or greater than zero. 	|
|	 400 Bad Request 	|	 InvalidField.Origin.Length 	|	 The 'Origin' station code has a maximum length of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.PageNumber 	|	 The 'Page' number must be between {0} and {1}. 	|
|	 400 Bad Request 	|	 InvalidField.PageSize 	|	 The 'PageSize' number must be between {0} and {1}. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger 	|	 The minimum count of 'passengers' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.Email 	|	 The 'Passenger.Email' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.IssuingCountry 	|	 The 'InvalidField.Passenger.IssuingCountry' has a maximum of 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.Name 	|	 The 'Passengers.Name' is required. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.Nationality 	|	 The 'Passenger.Nationality' has a maximum of 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.OverMaximum 	|	 The maximum count of 'Passenger' array is 3. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.Phone 	|	 The 'PassengerAddress.Phone' has a maximum of 20 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.Type 	|	 The 'PassengerRequest.PassengerTypeCode' has a maximum of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Passenger.UnderMinimum 	|	 The minimum count of 'Passenger' array is 1. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerAddress.CultureCode 	|	 The 'PassengerAddress.CultureCode' has a maximum of 17 characters. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerAddress.StationCode 	|	 The 'PassengerAddress.StationCode' has a minimum of 3 and a maximum of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerCount.UnderMinimum 	|	 The 'Passengers.Count' must be greater than 0. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerKeys.Empty 	|	 The 'PassengerKeys' array cannot contain empty values. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerType 	|	 The 'Passengers.Type' must be equal to 'ADT', 'CHD' or 'INF'. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerType.Length 	|	 The 'Passengers.Type' has a maximum length of 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.PassengerType.Repeated 	|	 Must only have one 'Passenger.Type' of type ADT. 	|
|	 400 Bad Request 	|	 InvalidField.Password 	|	 The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. 	|
|	 400 Bad Request 	|	 InvalidField.ProductClass 	|	 The 'ProductClass' must have a maximum of 2 character. 	|
|	 400 Bad Request 	|	 InvalidField.ProgramNumber 	|	 The 'ProgramNumber' has a maximum lenght of 20 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Promotion.Code 	|	 The 'PromotionCode' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.PromotionCode 	|	 The 'PromotionCode' is invalid! 	|
|	 400 Bad Request 	|	 InvalidField.PromotionCode.Length 	|	 The 'PromotionCode' has a maximum length of 8 characters. 	|
|	 400 Bad Request 	|	 InvalidField.ProviderType 	|	 The 'ProviderType' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.RecordLocator 	|	 The 'RecordLocator' must have 6 characters. 	|
|	 400 Bad Request 	|	 InvalidField.RefundType 	|	 The 'RefundType' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.ServicesCount 	|	 The 'Services.Count' must be greather than 0. 	|
|	 400 Bad Request 	|	 InvalidField.StationCode 	|	 The 'StationCode' must be 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.TaxAmount 	|	 The 'TaxAmount' must be greater than or equal to 0. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocument.BirthCountry 	|	 The 'TravelDocuments.BirthCountry' has a maximum length 2 characters. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocument.IssuingCountry 	|	 The 'TravelDocuments.IssuingCountry' has a maximum length 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocument.Number 	|	 The 'TravelDocuments.Number' has a maximum length 35 characters. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocument.Type 	|	 The 'TravelDocuments.Type' must be a valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocuments.IssuingCountry 	|	 The 'TravelDocuments.IssuingCountry' has a maximum length 3 characters. 	|
|	 400 Bad Request 	|	 InvalidField.TravelDocuments.Type 	|	 The 'TravelDocuments.Type' has a maximum of 4 characters. 	|
|	 400 Bad Request 	|	 InvalidField.Type 	|	 The 'Type' must be an valid Enum. 	|
|	 400 Bad Request 	|	 InvalidField.Username.Length 	|	 The 'Username' must be a string with a maximum length of 128. 	|
|	 400 Bad Request 	|	 InvalidField.UsernameMatching 	|	 The 'UsernameMatching' cannot be entered with 'FirstName'. 	|
|	 400 Bad Request 	|	 InvalidField.VerificationCode 	|	 The 'VerificationCode' is invalid. 	|
|	 400 Bad Request 	|	 InvalidField.VerificationCode.Length 	|	 The 'VerificationCode' has a maximum length of 4 characters. 	|
|	 400 Bad Request 	|	 JourneyKey.Decoding.Error 	|	 An error occurred while decoding a JourneyKey. 	|
|	 400 Bad Request 	|	 Journeys.Overlap 	|	 There are journeys overlapping. 	|
|	 400 Bad Request 	|	 LiableRecordLocator.UnaccompaniedMinor.Issuing 	|	 The 'LiableRecordLocator' can only be informed for issuing an order with unaccompanied minors. 	|
|	 400 Bad Request 	|	 Loyalty.Request.Failed 	|	 The Loyalty request failed. 	|
|	 400 Bad Request 	|	 Market.Unavailable 	|	 The informed origin/destination market are currently unavailable for low fare estimate search. 	|
|	 400 Bad Request 	|	 Navitaire.SeatCreate.Failed 	|	 The request failed to assign seat. 	|
|	 400 Bad Request 	|	 NotAvailable.Credit 	|	 The informed 'RecordLocator' has no credit available. 	|
|	 400 Bad Request 	|	 Offer.UnaccompaniedMinor.AdditionalFees 	|	 Unaccompanied minor may incur additional fee, according to company policy. 	|
|	 400 Bad Request 	|	 Order.Calculation.NotPending 	|	 The order in the state has no calculations to be done. 	|
|	 400 Bad Request 	|	 Order.Journeys.Count 	|	 The maximum number of Journeys allowed in a order is {0}. 	|
|	 400 Bad Request 	|	 Order.PendingCalculation 	|	 There are pending calculations to be performed. Call the order calculate method before confirming your order changes. 	|
|	 400 Bad Request 	|	 Order.State.Timeout 	|	 The state time for this order has expired. Please retrieve the order again with the GET Order method. 	|
|	 400 Bad Request 	|	 OrderDivide.BalanceDue.Positive 	|	 The order in state has a positive balance due. 	|
|	 400 Bad Request 	|	 OrderDivide.CreditAmount.invalid 	|	 The informed 'creditAmount' is invalid because it's greater than the amount available in the informed order. 	|
|	 400 Bad Request 	|	 OrderDivide.DivideCredit.Failed 	|	 An error occurred while dividing the order credit. Credit values have not been divided or changed, remaining entirely in the parent order. 	|
|	 400 Bad Request 	|	 OrderDivide.PassengerKeys.InvalidAmount 	|	 The number of 'passengerKeys' in the request must be less than the number of passengers in the informed order. 	|
|	 400 Bad Request 	|	 OrderDivide.Payments.Empty 	|	 The order in state does not have informed payments. 	|
|	 400 Bad Request 	|	 OrderDivide.Unaccompanied.NotAllowed 	|	 It's not allowed to divide an order when it will result in orders where there are only unaccompanied minors (under {0} years old). Both involved orders must contain at least one adult passenger (ADT) over {0} years of age at the end of the division. 	|
|	 400 Bad Request 	|	 Organization.Request.Failed 	|	 The Organization request failed. 	|
|	 400 Bad Request 	|	 Passenger.DocumentTypeMatch.NotAllowed 	|	 Multiple Passengers with the same Travel Document Type and Number are not allowed, including Infants. 	|
|	 400 Bad Request 	|	 Passenger.InvalidAge 	|	 Passenger under 12 years old on the departure date cannot be considered an adult (ADT). 	|
|	 400 Bad Request 	|	 Passenger.NameMatch.NotAllowed 	|	 Multiple Passengers with exactly the same First Name, Middle Name, Last Name and Suffix are not allowed, including Infants. 	|
|	 400 Bad Request 	|	 Passenger.TraveDocument.Expired 	|	 Informed travel document will be expired on the departure date. 	|
|	 400 Bad Request 	|	 Passenger.Unaccompanied.InvalidAge 	|	 Minors must be over 8 years old to travel unaccompanied. 	|
|	 400 Bad Request 	|	 Payments.Credit.Failed 	|	 An error occurred while using the credit. 	|
|	 400 Bad Request 	|	 Payments.ValidationError 	|	 Checkout validation error. Payments amount does not match the total cost of the order. 	|
|	 400 Bad Request 	|	 Quote.UnaccompaniedMinor.NotAllowed 	|	 The 'JourneyKeys' {0} does not allow unaccompanied minors. 	|
|	 400 Bad Request 	|	 RequestFailed.CreditCard.Expired 	|	 Expired credit card. 	|
|	 400 Bad Request 	|	 RequestFailed.Enterprise 	|	 An error occurred while validating order passengers names. 	|
|	 400 Bad Request 	|	 RequestFailed.International.Required 	|	 The organization fee override is only allowed for orders with international journeys. 	|
|	 400 Bad Request 	|	 RequestFailed.Journeys.NotAllowed 	|	 The organization fee override is only allowed while adding new journeys to the order. 	|
|	 400 Bad Request 	|	 RequestFailed.PassengerMinor.NotAllowedInfants 	|	 Passengers under 18 years old are not allowed to have infants. 	|
|	 400 Bad Request 	|	 RequestFailed.Passengers.WithoutFee 	|	 No passengers in this order have organization fees charged. 	|
|	 400 Bad Request 	|	 RequestFailed.TudoAzul.Retrieve 	|	 An error occurred while retrieving the TudoAzul program. 	|
|	 400 Bad Request 	|	 RequestFailed.Unexpected 	|	 An unexpected error has occurred. 	|
|	 400 Bad Request 	|	 RequiredField.Account 	|	 The 'Account' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Amount 	|	 The 'Amount' is required. 	|
|	 400 Bad Request 	|	 RequiredField.AssistanceArray 	|	 The 'Assistances' array is required. 	|
|	 400 Bad Request 	|	 RequiredField.AssistancesCount 	|	 The 'Assistances.Count' is required. 	|
|	 400 Bad Request 	|	 RequiredField.AssistancesKey 	|	 The 'Assistances.Key' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Code 	|	 The 'Code' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Contact.FirstName 	|	 The 'Contact.FirstName' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Contact.LastName 	|	 The 'Contact.LastName' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Contact.Phones 	|	 The 'Contact.Phones' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactAddress.LineOne 	|	 The 'Contact.Address.LineOne' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactName 	|	 The 'Contact.Name' object is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactName.First 	|	 The 'Contact.Name.First' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactName.Last 	|	 The 'Contact.Name.Last' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactPhones.Number 	|	 The 'Contact.Phones.Number' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactPhones.Type 	|	 The 'Contact.Phones.Type' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ContactPhonesHome 	|	 The 'Contact.Phones' a home object is required. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.ExpirationMonth 	|	 The 'ExpirationMonth' is required. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.ExpirationYear 	|	 The 'ExpirationYear' is required. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.GovId 	|	 The 'GovId' is required for this method code due to the currency code of the order. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.HolderName 	|	 The 'HolderName' is required. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.MethodCode 	|	 The 'MethodCode' is required. 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.Type 	|	 The 'CreditCard.Type' is required 	|
|	 400 Bad Request 	|	 RequiredField.CreditCard.VerificationCode 	|	 The 'VerificationCode' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Criteria 	|	 The 'Criteria' is only required for 'CriteriaType': 'Phone', 'Email', 'DocumentNumber', 'CardNumber' and 'CustomerNumber'. 	|
|	 400 Bad Request 	|	 RequiredField.CriteriaType 	|	 The 'CriteriaType' is only required for 'Type': 'Organization'. 	|
|	 400 Bad Request 	|	 RequiredField.CurrencyCode 	|	 The 'CurrencyCode' is required. 	|
|	 400 Bad Request 	|	 RequiredField.CurrentPassword 	|	 User not authenticated. The field 'Username' is required. 	|
|	 400 Bad Request 	|	 RequiredField.DateOfBirth 	|	 The 'DateOfBirth' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Departure 	|	 The 'Departure' is required. 	|
|	 400 Bad Request 	|	 RequiredField.DepartureBegin 	|	 The 'DepartureBegin' is required. 	|
|	 400 Bad Request 	|	 RequiredField.DepartureDate 	|	 The 'Departure' is required. 	|
|	 400 Bad Request 	|	 RequiredField.DepartureEnd 	|	 The 'DepartureEnd' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Destination 	|	 The 'Destination' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Document.Type 	|	 The 'Infant.Document.Type' CPF, RNE or PASSPORT is required. 	|
|	 400 Bad Request 	|	 RequiredField.DocumentType 	|	 The 'DocumentType' is required for the informed 'CriteriaType'. 	|
|	 400 Bad Request 	|	 RequiredField.FareKey 	|	 The 'FareKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.FirstName 	|	 The 'FirstName' is required for the 'FirstNameMatching' field. 	|
|	 400 Bad Request 	|	 RequiredField.FirstNameMatching 	|	 The 'FirstNameMatching' is required for the 'FirstName' field. 	|
|	 400 Bad Request 	|	 RequiredField.Gender 	|	 The 'Gender' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Infant.FirstName 	|	 The 'Infant.FirstName' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Infant.Gender 	|	 The 'Infant:Gender' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Infant.LastName 	|	 The 'Infant.LastName' is required. 	|
|	 400 Bad Request 	|	 RequiredField.IropContact 	|	 The 'Passengers.IropContact' is required. 	|
|	 400 Bad Request 	|	 RequiredField.IropContact.EmailMobile 	|	 The 'Passengers.IropContact.Email' or 'Passengers.IropContact.Mobile is required. 	|
|	 400 Bad Request 	|	 RequiredField.IropContact.Refused 	|	 The 'Passengers.IropContact.Refused' is required. 	|
|	 400 Bad Request 	|	 RequiredField.JourneyKey 	|	 The 'JourneyKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Journeys 	|	 The 'Journeys' array is required. 	|
|	 400 Bad Request 	|	 RequiredField.Key 	|	 The 'Key' is required. 	|
|	 400 Bad Request 	|	 RequiredField.LastName 	|	 The 'LastName' is only required for 'CriteriaType': 'PassengerName' or 'ContactName'. 	|
|	 400 Bad Request 	|	 RequiredField.Name 	|	 The 'Name' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Name.First 	|	 The 'Name.First' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Name.Last 	|	 The 'Name.Last' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Name.Middle 	|	 The 'Name.Middle' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Nationality 	|	 The 'Nationality' is required. 	|
|	 400 Bad Request 	|	 RequiredField.NewPassword 	|	 The 'NewPassword' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Offers 	|	 The 'Offers' array is required. 	|
|	 400 Bad Request 	|	 RequiredField.Offers.FareKey 	|	 The 'Offers.FareKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Offers.JourneyKey 	|	 The 'Offers.JouneyKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.OrganizationCode 	|	 The 'OrganizationCode' is required. 	|
|	 400 Bad Request 	|	 RequiredField.OrganizationGroupCode 	|	 The 'OrganizationGroupCode' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Origin 	|	 The 'Origin' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger 	|	 The 'Passenger' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger.DateOfBirth 	|	 The 'Passenger.DateOfBirth' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger.Gender 	|	 The 'Passenger.Gender' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger.Key 	|	 The 'PassengerKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger.PhoneEmail 	|	 The 'Passengers.Phone' or  'Passengers.Email' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Passenger.Type 	|	 The 'Passengers.Type' is required. 	|
|	 400 Bad Request 	|	 RequiredField.PassengerKey 	|	 The 'PassengerKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.PassengerKeys 	|	 The 'passengerKeys' informed in the request does not exist in the informed order. 	|
|	 400 Bad Request 	|	 RequiredField.Passengers 	|	 The 'Passengers' array is required. 	|
|	 400 Bad Request 	|	 RequiredField.PassengerType 	|	 The 'Passenger.Type' is required. 	|
|	 400 Bad Request 	|	 RequiredField.PassengerType.Adult 	|	 The 'Passengers.Type' a ADT value is required. 	|
|	 400 Bad Request 	|	 RequiredField.Password 	|	 The 'Password' is required. 	|
|	 400 Bad Request 	|	 RequiredField.PhonesNumber 	|	 The 'Phones.Number' is required. 	|
|	 400 Bad Request 	|	 RequiredField.PhonesType 	|	 The 'Phones.Type' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ProviderType 	|	 The 'ProviderType' is required. 	|
|	 400 Bad Request 	|	 RequiredField.RecordLocator 	|	 The 'RecordLocator' is required. 	|
|	 400 Bad Request 	|	 RequiredField.SegmentKey 	|	 The 'segmentkey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Services 	|	 The 'Services' list is required. 	|
|	 400 Bad Request 	|	 RequiredField.ServicesCount 	|	 The 'Services.Count' is required. 	|
|	 400 Bad Request 	|	 RequiredField.ServicesKey 	|	 The 'Services.Key' is required. 	|
|	 400 Bad Request 	|	 RequiredField.SessionContext 	|	 The 'SessionContext' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Status 	|	 The 'Status' is required. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocument 	|	 The minimum count of 'TravelDocument' array is 1. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocument.ExpirationDate 	|	 The 'TravelDocuments.ExpirationDate' is required. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocument.Number 	|	 The 'TravelDocuments.Number' is required. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocument.Type 	|	 The 'TravelDocuments.Type' CPF, RNE or PASSPORT is required. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocuments.IssuingCountry 	|	 The 'TravelDocuments.IssuingCountry' is required. 	|
|	 400 Bad Request 	|	 RequiredField.TravelDocuments.Type 	|	 The 'TravelDocuments.Type' is required. 	|
|	 400 Bad Request 	|	 RequiredField.UnitKey 	|	 The 'unitkey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.UserKey 	|	 The 'UserKey' is required. 	|
|	 400 Bad Request 	|	 RequiredField.Username 	|	 The 'Username' is required. 	|
|	 400 Bad Request 	|	 Shopping.Request.Failed 	|	 The Shopping request failed. 	|
|	 400 Bad Request 	|	 Stations.NotAllowed 	|	 These requested stations are invalid: 	|
|	 400 Bad Request 	|	 TudoAzul.Categorization.Failed 	|	 There was a failure in the categorization of TudoAzul of 'passengers.customerProgram.number': {0}. Try categorize again after the order creation (before assigning seats or adding baggages to ensure all potential benefits). 	|
|	 400 Bad Request 	|	 User.CannotBeUnlocked 	|	 Only API users can be unlocked. 	|
|	 400 Bad Request 	|	 User.Password.Expired 	|	 Expired password, user must change password. 	|
|	 400 Bad Request 	|	 Warning.OrganizationFeeOverride 	|	 Organization fee override is not applicable for this order. 	|
|	 401 Unauthorized 	|	 InvalidToken.Expired 	|	 An error occurred while performing authentication. 	|
|	 401 Unauthorized 	|	 InvalidToken.NotAuthenticated 	|	 The Bearer Token provided is invalid or expired. 	|
|	 401 Unauthorized 	|	 RequestFailed.Authentication 	|	 An error occurred while authenticating. 	|
|	 403 Forbidden 	|	 Agent.NoAccess 	|	 The agent does not have access to the informed user. 	|
|	 403 Forbidden 	|	 AssignSeat.UnitKey.Blocked 	|	 The request failed to assign the seat, because this seat is blocked by passengers rules (age, SSR or equipment). 	|
|	 403 Forbidden 	|	 Organization.AuthorizationFailed.User 	|	 This user does not have access to the informed organization. 	|
|	 404 Not Found 	|	 Assistance.NoMatches 	|	 This assistance does not exist or was not found. 	|
|	 404 Not Found 	|	 Assistances.NoMatches 	|	 Assistance not found in the specified journey. 	|
|	 404 Not Found 	|	 AssistancesKey.NoMatches 	|	 The informed 'Assistances.Key' does not exists or does not belong to a previously retrieved 'assistance/search'. 	|
|	 404 Not Found 	|	 BagKey.NoMatches 	|	 The informed 'Key' does not exists or does not belong to a previously retrieved 'baggage/search'. 	|
|	 404 Not Found 	|	 Code.NoMatches 	|	 The informed service is invalid. 	|
|	 404 Not Found 	|	 Countries.NoMatches 	|	 Unable to retrieve the countries data. 	|
|	 404 Not Found 	|	 Country.NoMatches 	|	 This country does not exist or was not found. 	|
|	 404 Not Found 	|	 CreditNoMatches 	|	 There is no credit available for the informed type. 	|
|	 404 Not Found 	|	 CustomerNumber.NoMatches 	|	 The 'CustomerProgram' not found. 	|
|	 404 Not Found 	|	 CustomerProgram.NoMatches 	|	 The Customer Program was not found. 	|
|	 404 Not Found 	|	 Equipment.NoMatches 	|	 This equipament does not exist or was not found. 	|
|	 404 Not Found 	|	 Fare.NoMatches 	|	 This fare does not exist or was not found. 	|
|	 404 Not Found 	|	 Fares.NoMatches 	|	 Unable to retrieve the fares data. 	|
|	 404 Not Found 	|	 Fee.NoMatches 	|	 This fee does not exist or was not found. 	|
|	 404 Not Found 	|	 Fees.NoMatches 	|	 Unable to retrieve the fees data. 	|
|	 404 Not Found 	|	 InvalidField.JourneyKey 	|	 The 'JourneyKey' is invalid. 	|
|	 404 Not Found 	|	 JourneyKey.NoMatches 	|	 The 'JourneyKey' is invalid or does not exists in the current state. 	|
|	 404 Not Found 	|	 JourneyKey.NotFound 	|	 The 'JourneyKey' not found. 	|
|	 404 Not Found 	|	 NoMatches 	|	 The informed user does not exist or was not found. 	|
|	 404 Not Found 	|	 Order.NoMatches 	|	 The requested order was not found or does not exist. 	|
|  404 Not Found  |  Order.RetrieveRequired | No order found in state. |
|	 404 Not Found 	|	 OrderCache.NoMatches 	|	 An order must be attached. 	|
|	 404 Not Found 	|	 OrderSearch.NoMatches 	|	 No orders found for the informed search filters. 	|
|	 404 Not Found 	|	 Organization.NoMatches 	|	 The informed organization is invalid or the logged user does not have permission to use it! 	|
|	 404 Not Found 	|	 OrganizationGroup.NoMatches 	|	 The informed organization group does not exist or was not found. 	|
|	 404 Not Found 	|	 PassengerKey.NoMatches 	|	 The informed 'PassengerKey' does not match within those on the order in state. 	|
|  404 Not Found  |  PassengerFeeKey.NotFound | The 'PassengerFeeKey' not found. |
|	 404 Not Found 	|	 PassengerName.NoMatches 	|	 The Passenger does not match TudoAzul customer number. 	|
|	 404 Not Found 	|	 Payments.NoMatches 	|	 No payments were found for the order in state. 	|
|	 404 Not Found 	|	 RecordLocator.NoMatches 	|	 Your order must be created to use its credits. 	|
|  404 Not Found  |  RecordLocator.NotFound | The 'RecordLocator' not found. |
|	 404 Not Found 	|	 Seat.NoMatches 	|	 Seat not found. 	|
|	 404 Not Found 	|	 SeatMap.NoMatches 	|	 No matching seats. 	|
|	 404 Not Found 	|	 SegmentKey.NoMatches 	|	 The 'SegmentKey' is invalid or does not exists in the current state. 	|
|	 404 Not Found 	|	 Service.NoMatches 	|	 Service not found in the specified Journey. 	|
|	 404 Not Found 	|	 ServiceKey.NoMatches 	|	 The informed 'Services.Key' does not exists or does not belong to a previously retrieved 'service/search'. 	|
|	 404 Not Found 	|	 SessionContextToken.NoMatches 	|	 No sessions found for the given provider. 	|
|	 404 Not Found 	|	 Station.NoMatches 	|	 This station does not exist or was not found. 	|
|	 404 Not Found 	|	 Stations.NoMatches 	|	 Unable to retrieve the stations data. 	|
|	 404 Not Found 	|	 TudoAzul.NoMatches 	|	 The informed 'passengers.customerProgram.number': {0} does not exists or was not found. 	|
|	 404 Not Found 	|	 TudoAzulNames.NoMatches 	|	 The names of the informed 'passengers.customerProgram.number': {0} do not match those registered in TudoAzul. |
|	 404 Not Found 	|	 UnitKey.NoMatches 	|	 The 'UnitKey' is invalid or does not exists in the current state. 	|
|	 404 Not Found 	|	 User.NoMatches 	|	 The informed user does not exist or was not found. 	|
|  406 Not Found  |  Journey.DepartureDate.Passed | It is not possible to remove a journey whose departure date has already passed. |
|	 409 Conflict 	|	 AssignSeat.PassengerKey.Conflict 	|	 The PassengerKey does not exists in the order state. 	|
|	 409 Conflict 	|	 AssignSeat.Seat.Conflict 	|	 Seat Already Assigned. 	|
|	 409 Conflict 	|	 InvalidField.AssistanceCode 	|	 The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. 	|
|	 409 Conflict 	|	 InvalidField.AssistanceLimit 	|	 The count for the 'Assistances.key' {0} is greater than the specified limit. 	|
|	 409 Conflict 	|	 InvalidField.Assistanceskey 	|	 There are duplicated 'Assistances.key' {0}. 	|
|	 409 Conflict 	|	 InvalidField.PassengerKeyCache 	|	 The requested service is not available for the informed passenger. 	|
|	 409 Conflict 	|	 InvalidField.RecordLocator 	|	 The 'RecordLocator' must have 6 characters. 	|
|	 409 Conflict 	|	 InvalidField.ServiceLimit 	|	 The count for the 'Services.key' {0} is greater than the specified limit. 	|
|	 409 Conflict 	|	 InvalidField.Serviceskey 	|	 There are duplicated 'Services.key' {0}. 	|
|	 409 Conflict 	|	 InvalidToken.Expired 	|	 An error occurred while performing authentication. 	|
|	 409 Conflict 	|	 InvalidToken.NotAuthenticated 	|	 The Bearer Token provided is invalid or expired. 	|
|	 409 Conflict 	|	 LiableRecordLocator.UnaccopaniedMinor.NotMatchJourneys 	|	 Liable order and unaccompanied minors order flights must match. 	|
|	 409 Conflict 	|	 NotEmpty.State 	|	 It's not possible to attach with an order already retrieved in the current state. Please execute an order delete before the order attach. 	|
|	 409 Conflict 	|	 Order.HasRecordLocator 	|	 This method is for orders under creation process. If you want to checkout a previously created order, please use the equivalent method in the Order.Management.Api. 	|
|	 409 Conflict 	|	 Order.Recordlocator.Empty 	|	 This method is for previously created orders. If you want to retrieve an order under creation, please use the equivalent method in the Order.Api. 	|
|	 409 Conflict 	|	 Order.State.Change 	|	 Removing a journey after adding journeys is not allowed. Please confirm your changes or restart the process retrieving the order again. 	|
|	 409 Conflict 	|	 Order.State.Modified 	|	 The order in state has been externally modified. Retrieve the order again with the GET Order methods and try again. 	|
|	 409 Conflict 	|	 Order.UnaccopaniedMinor.OperatedFligthAzul 	|	 Unaccompanied minors are allowed in Azul operated flights only. 	|
|	 409 Conflict 	|	 Order.UnderCreationException 	|	 This method is for orders under creation process. If you want to retrieve a previously created order, please use the equivalent method in the Order.Management.Api. 	|
|	 409 Conflict 	|	 Refund.NotApplicable 	|	 There is no amount in the order to be refunded. 	|
|	 409 Conflict 	|	 RequestFailed.UnaccompaniedMinor.DomesticFligths 	|	 Unaccompanied minors are allowed in brazilian domestic flights only. 	|
|	 409 Conflict 	|	 RequestFailed.UnaccopaniedMinor.OnlyDirectFlight 	|	 Unaccompanied minors are allowed in direct flights only. 	|
|	 409 Conflict 	|	 RequiredField.LiableRecordLocator 	|	 A passenger over 18 years old is required in the liable order. 	|
|	 422 Unprocessable Content 	|	 Assistance.SearchRequired 	|	 Retrieve a 'assistances/search' with journeyKey before execute this method. 	|
|	 422 Unprocessable Content 	|	 Baggage.SearchRequired 	|	 Retrieve a 'baggage/search' with journeyKey before execute this method. 	|
|	 422 Unprocessable Content 	|	 Checkout.V2.Blocked 	|	 This method is not compatible with retrieve order in V2. 	|
|	 422 Unprocessable Content 	|	 NotMatch.Name 	|	 The names sent do not match those on the attached order. 	|
|	 422 Unprocessable Content 	|	 NotMatch.PassengerKey 	|	 An informed passenger key does not exists in the attached order or is invalid. 	|
|	 422 Unprocessable Content 	|	 Order.RetrieveRequired 	|	 The requested order was not found or does not exist. 	|
|	 422 Unprocessable Content 	|	 Order.State.Timeout 	|	 The state time for this order has expired. Please retrieve the order again with the GET Order method. 	|
|	 422 Unprocessable Content 	|	 SeatMapCache.SearchRequired 	|	 No seatmap found or generated in state. Please retrieve a seatmap before trying to assign a seat. 	|
|	 422 Unprocessable Content 	|	 RefundType.CreditsShell.CannotBeApplied 	|	 It is not possible to make the refund using credit shell. 	|
|	 422 Unprocessable Content 	|	 RefundType.Payments.CannotBeApplied 	|	 There are no amounts to be refunded. 	|
|	 422 Unprocessable Content 	|	 Service.SearchRequired 	|	 Retrieve a 'services/search' with journeyKey before execute this method. 	|
|	 422 Unprocessable Content 	|	 UnitKey.SearchRequired 	|	 The informed UnitKey does not belong to a previously retrieved SeatMap or the previous retrive is expired. 	|
|	 502 Bad Gateway 	|	 Agent.DefaultEmail.NotConfigured 	|	 The informed agent does not have a configured default email. 	|
|	 502 Bad Gateway 	|	 Agent.NotActive 	|	 The Agent is not active. 	|
|	 502 Bad Gateway 	|	 AuthorizationFailed.Credentials 	|	 An error occurred while authenticating. 	|
|	 502 Bad Gateway 	|	 B2b.OrderManagementRequest.Failed 	|	 The request failed. 	|
|	 502 Bad Gateway 	|	 Integration.Error 	|	 The informed 'RecordLocator' is invalid! 	|
|	 502 Bad Gateway 	|	 Integration.Failed 	|	 The request failed. 	|
|	 502 Bad Gateway 	|	 Integration.InvalidFare 	|	 There is an error within the requested fares 	|
|	 502 Bad Gateway 	|	 Integration.InvalidField.CurrencyCode 	|	 The 'CurrencyCode' is invalid. 	|
|	 502 Bad Gateway 	|	 InvalidField.Account 	|	 The 'Account' is invalid. 	|
|	 502 Bad Gateway 	|	 InvalidField.Amount 	|	 The 'Amount' value must be equal or greater than zero. 	|
|	 502 Bad Gateway 	|	 InvalidField.CountryCode 	|	 An error occurred while requesting order. 	|
|	 502 Bad Gateway 	|	 InvalidField.CurrencyCode.Length 	|	 The 'CurrencyCode' has a maximum length of 3 characters. 	|
|	 502 Bad Gateway 	|	 InvalidField.DepartureDate 	|	 Arrival date may not be before Departure date. 	|
|	 502 Bad Gateway 	|	 InvalidField.Destination.Length 	|	 The 'Destination' station code has a maximum length of 3 characters. 	|
|	 502 Bad Gateway 	|	 InvalidField.FareKey 	|	 The 'FareKey' is invalid. 	|
|	 502 Bad Gateway 	|	 InvalidField.Installments 	|	 The 'Installments' cannot be zero or null. 	|
|	 502 Bad Gateway 	|	 InvalidField.MethodCode.Length 	|	 The 'MethodCode' must be 2 characters. 	|
|	 502 Bad Gateway 	|	 InvalidField.Miscelaneous.Length 	|	 Check the length of fields 'GovId, AccountHolderName and VerificationCode'. 	|
|	 502 Bad Gateway 	|	 InvalidField.Organization 	|	 The 'Organization' is invalid! 	|
|	 502 Bad Gateway 	|	 InvalidField.OrganizationCode 	|	 The 'OrganizationCode' is invalid. 	|
|	 502 Bad Gateway 	|	 InvalidField.OrganizationCode.Length 	|	 The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. 	|
|	 502 Bad Gateway 	|	 InvalidField.PassengerType.Length 	|	 The 'Passengers.Type' has a maximum length of 3 characters. 	|
|	 502 Bad Gateway 	|	 InvalidField.Password 	|	 The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. 	|
|	 502 Bad Gateway 	|	 InvalidField.PromotionCode 	|	 The 'PromotionCode' is invalid! 	|
|	 502 Bad Gateway 	|	 InvalidField.PromotionCode.Length 	|	 The 'PromotionCode' has a maximum length of 8 characters. 	|
|	 502 Bad Gateway 	|	 Navitaire.Authenticated.NoAgentRoles 	|	 Unable to find valid role for agent. 	|
|	 502 Bad Gateway 	|	 Navitaire.Authenticated.Session 	|	 An agent is already authenticated. 	|
|	 502 Bad Gateway 	|	 Navitaire.GetBooking.Failed 	|	 The requested order was not found or does not exist. 	|
|	 502 Bad Gateway 	|	 Navitaire.Request.Failed 	|	 The request failed. 	|
|	 502 Bad Gateway 	|	 Navitaire.SeatKey.Invalid 	|	 Invalid seat key for equipment. 	|
|	 502 Bad Gateway 	|	 Navitaire.SegmentKey.Invalid 	|	 The 'SegmentKey' is invalid. 	|
|	 502 Bad Gateway 	|	 Order.RequestFailed 	|	 An error has ocurred retrieving the order from state. 	|
|	 502 Bad Gateway 	|	 Order.RequestFailed.Credits 	|	 An error occurred while searching for credit. 	|
|	 502 Bad Gateway 	|	 Order.RequestFailed.InsufficientFunds 	|	 Not enough funds available. 	|
|	 502 Bad Gateway 	|	 Order.RequestFailed.NoFunds 	|	 The Order in state has no funds. 	|
|	 502 Bad Gateway 	|	 Order.RequestFailed.NotUpdated 	|	 Unable to update booking. 	|
|	 502 Bad Gateway 	|	 Organization.AuthorizationFailed.User 	|	 This user does not have access to the informed organization. 	|
|	 502 Bad Gateway 	|	 Organization.NotActive 	|	 The Organization is not active. 	|
|	 502 Bad Gateway 	|	 Passengers.Count.OverMaximum 	|	 The sum of adult and child passenger must be less than or equal to 9. 	|
|	 502 Bad Gateway 	|	 Passengers.Count.UnderMinimum 	|	 The minimum count of 'Passenger' array is 1. 	|
|	 502 Bad Gateway 	|	 RequestFailed 	|	 The request failed. 	|
|	 502 Bad Gateway 	|	 RequestFailed.AssistanceCode.NotAllowed 	|	 The informed assistance code is invalid or cannot be added to this journey. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Authentication 	|	 An error occurred while authenticating. 	|
|	 502 Bad Gateway 	|	 RequestFailed.ChangeNotAllowed 	|	 The requested journey cannot be changed. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Comarch 	|	 An error occurred while retrieving the data in the comarch. 	|
|	 502 Bad Gateway 	|	 RequestFailed.CompletedPayment 	|	 The amounts for this order have already been totally paid. 	|
|	 502 Bad Gateway 	|	 RequestFailed.ContactError 	|	 Your Order request was succefully processed, but the informed booking contact has errors. 	|
|	 502 Bad Gateway 	|	 RequestFailed.DeletingError 	|	 An error occurred when deleting the order. 	|
|	 502 Bad Gateway 	|	 RequestFailed.GetPayment 	|	 There was an error retrieving the payment. 	|
|	 502 Bad Gateway 	|	 RequestFailed.IncompletePayment 	|	 The Payment must include at least the total amount of the order taxes. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Installments 	|	 Installment payment available only for BRL currency code. 	|
|	 502 Bad Gateway 	|	 RequestFailed.NotAuthenticated 	|	 An error occurred while authenticating. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Order.AlreadyExistsInState 	|	 There is already an order created in state. 	|
|	 502 Bad Gateway 	|	 RequestFailed.OrderPayments 	|	 The order in the current state has not been checked out yet. The CreditType 'Order' only applies to created orders. 	|
|	 502 Bad Gateway 	|	 RequestFailed.OverPayment 	|	 The informed amount is greater than the balance due for this order. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Payments 	|	 An error occurred with the order payments service. 	|
|	 502 Bad Gateway 	|	 RequestFailed.SSR.AddNotPossible 	|	 It was not possible to add an SSR to the order. 	|
|	 502 Bad Gateway 	|	 RequestFailed.UnaccompaniedMinor.Information 	|	 There are unaccompanied minors in your order, please verify possible costs and required documentations. 	|
|	 502 Bad Gateway 	|	 RequestFailed.Unexpected 	|	 An unexpected error has occurred. 	|
|	 502 Bad Gateway 	|	 RequiredField.Amount 	|	 The 'Amount' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.CreditCard.MethodCode 	|	 The 'MethodCode' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.Departure 	|	 The 'Departure' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.FareKey 	|	 The 'FareKey' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.JourneyKey 	|	 The 'JourneyKey' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.OrganizationCode 	|	 The 'OrganizationCode' is required. 	|
|	 502 Bad Gateway 	|	 RequiredField.PassengerType 	|	 The 'Passenger.Type' is required. 	|
|	 502 Bad Gateway 	|	 Resources.RequestFailed 	|	 The Resources request failed. 	|
|	 502 Bad Gateway 	|	 UserOrganization.NotAllowed 	|	 The logged user organization does not have access to the requested order. 	|
