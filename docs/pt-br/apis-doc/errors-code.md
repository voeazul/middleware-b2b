# Códigos de Erro e Mensagens

Nosso barramento tem diversas regras e tratativas para garantir a integridade do fluxo. Abaixo estão mapeados todos códigos de resposta HTTP, possíveis códigos de erro e suas respectivas mensagens de erro:

## Erros Gerais

| Código HTTP       | Código Interno | Mensagem de Erro                               | Descrição                                     |
| ----------------- | -------------- | ---------------------------------------------- | ----------------------------------------------|
| 400 Bad Request | Agent.NoOrganizationGroup | The Agent must be in a organization group when 'OrderCriteria.Type' is equal to 'OrganizationGroup'. | O Agente deve estar em um grupo de uma organização quando 'OrderCriteria.Type' for igual a 'OrganizationGroup'. |
| 400 Bad Request | Agent.NotAuthorized | Agent is not allowed to assign seat. | O agente não tem permissão para atribuir assento. |
| 400 Bad Request | AgentOrder.NotAuthorized | Agent is not authorized to commit order with invalid price status without requesting to override restrictions. | O agente não está autorizado a confirmar a reserva com status de preço inválido sem solicitar a substituição das restrições. |
| 400 Bad Request | Alerts.Authentication.Invalid | Invalid Authentication. | Autenticação inválida. |
| 400 Bad Request | AlreadyExists.Username | The 'Username' entered already exists in this or another organization. | O 'Username' inserido já existe nesta ou em outra organização. |
| 400 Bad Request | AuthorizationFailed.Credentials | Username or password is incorrect. | Nome de usuário ou senha está incorreta. |
| 400 Bad Request | B2b.OrderManagementRequest.Failed | The request failed. | A solicitação falhou. |
| 400 Bad Request | B2b.Request.Failed | The request failed. | A solicitação falhou. |
| 400 Bad Request | B2b.User.Failed | The request failed. | A solicitação falhou. |
| 400 Bad Request | BirthCountry.NotFound | The 'BirthCountry' was not found. | O 'BirthCountry' não foi encontrado. |
| 400 Bad Request | Change.Hold.Information | The hold date has changed from {0} to {1}. | A data de retenção mudou de {0} para {1}. |
| 400 Bad Request | Change.Hold.NotAllowed | Unable to update hold date. Check the given date. | Não foi possível atualizar a data de retenção.  |
| 400 Bad Request | ChangeCancel.NotFound | No ChangeCancel session found. | Nenhuma sessão ChangeCancel encontrada. |
| 400 Bad Request | Checkout.V2.Blocked | This method is not compatible with retrieve order in V1. | Este método não é compatível com a reserva de recuperação em V1. |
| 400 Bad Request | Codeshare.Departure.LessThan24Hours | It is not allowed to create an order with codeshare when the journey departure date is less than 24 hours. | Não é permitido criar uma reserva com codeshare quando a data de saída da viagem for inferior a 24 horas. |
| 400 Bad Request | Contact.AddressLine.Required | The 'AddressLine1' is required. | O 'AddressLine1' é obrigatório. |
| 400 Bad Request | Contact.Duplicate | The 'TypeCode' is duplicated. | O 'TypeCode' está duplicado. |
| 400 Bad Request | Contact.LastName.Required | The 'LastNameRequired' is required. | O 'LastNameRequired' é obrigatório. |
| 400 Bad Request | CustomerProgram.NotAllowed | This user profile cannot categorize customers. | Este perfil de usuário não pode categorizar clientes. |
| 400 Bad Request | CustomProgram.NotMatch | Passenger name does not match within informed Customer Program. | O nome do passageiro não corresponde ao Programa do Cliente informado. |
| 400 Bad Request | Dates.Range.OverMaximum | The difference in days between 'DepartureBegin' and 'DepartureEnd' cannot be greater than {0} days. | A diferença de dias entre 'DepartureBegin' e 'DepartureEnd' não pode ser superior a {0} dias. |
| 400 Bad Request | DiscountPayment.TudoAzul | A discount have been applied to your order for using a TudoAzul card. | Foi aplicado um desconto na sua reserva pela utilização do cartão TudoAzul. |
| 400 Bad Request | Email.NotFound | User has no email assigned. | O usuário não tem email atribuído. |
| 400 Bad Request | FlexibleDays.Disabled | Unable to get flexible days because this feature is disabled. | Não é possível obter dias flexíveis porque esse recurso está desativado. |
| 400 Bad Request | Infant.NotNull | There is already a infant in the order for this passenger. | Já existe um bebê na reserva para este passageiro. |
| 400 Bad Request | Infant.Request.Failed | There was an error sending the passenger document. | Ocorreu um erro no envio do documento do passageiro. |
| 400 Bad Request | Integration.EnterpriseStation | An error occurred while returning the stations. | Ocorreu um erro ao retornar as estações. |
| 400 Bad Request | Integration.Error | ServiceBus connection error! | Erro de conexão do ServiceBus! |
| 400 Bad Request | InvalidField.Account | The 'Account' is invalid. | A 'Account' é inválida. |
| 400 Bad Request | InvalidField.Account.Length | The 'Account' has a maximum length of 16 characters. | A 'Account' tem um comprimento máximo de 16 caracteres. |
| 400 Bad Request | InvalidField.Address.City | The 'Address.City' has a maximum of 32 characters. | O 'Address.City' possui no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.Address.Country | The 'Address.CountryCode' has a maximum of 2 characters. | O 'Address.CountryCode' possui no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.Address.LineOne | The 'Address.LineOne' has a maximum of 128 characters. | O 'Address.LineOne' possui no máximo 128 caracteres. |
| 400 Bad Request | InvalidField.Address.LineThree | The 'Address.LineThree' has a maximum of 128 characters. | O 'Address.LineThree' possui no máximo 128 caracteres. |
| 400 Bad Request | InvalidField.Address.LineTwo | The 'Address.LineTwo' has a maximum of 128 characters. | O 'Address.LineTwo' possui no máximo 128 caracteres. |
| 400 Bad Request | InvalidField.Address.PostalCode | The 'Address.PostalCode' has a maximum of 10 characters. | O 'Address.PostalCode' tem no máximo 10 caracteres. |
| 400 Bad Request | InvalidField.Address.ProvinceState | The 'Address.ProvinceState' has a maximum of 3 characters. | O 'Address.ProvinceState' possui no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.Amount | The 'Amount' value must be equal or greater than zero. | O valor 'Amount' deve ser igual ou maior que zero. |
| 400 Bad Request | InvalidField.AssistanceArray | The minimum count of 'Assistances' array is 1. | A contagem mínima da lista 'Assistances' é 1. |
| 400 Bad Request | InvalidField.AssistanceCode | The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. | A assistência '{0}' é inválida para a Jornada '{1}-{2} - {3}'. |
| 400 Bad Request | InvalidField.AssistancesCount | The 'Assistances.Count' must be greather than 0. | O 'Assistances.Count' deve ser maior que 0. |
| 400 Bad Request | InvalidField.Authorization | The 'PaymentCriteria.Authorization' has a maximum of 20 characters. | O 'PaymentCriteria.Authorization' possui no máximo 20 caracteres. |
| 400 Bad Request | InvalidField.BaggageAllowance | The 'BaggageAllowance' must be a valid Enum. | O 'BaggageAllowance' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Bin | The 'BIN' is not a valid number. | O 'BIN' não é um número válido. |
| 400 Bad Request | InvalidField.Bin.Length | The 'BIN' must be of 6 characters. | O 'BIN' deve ter 6 caracteres. |
| 400 Bad Request | InvalidField.CardEnd | The 'PaymentCriteria.CardEnd' has a maximum of 4 characters. | O 'PaymentCriteria.CardEnd' possui no máximo 4 caracteres. |
| 400 Bad Request | InvalidField.ChangeType | The 'ChangeType' must be a valid Enum. | O 'ChangeType' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Code | The 'Code' must have a maximum length of 10 characters. | O 'Code' deve ter no máximo 10 caracteres. |
| 400 Bad Request | InvalidField.Codes | The minimum count of 'Codes' array is 1. | A contagem mínima da lista 'Codes' é 1. |
| 400 Bad Request | InvalidField.Contact.AddressCity | The 'Contact.Address.City' has a maximum length 32 characters. | O 'Contact.Address.City' tem no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.Contact.CompanyName | The 'Contact.CompanyName' has a maximum of 64 characters. | O 'Contact.CompanyName' possui no máximo 64 caracteres. |
| 400 Bad Request | InvalidField.Contact.Email | The 'Contact.Email' is invalid. | O 'Contact.Email' é inválido. |
| 400 Bad Request | InvalidField.Contact.FirstName | The 'Name.First' has a maximum of 32 characters. | O 'Name.First' possui no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.Contact.LastName | The 'Name.Last' has a maximum of 32 characters. | O 'Name.Last' possui no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.ContactAddress.LineOne | The 'Contact.Address.LineOne' has a maximum length 52 characters. | O 'Contact.Address.LineOne' tem comprimento máximo de 52 caracteres. |
| 400 Bad Request | InvalidField.ContactAddress.LineThree | The 'Contact.Address.LineThree' has a maximum length 52 characters. | O 'Contact.Address.LineThree' tem comprimento máximo de 52 caracteres. |
| 400 Bad Request | InvalidField.ContactAddress.LineTwo | The 'Contact.Address.LineTwo' has a maximum length 52 characters. | O 'Contact.Address.LineTwo' tem comprimento máximo de 52 caracteres. |
| 400 Bad Request | InvalidField.ContactAddress.PostalCode | The 'Contact.Address.PostalCode' has a maximum length 10 characters. | O 'Contact.Address.PostalCode' tem no máximo 10 caracteres. |
| 400 Bad Request | InvalidField.ContactAddress.ProviceState | The 'Contact.Address.ProvinceState' has a maximum length 3 characters. | O 'Contact.Address.ProvinceState' tem no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.ContactAddressLineCountry | The 'Contact.Address.Country' has a maximum length 2 characters. | O 'Contact.Address.Country' tem no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.ContactName.First | The 'Contact.Name.First' has a maximum length 32 characters. | O 'Contact.Name.First' tem no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.ContactName.Last | The 'Contact.Name.Last' has a maximum length 32 characters. | O 'Contact.Name.Last' tem no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.ContactName.Middle | The 'Contact.Name.Middle' has a maximum length 32 characters. | O 'Contact.Name.Middle' tem no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.ContactName.Suffix | The 'Contact.Name.Suffix' must be a valid enum. | O 'Contact.Name.Suffix' deve ser um enum válido. |
| 400 Bad Request | InvalidField.ContactNameT.itle | The 'Contact.Name.Title' must be a valid enum. | O 'Contact.Name.Title' deve ser um enum válido. |
| 400 Bad Request | InvalidField.ContactPhones.Number | The 'Contact.Phones.Number' has a maximum length 20 characters. | O 'Contact.Phones.Number' tem no máximo 20 caracteres. |
| 400 Bad Request | InvalidField.ContactPhones.Type | The 'Contact.Phones.Type' must be a valid enum. | O 'Contact.Phones.Type' deve ser um enum válido. |
| 400 Bad Request | InvalidField.Count.Infant | The 'ADT' type passenger count must be greater than 'INF' type passenger count. | A contagem de passageiros do tipo 'ADT' deve ser maior que a contagem de passageiros do tipo 'INF'. |
| 400 Bad Request | InvalidField.Count.OverMaximum | The sum of 'Passengers.Count' of type ADT and CHD must be less than or equal to {0} passengers. | A soma de 'Passengers.Count' do tipo ADT e CHD deve ser menor ou igual a {0} passageiros. |
| 400 Bad Request | InvalidField.Count.UnderMinimum | The minimum value of 'Passengers.Count' is 1. | O valor mínimo de 'Passengers.Count' é 1. |
| 400 Bad Request | InvalidField.CountryCode | The 'CountryCode' must have 2 characters. | O 'CountryCode' deve ter 2 caracteres. |
| 400 Bad Request | InvalidField.CreatedBy | The 'OrderCriteria.CreatedBy' has a maximum of 20 characters. | O 'OrderCriteria.CreatedBy' possui no máximo 20 caracteres. |
| 400 Bad Request | InvalidField.CreditAmount.Empty | The 'CreditAmount' value must be greater than zero. | O valor 'CreditAmount' deve ser maior que zero. |
| 400 Bad Request | InvalidField.CriteriaType | The 'CriteriaType' must be an valid Enum. | O 'CriteriaType' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.customerProgram.number | Alphabetic characters are not allowed. | Caracteres alfabéticos não são permitidos. |
| 400 Bad Request | InvalidField.CustomerProgram.Number | The 'Passengers.CustomerProgram.Number' has a maximum lenght of 20 characters. | O 'Passengers.CustomerProgram.Number' tem no máximo 20 caracteres. |
| 400 Bad Request | InvalidField.DateOfBirth | The agent must be at least {0} years old. | O agente deve ter pelo menos {0} anos. |
| 400 Bad Request | InvalidField.Day | the 'PeriodCriteria.Day' can only be informed if the 'PeriodCriteria.Type' is equal to 'Day'. | o 'PeriodCriteria.Day' só poderá ser informado se o 'PeriodCriteria.Type' for igual a 'Day'. |
| 400 Bad Request | InvalidField.Departure | The 'Departure' must be greater than or equal today's date. | A 'Departure' deve ser maior ou igual à data de hoje. |
| 400 Bad Request | InvalidField.DepartureBegin | The 'DepartureBegin' must be greater than today's date. | O 'DepartureBegin' deve ser maior que a data de hoje. |
| 400 Bad Request | InvalidField.DepartureEnd | The 'DepartureBegin' must be greater than 'DepartureEnd'. | O 'DepartureBegin' deve ser maior que 'DepartureEnd'. |
| 400 Bad Request | InvalidField.Destination.Length | The 'Destination' station code has a maximum length of 3 characters. | O código da estação 'Destination' tem um comprimento máximo de 3 caracteres. |
| 400 Bad Request | InvalidField.Email | The 'Email' provided is invalid. | O 'E-mail' fornecido é inválido. |
| 400 Bad Request | InvalidField.EquipmentCode | The 'EquipmentCode' must have a maximum of 3 characters. | O 'EquipmentCode' deve ter no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.ExpirationDate | Invalid credit card expiration date. | Data de validade do cartão de crédito inválida. |
| 400 Bad Request | InvalidField.ExpirationMonth | The 'ExpirationMonth' must be empty when MethodCode is {0} | O 'ExpirationMonth' deve estar vazio quando MethodCode for {0} |
| 400 Bad Request | InvalidField.ExpirationYear | The 'ExpirationYear' must be empty when MethodCode is {0} | O 'ExpirationYear' deve estar vazio quando MethodCode for {0} |
| 400 Bad Request | InvalidField.FareKey | The 'FareAvailabilityKey' is invalid! | O 'FareAvailabilityKey' é inválido! |
| 400 Bad Request | InvalidField.FeeCode | The 'FeeCode' must have a maximum of 6 characters. | O 'FeeCode' deve ter no máximo 6 caracteres. |
| 400 Bad Request | InvalidField.Filter | Can only be filtered by 'Username' or 'FirstName'. | Só pode ser filtrado por 'Username' ou 'Nome'. |
| 400 Bad Request | InvalidField.FirstName | The 'FirstName' must be a string with a maximum length of 32. | O 'Nome' deve ser uma string com comprimento máximo de 32. |
| 400 Bad Request | InvalidField.FirstName.Length | The 'FirstName' must be a string with a maximum length of 128. | O 'Nome' deve ser uma string com comprimento máximo de 128. |
| 400 Bad Request | InvalidField.FirstNameMatching | The 'FirstNameMatching' cannot be entered with 'Username'. | O 'FirstNameMatching' não pode ser inserido com 'Username'. |
| 400 Bad Request | InvalidField.FlexibleDays.Ahead | The minimum value of 'FlexibleDays.Ahead' is {0}. | O valor mínimo de 'FlexibleDays.Ahead' é {0}. |
| 400 Bad Request | InvalidField.FlexibleDays.Behind | The minimum value of 'FlexibleDays.Behind' is {0}. | O valor mínimo de 'FlexibleDays.Behind' é {0}. |
| 400 Bad Request | InvalidField.FlightNumber | Some segments for the Journey '{0}-{1} - {2}' do not support the assistance '{3}'. Please contact the customer service to complete the special assistance process. | Alguns segmentos da Jornada '{0}-{1} - {2}' não suportam a assistência '{3}'.  |
| 400 Bad Request | InvalidField.Gender | The 'TravelDocuments.Gender' must be a valid Enum. | O 'TravelDocuments.Gender' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.GovId | The 'GovId' is invalid. | O 'GovId' é inválido. |
| 400 Bad Request | InvalidField.GovId.Length | The 'GovId' has a maximum length of 11 characters. | O 'GovId' tem no máximo 11 caracteres. |
| 400 Bad Request | InvalidField.HolderName | The 'HolderName' must be empty when MethodCode is {0} | O 'HolderName' deve estar vazio quando MethodCode for {0} |
| 400 Bad Request | InvalidField.HolderName.Length | The 'HolderName' has a maximum length of 255 characters. | O 'HolderName' tem um comprimento máximo de 255 caracteres. |
| 400 Bad Request | InvalidField.Identifier | The Identifier cannot be more than 20 digits. | O Identificador não pode ter mais de 20 dígitos. |
| 400 Bad Request | InvalidField.Infant.DateOfBirth | The 'Infant.DateOfBirth' is invalid. | O 'Infant.DateOfBirth' é inválido. |
| 400 Bad Request | InvalidField.Infant.Nationality | The 'Infant.Nationality' has a maximum of 2 characters. | A 'Infant.Nationality' tem no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.Installments | The 'Installments' cannot be zero or null. | As 'Installments' não podem ser zero ou nulas. |
| 400 Bad Request | InvalidField.IropContact.Email | The 'Passengers.IropContact.Email' has a maximum length 128 characters. | O 'Passengers.IropContact.Email' tem um comprimento máximo de 128 caracteres. |
| 400 Bad Request | InvalidField.IropContact.Mobile | The 'Passengers.IropContact.Mobile' cannot be informed when Passengers.IropContact.Refused is True. | O 'Passengers.IropContact.Mobile' não pode ser informado quando Passengers.IropContact.Refused for verdadeiro. |
| 400 Bad Request | InvalidField.Jorneys.Departure | Departure of each JourneyKey must be greater than or equal to the current date. | A partida de cada JourneyKey deverá ser maior ou igual à data atual. |
| 400 Bad Request | InvalidField.Journey | The Journey.Key '{0}' is duplicated. | O Journey.Key '{0}' está duplicado. |
| 400 Bad Request | InvalidField.Journey.Key | One or more journeyKeys informed in the request does not exist for the order informed. | Uma ou mais travelKeys informadas na solicitação não existem para a reserva informada. |
| 400 Bad Request | InvalidField.Journeys | The minimum count of 'Journeys' array is 1. | A contagem mínima da lista 'Journeys' é 1. |
| 400 Bad Request | InvalidField.Journeys.Count | The maximum number of Journeys allowed in a order is {0}. | O número máximo de jornadas permitidas em uma reserva é {0}. |
| 400 Bad Request | InvalidField.Journeys.OverMaximum | The number of 'Journeys' must be less than {0}. | O número de 'Journeys' deve ser menor que {0}. |
| 400 Bad Request | InvalidField.Journeys.UnderMinimum | The number of 'Journeys' must be greater than {0}. | O número de 'Journeys' deve ser maior que {0}. |
| 400 Bad Request | InvalidField.Keys | The key '{0}' cannot be accepted. | A chave '{0}' não pode ser aceita. |
| 400 Bad Request | InvalidField.Keys.UnderMinimum | The number of 'Keys' must be greater than 1. | O número de 'Keys' deve ser maior que 1. |
| 400 Bad Request | InvalidField.LastName | The 'LastName' cannot be entered with 'Username'. | O 'LastName' não pode ser inserido com 'Username'. |
| 400 Bad Request | InvalidField.LastName.Length | The 'OrganizationCode' must be a string with a maximum length of 64. | O 'OrganizationCode' deve ser uma string com comprimento máximo de 64. |
| 400 Bad Request | InvalidField.LiableRecordLocator | The 'LiableRecordLocator' must have 6 characters. | O 'LiableRecordLocator' deve ter 6 caracteres. |
| 400 Bad Request | InvalidField.Method | The 'PaymentCriteria.Method' must be a valid Enum. | O 'PaymentCriteria.Method' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.MethodCode | The 'MethodCode' must be equals to {0}, {1}. | O 'MethodCode' deve ser igual a {0}, {1}. |
| 400 Bad Request | InvalidField.MethodCode.Length | The 'MethodCode' must be 2 characters. | O 'MethodCode' deve ter 2 caracteres. |
| 400 Bad Request | InvalidField.MiddleName | The 'MiddleName' must be a string with a maximum length of 32. | O 'MiddleName' deve ser uma string com comprimento máximo de 32. |
| 400 Bad Request | InvalidField.MiddleName.Length | The 'Name.Middle' has a maximum of 32 characters. | O 'Name.Middle' possui no máximo 32 caracteres. |
| 400 Bad Request | InvalidField.Month | The 'PeriodCriteria.Month' must be between 1 and 12. | O 'PeriodCriteria.Month' deve estar entre 1 e 12. |
| 400 Bad Request | InvalidField.Name.First | The 'Name.First' has a maximum length 32 characters. | O 'Name.First' tem comprimento máximo de 32 caracteres. |
| 400 Bad Request | InvalidField.Name.Last | The 'Name.Last' has a maximum length 32 characters. | O 'Name.Last' tem comprimento máximo de 32 caracteres. |
| 400 Bad Request | InvalidField.Name.Length | The 'Username' must be a string with a maximum length of 64. | O 'Username' deve ser uma string com comprimento máximo de 64. |
| 400 Bad Request | InvalidField.Name.Suffix | The 'Name.Sufix' must be a valid Enum. | O 'Name.Sufix' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Name.Title | The 'Name.Title' must be a valid Enum. | O 'Name.Title' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Nationality.Length | The 'Nationality' has a maximum length 2 characters. | A 'Nationality' tem um comprimento máximo de 2 caracteres. |
| 400 Bad Request | InvalidField.NewPassword | The 'NewPassword' must be different from the 'CurrentPassword'. | A 'NewPassword' deve ser diferente da 'CurrentPassword'. |
| 400 Bad Request | InvalidField.NoFilter | Filter by 'Username' or 'FirstName'. | Filtre por 'Username' ou 'FirstName'. |
| 400 Bad Request | InvalidField.Offers | The minimum count of 'Offers' array is 1. | A contagem mínima da lista 'Offers' é 1. |
| 400 Bad Request | InvalidField.Offers.CurrentJourneyKey | One or more CurrentJourneyKey informed in the request does not exist for the order informed. | Uma ou mais CurrentJourneyKey informadas na requisição não existem para a reserva informada. |
| 400 Bad Request | InvalidField.Offers.OverMaximum | The maximum count of 'offer' array is 4 | A contagem máxima da lista 'offer' é 4 |
| 400 Bad Request | InvalidField.Offers.UnderMinimum | The minimum count of 'offer' array is 1. | A contagem mínima da lista 'offer' é 1. |
| 400 Bad Request | InvalidField.OrderCriteria.Status | The 'OrderCriteria.Status' must be a valid Enum. | O 'OrderCriteria.Status' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.OrderCriteria.Type | The 'OrderCriteria.Type' must be a valid Enum. | O 'OrderCriteria.Type' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.OrganizationCode | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. | O 'OrganizationCode' deve ser uma string com comprimento mínimo de 2 e máximo de 10. |
| 400 Bad Request | InvalidField.OrganizationCode.Length | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. | O 'OrganizationCode' deve ser uma string com comprimento mínimo de 2 e máximo de 10. |
| 400 Bad Request | InvalidField.OrganizationCriteria.Type | The 'OrganizationCriteria.Type' must be a valid Enum. | O 'OrganizationCriteria.Type' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.OrganizationFeeOverride.Amount | The 'Amount' value must be equal or greater than zero. | O valor 'Amount' deve ser igual ou maior que zero. |
| 400 Bad Request | InvalidField.OrganizationGroupCode | The 'organizationGroupCode' must be 3 characters in length. | O 'organizationGroupCode' deve ter 3 caracteres. |
| 400 Bad Request | InvalidField.Origin.Length | The 'Origin' station code has a maximum length of 3 characters. | O código da estação 'Origin' tem um comprimento máximo de 3 caracteres. |
| 400 Bad Request | InvalidField.Page | The 'Page' must be greather than or equal to 1. | A 'Page' deve ser maior ou igual a 1. |
| 400 Bad Request | InvalidField.PageNumber | The 'Page' number must be between {0} and {1}. | O número da 'Page' deve estar entre {0} e {1}. |
| 400 Bad Request | InvalidField.PageSize | The 'PageSize' number must be between {0} and {1}. | O número 'PageSize' deve estar entre {0} e {1}. |
| 400 Bad Request | InvalidField.Passenger | The minimum count of 'passengers' array is 1. | A contagem mínima da lista 'passengers' é 1. |
| 400 Bad Request | InvalidField.Passenger.Email | The 'Passenger.Email' is invalid. | O 'Passenger.Email' é inválido. |
| 400 Bad Request | InvalidField.Passenger.IssuingCountry | The 'InvalidField.Passenger.IssuingCountry' has a maximum of 2 characters. | O 'InvalidField.Passenger.IssuingCountry' possui no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.Passenger.Name | The 'Passengers.Name' is required. | O 'Passengers.Name' é obrigatório. |
| 400 Bad Request | InvalidField.Passenger.Nationality | The 'Passenger.Nationality' has a maximum of 2 characters. | O 'Passenger.Nationality' tem no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.Passenger.OverMaximum | The maximum count of 'Passenger' array is 3. | A contagem máxima da lista 'Passenger' é 3. |
| 400 Bad Request | InvalidField.Passenger.Phone | The 'PassengerAddress.Phone' has a maximum of 20 characters. | O 'PassengerAddress.Phone' possui no máximo 20 caracteres. |
| 400 Bad Request | InvalidField.Passenger.Type | The 'PassengerRequest.PassengerTypeCode' has a maximum of 3 characters. | O 'PassengerRequest.PassengerTypeCode' possui no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.Passenger.UnderMinimum | The minimum count of 'Passenger' array is 1. | A contagem mínima da lista 'Passenger' é 1. |
| 400 Bad Request | InvalidField.PassengerAddress.CultureCode | The 'PassengerAddress.CultureCode' has a maximum of 17 characters. | O 'PassengerAddress.CultureCode' possui no máximo 17 caracteres. |
| 400 Bad Request | InvalidField.PassengerAddress.StationCode | The 'PassengerAddress.StationCode' has a minimum of 3 and a maximum of 3 characters. | O 'PassengerAddress.StationCode' possui no mínimo 3 e no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.PassengerCount.UnderMinimum | The 'Passengers.Count' must be greater than 0. | O 'Passengers.Count' deve ser maior que 0. |
| 400 Bad Request | InvalidField.PassengerKeys.Empty | The 'PassengerKeys' array cannot contain empty values. | A lista 'PassengerKeys' não pode conter valores vazios. |
| 400 Bad Request | InvalidField.PassengerType | The 'Passengers.Type' must be equal to 'ADT', 'CHD' or 'INF'. | O 'Passengers.Type' deve ser igual a 'ADT', 'CHD' ou 'INF'. |
| 400 Bad Request | InvalidField.PassengerType.Length | The 'Passengers.Type' has a maximum length of 3 characters. | O 'Passengers.Type' tem no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.PassengerType.Repeated | Must only have one 'Passenger.Type' of type ADT. | Deve ter apenas um 'Passenger.Type' do tipo ADT. |
| 400 Bad Request | InvalidField.Password | The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. | A senha fornecida viola a política de senha.  |
| 400 Bad Request | InvalidField.Period | The 'PeriodCriteria.Period' must be a valid Enum. | O 'PeriodCriteria.Period' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.PeriodCriteria.Type | The 'PeriodCriteria.Type' must be a valid Enum. | O 'PeriodCriteria.Type' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Phone | The 'Phone' provided is invalid. | O 'Telefone' fornecido é inválido. |
| 400 Bad Request | InvalidField.ProductClass | The 'ProductClass' must have a maximum of 2 character. | O 'ProductClass' deve ter no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.ProgramNumber | The 'ProgramNumber' has a maximum lenght of 20 characters. | O 'ProgramNumber' tem um comprimento máximo de 20 caracteres. |
| 400 Bad Request | InvalidField.Promotion.Code | The 'PromotionCode' is invalid. | O 'PromotionCode' é inválido. |
| 400 Bad Request | InvalidField.PromotionCode | The 'PromotionCode' is invalid! | O 'PromotionCode' é inválido! |
| 400 Bad Request | InvalidField.PromotionCode.Length | The 'PromotionCode' has a maximum length of 8 characters. | O 'PromotionCode' tem no máximo 8 caracteres. |
| 400 Bad Request | InvalidField.ProviderType | The 'ProviderType' must be a valid Enum. | O 'ProviderType' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.RecordLocator | The 'RecordLocator' must have 6 characters. | O 'RecordLocator' deve ter 6 caracteres. |
| 400 Bad Request | InvalidField.RefundType | The 'RefundType' must be a valid Enum. | O 'RefundType' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.ReportId | The informed 'ReportId' is invalid. | O 'ReportId' informado é inválido. |
| 400 Bad Request | InvalidField.Role.User | The 'Role' for user informed is invalid. | O 'Role' do usuário informado é inválido. |
| 400 Bad Request | InvalidField.ServicesCount | The 'Services.Count' must be greather than 0. | O 'Services.Count' deve ser maior que 0. |
| 400 Bad Request | InvalidField.StationCode | The 'StationCode' must be 3 characters. | O 'StationCode' deve ter 3 caracteres. |
| 400 Bad Request | InvalidField.Suffix | The 'Suffix' must be a valid Enum. | O 'Sufixo' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.TaxAmount | The 'TaxAmount' must be greater than or equal to 0. | O 'TaxAmount' deve ser maior ou igual a 0. |
| 400 Bad Request | InvalidField.Title | The 'Title' must be a valid Enum. | O 'Title' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Transaction | The 'PaymentCriteria.Transaction' must be a valid Enum. | O 'PaymentCriteria.Transaction' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.TravelDocument.BirthCountry | The 'TravelDocuments.BirthCountry' has a maximum length 2 characters. | O 'TravelDocuments.BirthCountry' tem no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.TravelDocument.IssuingCountry | The 'TravelDocuments.IssuingCountry' has a maximum length 2 characters. | O 'TravelDocuments.IssuingCountry' tem no máximo 2 caracteres. |
| 400 Bad Request | InvalidField.TravelDocument.Number | The 'TravelDocuments.Number' has a maximum length 35 characters. | O 'TravelDocuments.Number' tem no máximo 35 caracteres. |
| 400 Bad Request | InvalidField.TravelDocument.Type | The 'TravelDocuments.Type' must be a valid Enum. | O 'TravelDocuments.Type' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.TravelDocuments.IssuingCountry | The 'TravelDocuments.IssuingCountry' has a maximum length 3 characters. | O 'TravelDocuments.IssuingCountry' tem no máximo 3 caracteres. |
| 400 Bad Request | InvalidField.TravelDocuments.Type | The 'TravelDocuments.Type' has a maximum of 4 characters. | O 'TravelDocuments.Type' possui no máximo 4 caracteres. |
| 400 Bad Request | InvalidField.Type | The 'Type' must be an valid Enum. | O 'Tipo' deve ser um Enum válido. |
| 400 Bad Request | InvalidField.Username | The 'Username' is invalid. Must be a valid CPF. | O 'Username' é inválido.  |
| 400 Bad Request | InvalidField.Username.Length | The 'Username' must be a string with a maximum length of 128. | O 'Username' deve ser uma string com comprimento máximo de 128. |
| 400 Bad Request | InvalidField.UsernameMatching | The 'UsernameMatching' cannot be entered with 'FirstName'. | O 'UsernameMatching' não pode ser inserido com 'FirstName'. |
| 400 Bad Request | InvalidField.VerificationCode | The 'VerificationCode' is invalid. | O 'VerificationCode' é inválido. |
| 400 Bad Request | InvalidField.VerificationCode.Length | The 'VerificationCode' has a maximum length of 4 characters. | O 'VerificationCode' tem comprimento máximo de 4 caracteres. |
| 400 Bad Request | InvalidField.Week | the 'PeriodCriteria.Week' can only be informed if the 'PeriodCriteria.Type' is equal to 'Week'. | o 'PeriodCriteria.Week' só poderá ser informado se o 'PeriodCriteria.Type' for igual a 'Week'. |
| 400 Bad Request | InvalidField.Year | The 'PeriodCriteria.Year' must be equal to or before than the current year. | O 'PeriodCriteria.Year' deve ser igual ou anterior ao ano atual. |
| 400 Bad Request | IssuingCountry.NotFound | The 'IssuingCountry' was not found. | O 'IssuingCountry' não foi encontrado. |
| 400 Bad Request | Journey.DepartureDate.Passed | It is not possible to remove a journey whose departure date has already passed. | Não é possível cancelar uma viagem cuja data de partida já tenha passado. |
| 400 Bad Request | Journey.Fare.SoldOut | The informed 'fareKey' is sold out. | O 'fareKey' informado está esgotado. |
| 400 Bad Request | Journey.FareKey | The 'FareKey' is invalid or is sold out. | O 'FareKey' é inválido ou está esgotado. |
| 400 Bad Request | JourneyKey.Decoding.Error | An error occurred while decoding a JourneyKey. | Ocorreu um erro ao decodificar um JourneyKey. |
| 400 Bad Request | JourneyKey.NotFound | The 'JourneyKey' not found. | O 'JourneyKey' não encontrado. |
| 400 Bad Request | Journeys.DepartureTimeLimit | Sent JourneyKey is too close to it's deaparture time. | O JourneyKey enviado está muito próximo do horário de partida. |
| 400 Bad Request | Journeys.Duplicated | Leg already existing in the offer. | Perna já existente na oferta. |
| 400 Bad Request | Journeys.Overlap | The times of informed journeys overlaps. | Os tempos das viagens informadas se sobrepõem. |
| 400 Bad Request | LiableRecordLocator.UnaccompaniedMinor.Issuing | The 'LiableRecordLocator' can only be informed for issuing an order with unaccompanied minors. | O ‘LiableRecordLocator’ só poderá ser informado para emissão de reserva com menores desacompanhados. |
| 400 Bad Request | Loyalty.Authentication.Invalid | Invalid Authentication. | Autenticação inválida. |
| 400 Bad Request | Loyalty.Customer.NotFound | The customer not found. | O cliente não foi encontrado. |
| 400 Bad Request | Loyalty.InvalidToken.Expired | Token is invalid or expired. | O token é inválido ou expirou. |
| 400 Bad Request | Loyalty.Request.Failed | The Loyalty request failed. | A solicitação de fidelidade falhou. |
| 400 Bad Request | Loyalty.Tier.NotFound | The customer tier not found. | A camada do cliente não foi encontrada. |
| 400 Bad Request | Market.NotAvailable | The set of stations requested do not have an available market yet. | O conjunto de estações solicitadas ainda não tem mercado disponível. |
| 400 Bad Request | Market.Unavailable | The informed origin/destination market are currently unavailable for low fare estimate search. | O mercado de origem/destino informado não está atualmente disponível para pesquisa de estimativas de tarifas baixas. |
| 400 Bad Request | Nationality.NotFound | The 'Nationality' was not found. | A 'Nationality' não foi encontrada. |
| 400 Bad Request | Navitaire.SeatCreate.Failed | The request failed to assign seat. | A solicitação não conseguiu atribuir assento. |
| 400 Bad Request | NotAvailable.Credit | The informed 'RecordLocator' has no credit available. | O ‘RecordLocator’ informado não possui crédito disponível. |
| 400 Bad Request | NotChange.Password | Attempt to modify password was not successful. Please check if new password is different from the current or if it's different from the last 5 used passwords. | A tentativa de modificar a senha não foi bem-sucedida.  |
| 400 Bad Request | Offer.UnaccompaniedMinor.AdditionalFees | Unaccompanied minor may incur additional fee, according to company policy. | Menores desacompanhados poderão incorrer em taxa adicional, de acordo com a política da empresa. |
| 400 Bad Request | Order.Calculation.NotPending | The order in the state has no calculations to be done. | A reserva no estado não tem cálculos a serem feitos. |
| 400 Bad Request | Order.Calculation.Pending | Order details can only be retrieved after calculation of its changes. If you are changing journeys, please finish desired changes and do a calculate before retrieving. | Os detalhes da reserva só podem ser recuperados após o cálculo de suas alterações.  |
| 400 Bad Request | Order.Journeys.Count | The maximum number of Journeys allowed in a order is {0}. | O número máximo de jornadas permitidas em uma reserva é {0}. |
| 400 Bad Request | Order.NoChildren | The informed order does not have any children record locator associated. | A reserva informado não possui nenhum localizador de registros filhos associado. |
| 400 Bad Request | Order.NoJourneys | The informed order has no journeys to be managed. | A reserva informado não possui jornadas a serem gerenciadas. |
| 400 Bad Request | Order.Passengers.NoDateOfBirth | It is not possible to divide orders without all passengers having their date of birth informed in the order. | Não é possível dividir reservas sem que todos os passageiros tenham sua data de nascimento informada na reserva. |
| 400 Bad Request | Order.PendingCalculation | There are pending calculations to be performed. Call the order calculate method before confirming your order changes. | Existem cálculos pendentes a serem realizados.  |
| 400 Bad Request | Order.Reaccommodation.Pending | It is not possible manage an order with pending reaccommodation. | Não é possível gerir uma encomenda com reacomodação pendente. |
| 400 Bad Request | Order.RefundType.NotAllowed | The 'RefundType' field can only be entered when 'Cancel' is true. | O campo 'RefundType' só pode ser inserido quando 'Cancel' for verdadeiro. |
| 400 Bad Request | Order.Retrieve.V1.Conflict | This method is not compatible with retrieve order in V1. | Este método não é compatível com a ordem de recuperação em V1. |
| 400 Bad Request | Order.Retrieve.V2.Conflict | This method is not compatible with retrieve order in V2. | Este método não é compatível com a ordem de recuperação na V2. |
| 400 Bad Request | Order.State.Timeout | The state time for this order has expired. Please retrieve the order again with the GET Order method. | O tempo estadual para esta reserva expirou.  |
| 400 Bad Request | OrderDivide.BalanceDue.Underpaid | Underpaid orders cannot be divided. | Reservas mal pagos não podem ser divididos. |
| 400 Bad Request | OrderDivide.CreditAmount.invalid | The informed 'creditAmount' is invalid because it's greater than the amount available in the informed order. | O 'creditAmount' informado é inválido porque é maior que o valor disponível na reserva informado. |
| 400 Bad Request | OrderDivide.DivideCredit.Failed | An error occurred while dividing the order credit. Credit values have not been divided or changed, remaining entirely in the parent order. | Ocorreu um erro ao dividir o crédito da reserva.  |
| 400 Bad Request | OrderDivide.PassengerKeys.InvalidAmount | The number of 'passengerKeys' in the request must be less than the number of passengers in the informed order. | A quantidade de ‘passengerKeys’ na solicitação deverá ser menor que a quantidade de passageiros da reserva informado. |
| 400 Bad Request | OrderDivide.Pending.Service | It is not possible to perform order divide after a service addition/change. Please confirm changes to your order before splitting it, or split it first before making changes. | Não é possível realizar a divisão de reservas após uma adição/alteração de serviço.  |
| 400 Bad Request | OrderDivide.Unaccompanied.NotAllowed | It's not allowed to divide an order when it will result in orders where there are only unaccompanied minors (under {0} years old). Both involved orders must contain at least one adult passenger (ADT) over {0} years of age at the end of the division. | Não é permitida a divisão de uma reserva quando isso resultar em reservas onde haja apenas menores desacompanhados (menores de {0} anos).  |
| 400 Bad Request | Organization.AlreadyIntoGroup | The informed OrganizationCode is already inserted in this organization group. | O OrganizationCode informado já está inserido neste grupo organizacional. |
| 400 Bad Request | Organization.AuthorizationFailed | The agent does not have access to the finder organization, either on its own or by a group. | O agente não tem acesso à organização localizadora, nem por conta própria nem por grupo. |
| 400 Bad Request | Organization.CNPJ.Invalid | The point of sale organization does not have a valid CNPJ. | A organização do ponto de venda não possui CNPJ válido. |
| 400 Bad Request | Organization.Conflict | You are not allowed to delete your own point of sale from a group. | Você não tem permissão para excluir seu próprio ponto de venda de um grupo. |
| 400 Bad Request | Organization.Email | Your organization doesn't have a valid email. Please contact Azul's comercial team. | Sua organização não tem um e-mail válido.  |
| 400 Bad Request | Organization.Request.Failed | The Organization request failed. | A solicitação da organização falhou. |
| 400 Bad Request | OrganizationAccount.NotFound | Organization has no account. | A organização não tem conta. |
| 400 Bad Request | OrganizationGroup.Invalid | OrganizationGroup already exists or invalid. | OrganizationGroup já existe ou é inválido. |
| 400 Bad Request | Passenger.AssignedSeat | Seat already assigned to the passenger. | Assento já atribuído ao passageiro. |
| 400 Bad Request | Passenger.DocumentType.Confict | Document already informed to the passenger of the order. | Documento já informado ao passageiro da reserva. |
| 400 Bad Request | Passenger.DocumentTypeMatch.NotAllowed | Multiple Passengers with the same Travel Document Type and Number are not allowed, including Infants. | Não são permitidos vários passageiros com o mesmo tipo e número de documento de viagem, incluindo bebês. |
| 400 Bad Request | Passenger.InvalidAge | Passenger under 12 years old on the departure date cannot be considered an adult (ADT). | Passageiro menor de 12 anos na data do embarque não poderá ser considerado adulto (ADT). |
| 400 Bad Request | Passenger.NameMatch.NotAllowed | Multiple Passengers with exactly the same First Name, Middle Name, Last Name and Suffix are not allowed, including Infants. | Não são permitidos vários passageiros com exatamente o mesmo nome, nome do meio, sobrenome e sufixo, incluindo bebês. |
| 400 Bad Request | Passenger.TraveDocument.Expired | Informed travel document will be expired on the departure date. | O documento de viagem informado expirará na data da partida. |
| 400 Bad Request | Passenger.Unaccompanied.InvalidAge | Minors must be over 8 years old to travel unaccompanied. | Menores devem ter mais de 8 anos para viajar desacompanhados. |
| 400 Bad Request | PassengerFeeKey.NotFound | The 'PassengerFeeKey' not found. | O 'PassengerFeeKey' não foi encontrado. |
| 400 Bad Request | Payments.Credit.Failed | An error occurred while using the credit. | Ocorreu um erro ao usar o crédito. |
| 400 Bad Request | Payments.MinimumRequired | Payments must contemplate all journey fares, travel fees and taxes. | Os pagamentos deverão contemplar todas as tarifas de viagem, taxas de viagem e impostos. |
| 400 Bad Request | Payments.ValidationError | Checkout validation error. Payments amount does not match the total cost of the order. | Erro de validação de checkout.  |
| 400 Bad Request | Profile.HoldPermission | Your current profile does not allow hold creation. | Seu perfil atual não permite a criação de retenção. |
| 400 Bad Request | Quote.UnaccompaniedMinor.NotAllowed | The 'JourneyKeys' {0} does not allow unaccompanied minors. | O 'JourneyKeys' {0} não permite menores desacompanhados. |
| 400 Bad Request | Reaccommodation.InProcess | Reaccommodation is in process. Wait 24 hours for it to be updated. | A reacomodação está em processo.  |
| 400 Bad Request | RecordLocator.NotFound | The given 'RecordLocator' was not found. | O 'RecordLocator' fornecido não foi encontrado. |
| 400 Bad Request | RefundAuthentication.Request.Failed | The request failed. | A solicitação falhou. |
| 400 Bad Request | RefundOrder.Fare.NotAvailable | Fare not available. | Tarifa não disponível. |
| 400 Bad Request | RefundType.CreditShell.CannotBeApplied | It is not possible to make the refund via credit shell. | Não é possível efetuar o reembolso via shell de crédito. |
| 400 Bad Request | RefundType.Payments.CannotBeApplied | There are no amounts to be refunded. | Não há valores a serem reembolsados. |
| 400 Bad Request | Report.AlreadyExists | There is already an existing report for the informed 'OrderCriteria' and 'PeriodCriteria'. | Já existe um relatório para os 'OrderCriteria' e 'PeriodCriteria' informados. |
| 400 Bad Request | Report.InProcess | The report cannot be changed while it is being processed. | O relatório não pode ser alterado enquanto está sendo processado. |
| 400 Bad Request | Report.PendingCreation | The requested report is not available for download yet, as it has not been created. | O relatório solicitado ainda não está disponível para download, pois ainda não foi criado. |
| 400 Bad Request | Report.RetrieveError | An unexpected error occurred while retrieving the report file. | Ocorreu um erro inesperado ao recuperar o arquivo de relatório. |
| 400 Bad Request | Request.Failed | The Refund request failed. | A solicitação de reembolso falhou. |
| 400 Bad Request | RequestFailed.CreditCard.Expired | Expired credit card. | Cartão de crédito expirado. |
| 400 Bad Request | RequestFailed.Enterprise | An error occurred while validating order passengers names. | Ocorreu um erro ao validar os nomes dos passageiros da reserva. |
| 400 Bad Request | RequestFailed.International.Required | The organization fee override is only allowed for orders with international journeys. | O cancelamento da taxa de organização só é permitido para encomendas com viagens internacionais. |
| 400 Bad Request | RequestFailed.Journeys.NotAllowed | The organization fee override is only allowed while adding new journeys to the order and execute the calculate. | A substituição da taxa de organização só é permitida ao adicionar novas viagens a reserva e executar o cálculo. |
| 400 Bad Request | RequestFailed.PassengerMinor.NotAllowedInfants | Passengers under 18 years old are not allowed to have infants. | Passageiros menores de 18 anos não podem ter bebês. |
| 400 Bad Request | RequestFailed.Passengers.WithoutFee | No passengers in this order have organization fees charged. | Nenhum passageiro nesta ordem tem cobrança de taxas de organização. |
| 400 Bad Request | RequestFailed.TudoAzul.Retrieve | An error occurred while retrieving the TudoAzul program. | Ocorreu um erro ao recuperar o programa TudoAzul. |
| 400 Bad Request | RequestFailed.Unexpected | An unexpected error has occurred. | Ocorreu um erro inesperado. |
| 400 Bad Request | Required.RefundType | The 'RefundType' is required. | O 'RefundType' é obrigatório. |
| 400 Bad Request | RequiredField.Account | The 'Account' is required. | A 'Conta' é obrigatória. |
| 400 Bad Request | RequiredField.Amount | The 'Amount' is required. | O 'Valor' é obrigatório. |
| 400 Bad Request | RequiredField.AssistanceArray | The 'Assistances' array is required. | A lista 'Assistências' é obrigatória. |
| 400 Bad Request | RequiredField.AssistancesCount | The 'Assistances.Count' is required. | O 'Assistances.Count' é obrigatório. |
| 400 Bad Request | RequiredField.AssistancesKey | The 'Assistances.Key' is required. | A 'Assistências.Key' é necessária. |
| 400 Bad Request | RequiredField.ChangeType | The 'ChangeType' is required. | O 'ChangeType' é obrigatório. |
| 400 Bad Request | RequiredField.Code | The 'Code' is required. | O 'Código' é obrigatório. |
| 400 Bad Request | RequiredField.Contact.FirstName | The 'Contact.FirstName' is required. | O 'Contact.FirstName' é obrigatório. |
| 400 Bad Request | RequiredField.Contact.LastName | The 'Contact.LastName' is required. | O 'Contact.LastName' é obrigatório. |
| 400 Bad Request | RequiredField.Contact.Phones | The 'Contact.Phones' is required. | O 'Contact.Phones' é obrigatório. |
| 400 Bad Request | RequiredField.ContactAddress.LineOne | The 'Contact.Address.LineOne' is required. | O 'Contact.Address.LineOne' é obrigatório. |
| 400 Bad Request | RequiredField.ContactName | The 'Contact.Name' object is required. | O objeto 'Contact.Name' é obrigatório. |
| 400 Bad Request | RequiredField.ContactName.First | The 'Contact.Name.First' is required. | O 'Contact.Name.First' é obrigatório. |
| 400 Bad Request | RequiredField.ContactName.Last | The 'Contact.Name.Last' is required. | O 'Contact.Name.Last' é obrigatório. |
| 400 Bad Request | RequiredField.ContactPhones.Number | The 'Contact.Phones.Number' is required. | O 'Contact.Phones.Number' é obrigatório. |
| 400 Bad Request | RequiredField.ContactPhones.Type | The 'Contact.Phones.Type' is required. | O 'Contact.Phones.Type' é obrigatório. |
| 400 Bad Request | RequiredField.ContactPhonesHome | The 'Contact.Phones' a home object is required. | O objeto 'Contact.Phones' é necessário. |
| 400 Bad Request | RequiredField.CreditCard.ExpirationMonth | The 'ExpirationMonth' is required. | O 'ExpirationMonth' é obrigatório. |
| 400 Bad Request | RequiredField.CreditCard.ExpirationYear | The 'ExpirationYear' is required. | O 'ExpirationYear' é obrigatório. |
| 400 Bad Request | RequiredField.CreditCard.GovId | The 'GovId' is required for this method code due to the currency code of the order. | O 'GovId' é necessário para este código de método devido ao código da moeda da reserva. |
| 400 Bad Request | RequiredField.CreditCard.HolderName | The 'HolderName' is required. | O 'HolderName' é obrigatório. |
| 400 Bad Request | RequiredField.CreditCard.MethodCode | The 'MethodCode' is required. | O 'MethodCode' é obrigatório. |
| 400 Bad Request | RequiredField.CreditCard.Type | The 'CreditCard.Type' is required | O 'CreditCard.Type' é obrigatório |
| 400 Bad Request | RequiredField.CreditCard.VerificationCode | The 'VerificationCode' is required. | O 'VerificationCode' é obrigatório. |
| 400 Bad Request | RequiredField.Criteria | The 'Criteria' is only required for 'CriteriaType': 'Phone', 'Email', 'DocumentNumber', 'CardNumber' and 'CustomerNumber'. | Os 'Critérios' só são necessários para 'CriteriaType': 'Telefone', 'E-mail', 'DocumentNumber', 'CardNumber' e 'CustomerNumber'. |
| 400 Bad Request | RequiredField.CriteriaType | The 'CriteriaType' is only required for 'Type': 'Organization'. | O 'CriteriaType' só é necessário para 'Tipo': 'Organização'. |
| 400 Bad Request | RequiredField.CurrencyCode | The 'CurrencyCode' is required. | O 'CurrencyCode' é obrigatório. |
| 400 Bad Request | RequiredField.CurrentPassword | User not authenticated. The field 'Username' is required. | Usuário não autenticado.  |
| 400 Bad Request | RequiredField.DateOfBirth | The 'DateOfBirth' is required. | O 'DateOfBirth' é obrigatório. |
| 400 Bad Request | RequiredField.Day | The 'PeriodCriteria.Day' is required. | O 'PeriodCriteria.Day' é obrigatório. |
| 400 Bad Request | RequiredField.Departure | The 'Departure' is required. | A 'Partida' é obrigatória. |
| 400 Bad Request | RequiredField.DepartureBegin | The 'DepartureBegin' is required. | O 'DepartureBegin' é obrigatório. |
| 400 Bad Request | RequiredField.DepartureDate | The 'Departure' is required. | A 'Partida' é obrigatória. |
| 400 Bad Request | RequiredField.DepartureEnd | The 'DepartureEnd' is required. | O 'DepartureEnd' é obrigatório. |
| 400 Bad Request | RequiredField.Destination | The 'Destination' is required. | O 'Destino' é obrigatório. |
| 400 Bad Request | RequiredField.Document.Type | The 'Infant.Document.Type' CPF, RNE or PASSPORT is required. | É necessário apresentar CPF, RNE ou PASSAPORTE 'Tipo.Documento.Infantil'. |
| 400 Bad Request | RequiredField.DocumentType | The 'DocumentType' is required for the informed 'CriteriaType'. | O 'DocumentType' é obrigatório para o 'CriteriaType' informado. |
| 400 Bad Request | RequiredField.Email | The 'Email' is required. | O 'E-mail' é obrigatório. |
| 400 Bad Request | RequiredField.FareKey | The 'FareKey' is required. | O 'FareKey' é obrigatório. |
| 400 Bad Request | RequiredField.FirstName | The 'FirstName' is required for the 'FirstNameMatching' field. | O 'FirstName' é obrigatório para o campo 'FirstNameMatching'. |
| 400 Bad Request | RequiredField.FirstNameMatching | The 'FirstNameMatching' is required for the 'FirstName' field. | O 'FirstNameMatching' é obrigatório para o campo 'FirstName'. |
| 400 Bad Request | RequiredField.Gender | The 'Gender' must be a valid Enum. | O 'Gênero' deve ser um Enum válido. |
| 400 Bad Request | RequiredField.Identifier | The 'Identifier' is required. | O 'Identificador' é obrigatório. |
| 400 Bad Request | RequiredField.Infant.FirstName | The 'Infant.FirstName' is required. | O 'Infant.FirstName' é obrigatório. |
| 400 Bad Request | RequiredField.Infant.Gender | The 'Infant:Gender' is required. | O 'Infantil:Gênero' é obrigatório. |
| 400 Bad Request | RequiredField.Infant.LastName | The 'Infant.LastName' is required. | O 'Infant.LastName' é obrigatório. |
| 400 Bad Request | RequiredField.IropContact | The 'Passengers.IropContact' is required. | O 'Passengers.IropContact' é obrigatório. |
| 400 Bad Request | RequiredField.IropContact.EmailMobile | The 'Passengers.IropContact.Email' or 'Passengers.IropContact.Mobile is required. | O 'Passengers.IropContact.Email' ou 'Passengers.IropContact.Mobile é obrigatório. |
| 400 Bad Request | RequiredField.IropContact.Refused | The 'Passengers.IropContact.Refused' is required. | O 'Passengers.IropContact.Refused' é obrigatório. |
| 400 Bad Request | RequiredField.JourneyKey | The 'JourneyKey' is required. | A 'JourneyKey' é necessária. |
| 400 Bad Request | RequiredField.Journeys | The 'Journeys' array is required. | A lista 'Journeys' é obrigatória. |
| 400 Bad Request | RequiredField.Journeys.Departure | The 'Departure' is required. | A 'Partida' é obrigatória. |
| 400 Bad Request | RequiredField.Journeys.Key | The 'Journey.Key' is required. | A 'Journey.Key' é necessária. |
| 400 Bad Request | RequiredField.Key | The 'Key' is required. | A 'Chave' é necessária. |
| 400 Bad Request | RequiredField.Keys | The 'Keys' array is required. | A lista 'Keys' é obrigatória. |
| 400 Bad Request | RequiredField.LastName | The 'LastName' is required. | O 'Sobrenome' é obrigatório. |
| 400 Bad Request | RequiredField.Month | The 'PeriodCriteria.Month' is required. | O 'PeriodCriteria.Month' é obrigatório. |
| 400 Bad Request | RequiredField.Name | The 'Name' is required. | O 'Nome' é obrigatório. |
| 400 Bad Request | RequiredField.Name.First | The 'Name.First' is required. | O 'Nome.Primeiro' é obrigatório. |
| 400 Bad Request | RequiredField.Name.Last | The 'Name.Last' is required. | O 'Nome.Último' é obrigatório. |
| 400 Bad Request | RequiredField.Name.Middle | The 'Name.Middle' is required. | O 'Nome.Middle' é obrigatório. |
| 400 Bad Request | RequiredField.Nationality | The 'Nationality' is required. | A 'Nacionalidade' é obrigatória. |
| 400 Bad Request | RequiredField.NewPassword | The 'NewPassword' is required. | A 'Nova Senha' é necessária. |
| 400 Bad Request | RequiredField.Offers | The 'Offers' array is required. | A lista 'Ofertas' é obrigatória. |
| 400 Bad Request | RequiredField.Offers.CurrentJourneyKey | The 'CurrentJourneyKey' is required. | O 'CurrentJourneyKey' é obrigatório. |
| 400 Bad Request | RequiredField.Offers.FareKey | The 'Offers.FareKey' is required. | O 'Offers.FareKey' é obrigatório. |
| 400 Bad Request | RequiredField.Offers.JourneyKey | The 'Offers.JouneyKey' is required. | O 'Offers.JouneyKey' é obrigatório. |
| 400 Bad Request | RequiredField.Offers.NewFareKey | The 'NewFareKey' is required. | O 'NewFareKey' é obrigatório. |
| 400 Bad Request | RequiredField.Offers.NewJourneyKey | The 'NewJourneyKey' is required. | A 'NewJourneyKey' é necessária. |
| 400 Bad Request | RequiredField.OrderCriteria | The 'OrderCriteria' is required. | O 'OrderCriteria' é obrigatório. |
| 400 Bad Request | RequiredField.OrderCriteria.Status | The 'OrderCriteria.Status' is required. | O 'OrderCriteria.Status' é obrigatório. |
| 400 Bad Request | RequiredField.OrderCriteria.Type | The 'OrderCriteria.Type' is required. | O 'OrderCriteria.Type' é obrigatório. |
| 400 Bad Request | RequiredField.OrganizationCode | The 'OrganizationCode' is required. | O 'OrganizationCode' é obrigatório. |
| 400 Bad Request | RequiredField.OrganizationCriteria | The 'OrganizationCriteria' is required. | O 'OrganizationCriteria' é obrigatório. |
| 400 Bad Request | RequiredField.OrganizationCriteria.Type | The 'OrganizationCriteria.Type' is required. | O 'OrganizationCriteria.Type' é obrigatório. |
| 400 Bad Request | RequiredField.OrganizationGroupCode | The 'OrganizationGroupCode' is required. | O 'OrganizationGroupCode' é obrigatório. |
| 400 Bad Request | RequiredField.Origin | The 'Origin' is required. | A 'Origem' é obrigatória. |
| 400 Bad Request | RequiredField.Passenger | The 'Passenger' is required. | O 'Passageiro' é obrigatório. |
| 400 Bad Request | RequiredField.Passenger.DateOfBirth | The 'Passenger.DateOfBirth' is required. | O 'Passenger.DateOfBirth' é obrigatório. |
| 400 Bad Request | RequiredField.Passenger.Gender | The 'Passenger.Gender' is required. | O 'Passenger.Gender' é obrigatório. |
| 400 Bad Request | RequiredField.Passenger.Key | The 'PassengerKey' is required. | A 'PassengerKey' é necessária. |
| 400 Bad Request | RequiredField.Passenger.PhoneEmail | The 'Passengers.Phone' or  'Passengers.Email' is required. | O 'Passengers.Phone' ou 'Passengers.Email' é obrigatório. |
| 400 Bad Request | RequiredField.Passenger.Type | The 'Passengers.Type' is required. | O 'Passengers.Type' é obrigatório. |
| 400 Bad Request | RequiredField.PassengerKey | The 'PassengerKey' is required. | A 'PassengerKey' é necessária. |
| 400 Bad Request | RequiredField.PassengerKeys | The 'passengerKeys' informed in the request does not exist in the informed order. | As 'passengerKeys' informadas na solicitação não existem no pedido informado. |
| 400 Bad Request | RequiredField.Passengers | The 'Passengers' array is required. | A lista 'Passageiros' é obrigatória. |
| 400 Bad Request | RequiredField.PassengerType | The 'Passenger.Type' is required. | O 'Passenger.Type' é obrigatório. |
| 400 Bad Request | RequiredField.PassengerType.Adult | The 'Passengers.Type' a ADT value is required. | O valor 'Passengers.Type' é obrigatório. |
| 400 Bad Request | RequiredField.Password | The 'Password' is required. | A 'Senha' é necessária. |
| 400 Bad Request | RequiredField.PaymentCriteria | The 'PaymentCriteria' is required. | O 'PaymentCriteria' é obrigatório. |
| 400 Bad Request | RequiredField.Period | The 'PeriodCriteria.Period' is required. | O 'PeriodCriteria.Period' é obrigatório. |
| 400 Bad Request | RequiredField.PeriodCriteria.Type | The 'PeriodCriteria.Type' is required. | O 'PeriodCriteria.Type' é obrigatório. |
| 400 Bad Request | RequiredField.Phone | The 'Phone' is required. | O 'Telefone' é obrigatório. |
| 400 Bad Request | RequiredField.PhonesNumber | The 'Phones.Number' is required. | O 'Phones.Number' é obrigatório. |
| 400 Bad Request | RequiredField.PhonesType | The 'Phones.Type' is required. | O 'Phones.Type' é obrigatório. |
| 400 Bad Request | RequiredField.Profile | The 'Profile' is required. | O 'Perfil' é obrigatório. |
| 400 Bad Request | RequiredField.ProgramNumber | The 'ProgramNumber' is required. | O 'ProgramNumber' é obrigatório. |
| 400 Bad Request | RequiredField.ProviderType | The 'ProviderType' is required. | O 'ProviderType' é obrigatório. |
| 400 Bad Request | RequiredField.RecordLocator | The 'RecordLocator' is required. | O 'RecordLocator' é necessário. |
| 400 Bad Request | RequiredField.ReportId | The 'ReportId' is required. | O 'ReportId' é obrigatório. |
| 400 Bad Request | RequiredField.SegmentKey | The 'segmentkey' is required. | A 'segmentkey' é necessária. |
| 400 Bad Request | RequiredField.Services | The 'Services' list is required. | A lista 'Serviços' é obrigatória. |
| 400 Bad Request | RequiredField.ServicesCount | The 'Services.Count' is required. | O 'Services.Count' é obrigatório. |
| 400 Bad Request | RequiredField.ServicesKey | The 'Services.Key' is required. | O 'Services.Key' é obrigatório. |
| 400 Bad Request | RequiredField.SessionContext | The 'SessionContext' is required. | O 'SessionContext' é obrigatório. |
| 400 Bad Request | RequiredField.Status | The 'Status' is required. | O 'Status' é obrigatório. |
| 400 Bad Request | RequiredField.TravelDocument | The minimum count of 'TravelDocument' array is 1. | A contagem mínima da lista 'TravelDocument' é 1. |
| 400 Bad Request | RequiredField.TravelDocument.ExpirationDate | The 'TravelDocuments.ExpirationDate' is required. | O 'TravelDocuments.ExpirationDate' é obrigatório. |
| 400 Bad Request | RequiredField.TravelDocument.Number | The 'TravelDocuments.Number' is required. | O 'TravelDocuments.Number' é obrigatório. |
| 400 Bad Request | RequiredField.TravelDocument.Type | The 'TravelDocuments.Type' CPF, RNE or PASSPORT is required. | É necessário o CPF, RNE ou PASSAPORTE 'TravelDocuments.Type'. |
| 400 Bad Request | RequiredField.TravelDocuments.IssuingCountry | The 'TravelDocuments.IssuingCountry' is required. | O 'TravelDocuments.IssuingCountry' é obrigatório. |
| 400 Bad Request | RequiredField.TravelDocuments.Type | The 'TravelDocuments.Type' is required. | O 'TravelDocuments.Type' é obrigatório. |
| 400 Bad Request | RequiredField.Type | The 'Type' is required. | O 'Tipo' é obrigatório. |
| 400 Bad Request | RequiredField.UnitKey | The 'unitkey' is required. | A 'chave de unidade' é necessária. |
| 400 Bad Request | RequiredField.UserKey | The 'UserKey' is required. | A 'UserKey' é necessária. |
| 400 Bad Request | RequiredField.Username | The 'Username' is required. | O 'Nome de usuário' é obrigatório. |
| 400 Bad Request | RequiredField.Week | The 'PeriodCriteria.Week' is required. | O 'PeriodCriteria.Week' é obrigatório. |
| 400 Bad Request | RequiredField.Year | The 'PeriodCriteria.Year' is required. | O 'PeriodCriteria.Year' é obrigatório. |
| 400 Bad Request | Retrieve.NoActions | There are no more journeys waiting for agent actions on this order. | Não há mais jornadas aguardando ações do agente nesta ordem. |
| 400 Bad Request | Roles.NotAllowed | Cannot edit the user that belongs to WebService roles. | Não é possível editar o usuário que pertence às funções WebService. |
| 400 Bad Request | Seat.Unavailable | Seat already assigned to another passenger. | Assento já atribuído a outro passageiro. |
| 400 Bad Request | Service.Quantity.Restricted | This service is restricted to one occurence per passenger and leg. | Este serviço está restrito a uma ocorrência por passageiro e trecho. |
| 400 Bad Request | Shopping.Request.Failed | The Shopping request failed. | A solicitação do Shopping falhou. |
| 400 Bad Request | Stations.NotAllowed | These requested stations are invalid: | Estas estações solicitadas são inválidas: |
| 400 Bad Request | TudoAzul.Categorization.Failed | There was a failure in the categorization of TudoAzul of 'passengers.customerProgram.number': {0}. Try categorize again after the order creation (before assigning seats or adding baggages to ensure all potential benefits). | Houve falha na categorização do TudoAzul de ‘passageiros.customerProgram.number’: {0}.  |
| 400 Bad Request | UnitKey.Invalid | The 'UnitKey' is invalid. | O 'UnitKey' é inválido. |
| 400 Bad Request | User.CannotBeUnlocked | Only API users can be unlocked. | Somente usuários da API podem ser desbloqueados. |
| 400 Bad Request | User.NoGroup | The user must be in an Organization Group when the ‘Type’ is Group. | O usuário deve estar em um grupo organizacional quando o ‘Tipo’ for Grupo. |
| 400 Bad Request | User.NotEditable | Deleted user cannot be edited. | O usuário excluído não pode ser editado. |
| 400 Bad Request | User.Password.Expired | Expired password, user must change password. | Senha expirada, o usuário deve alterar a senha. |
| 400 Bad Request | Warning.OrganizationFeeOverride | Organization fee override is not applicable for this order. | A substituição da taxa de organização não se aplica a este pedido. |
| 401 Unauthorized | InvalidToken.Expired | An error occurred while performing authentication. | Ocorreu um erro ao executar a autenticação. |
| 401 Unauthorized | InvalidToken.NotAuthenticated | The Bearer Token provided is invalid or expired. | O Bearer Token fornecido é inválido ou expirou. |
| 401 Unauthorized | RequestFailed.Authentication | An error occurred while validating the user authentication. | Ocorreu um erro ao validar a autenticação do usuário. |
| 403 Forbidden | Agent.NoAccess | The agent does not have access to the informed user. | O agente não tem acesso ao usuário informado. |
| 403 Forbidden | AssignSeat.UnitKey.Blocked | The request failed to assign the seat, because this seat is blocked by passengers rules (age, SSR or equipment). | A solicitação não conseguiu atribuir o assento, pois este assento está bloqueado pelas regras do passageiro (idade, SSR ou equipamento). |
| 403 Forbidden | Organization.AuthorizationFailed.User | This user does not have access to the informed organization. | Este usuário não tem acesso à organização informada. |
| 404 Not Found | Assistance.NoMatches | This assistance does not exist or was not found. | Esta assistência não existe ou não foi encontrada. |
| 404 Not Found | Assistances.NoMatches | Unable to retrieve the assistances data. | Não foi possível recuperar os dados de assistência. |
| 404 Not Found | AssistancesKey.NoMatches | The informed 'Assistances.Key' does not exists or does not belong to a previously retrieved 'assistance/search'. | A 'Assistances.Key' informada não existe ou não pertence a uma 'assistance/search' recuperada anteriormente. |
| 404 Not Found | Baggage.NoMatches | No 'Baggage' was found for removal. | Nenhuma 'Bagagem' foi encontrada para remoção. |
| 404 Not Found | BagKey.NoMatches | The informed 'Key' does not exists or does not belong to a previously retrieved 'baggage/search'. | A 'Chave' informada não existe ou não pertence a uma 'bagagem/busca' previamente recuperada. |
| 404 Not Found | Code.NoMatches | Informed Organization Code was not found. | O código da organização informada não foi encontrado. |
| 404 Not Found | Countries.NoMatches | Unable to retrieve the countries data. | Não foi possível recuperar os dados dos países. |
| 404 Not Found | Country.NoMatches | This country does not exist or was not found. | Este país não existe ou não foi encontrado. |
| 404 Not Found | CreditNoMatches | There is no credit available for the informed type. | Não há crédito disponível para o tipo informado. |
| 404 Not Found | CustomerNumber.NoMatches | The 'CustomerProgram' not found. | O 'CustomerProgram' não encontrado. |
| 404 Not Found | CustomerProgram.NoMatches | The Customer Program was not found. | O Programa do Cliente não foi encontrado. |
| 404 Not Found | Equipment.NoMatches | This equipament does not exist or was not found. | Este equipamento não existe ou não foi encontrado. |
| 404 Not Found | Fare.NoMatches | This fare does not exist or was not found. | Esta tarifa não existe ou não foi encontrada. |
| 404 Not Found | Fares.NoMatches | Unable to retrieve the fares data. | Não foi possível recuperar os dados das tarifas. |
| 404 Not Found | Fee.NoMatches | This fee does not exist or was not found. | Esta taxa não existe ou não foi encontrada. |
| 404 Not Found | Fees.NoMatches | Unable to retrieve the fees data. | Não foi possível recuperar os dados de taxas. |
| 404 Not Found | InvalidField.JourneyKey | The 'JourneyKey' is invalid. | O 'JourneyKey' é inválido. |
| 404 Not Found | JourneyKey.NoMatches | The 'JourneyKey' is invalid or does not exists in the current state. | O 'JourneyKey' é inválido ou não existe no state. |
| 404 Not Found | NoMatches | The informed user does not exist or was not found. | O usuário informado não existe ou não foi encontrado. |
| 404 Not Found | Order.NoMatches | The requested order was not found or does not exist. | A order solicitada não foi encontrado ou não existe. |
| 404 Not Found | OrderCache.NoMatches | An order must be attached. | Uma order deve ser anexado. |
| 404 Not Found | OrderSearch.NoMatches | No orders found for the informed search filters. | Não foram encontado orders para os filtros de busca informados. |
| 404 Not Found | Organization.NoMatches | The informed organization does not exist or was not found. | A organização informada não existe ou não foi encontrada. |
| 404 Not Found | OrganizationCode.NoMatches | The informed 'OrganizationCode' doesn't exists or doesn't belong to the same organization as your current Point of Sale. | O 'OrganizationCode' informado não existe ou não pertence à mesma organização do seu Ponto de Venda atual. |
| 404 Not Found | OrganizationGroup.NoMatches | The informed organization group does not exist or was not found. | O grupo organizacional informado não existe ou não foi encontrado. |
| 404 Not Found | OrganizationGroupCode.NoMatches | The 'OrganizationGroupCode does not exist or was not found. | O 'OrganizationGroupCode' não existe ou não foi encontrada. |
| 404 Not Found | PassengerKey.NoMatches | The informed 'PassengerKey' does not match within those on the order in state. | A 'PassengerKey' informada não corresponde a reserva no state. |
| 404 Not Found | PassengerName.NoMatches | The Passenger name does not match within informed Customer Program. | O nome do Passageiro não corresponde ao Programa do Cliente informado. |
| 404 Not Found | Payments.NoMatches | No payments were found for the order in state. | Nenhum pagamento foi encontrado para order no state. |
| 404 Not Found | RecordLocator.NoMatches | Your order must be created to use its credits. | Uma order deve ser criada para utilizar seus créditos. |
| 404 Not Found | RefundOrder.NoMatches | Order not found. Retrieve the order. | Order não encontrada.  |
| 404 Not Found | ReportId.NoMatches | The informed 'ReportId' does not exists or was not found. | O 'ReportId' informado não existe ou não foi encontrado. |
| 404 Not Found | Seat.NoMatches | Seat not found. | Assento não encontrado. |
| 404 Not Found | SeatMap.NoMatches | No matching seats. | Não há assentos correspondentes. |
| 404 Not Found | SegmentKey.NoMatches | The 'SegmentKey' is invalid or does not exists in the current state. | O 'SegmentKey' é inválido ou não existe no state. |
| 404 Not Found | Service.NoMatches | Service not found in the specified Journey. | Serviço não encontrado na journey especificada. |
| 404 Not Found | ServiceKey.NoMatches | The informed 'Services.Key' does not exists or does not belong to a previously retrieved 'service/search'. | O 'Services.Key' informado não existe ou não pertence a um 'serviço/busca' recuperado anteriormente. |
| 404 Not Found | SessionContextToken.NoMatches | No sessions found for the given provider. | Nenhuma sessão encontrada para o provedor fornecido. |
| 404 Not Found | Station.NoMatches | This station does not exist or was not found. | A station não existe ou não foi encontrada. |
| 404 Not Found | Stations.NoMatches | Unable to retrieve the stations data. | Não foi possível recuperar os dados das stations. |
| 404 Not Found | TudoAzul.NoMatches | The informed 'passengers.customerProgram.number': {0} does not exists or was not found. | O 'passengers.customerProgram.number' informado: {0} não existe ou não foi encontrado. |
| 404 Not Found | TudoAzulNames.NoMatches | The names of the informed 'passengers.customerProgram.number': {0} do not match those registered in TudoAzul. | Os nomes dos 'passageiros.customerProgram.number' informados: {0} não correspondem aos cadastrados no TudoAzul. |
| 404 Not Found | UnitKey.NoMatches | The 'UnitKey' is invalid or does not exists in the current state. | O 'UnitKey' é inválido ou não existe no state. |
| 404 Not Found | User.NoMatches | The informed user does not exist or was not found. | O usuário informado não existe ou não foi encontrado. |
| 404 Not Found | UserKey.NoMatches | The informed 'UserKey' does not exist or was not found. | O 'UserKey' informado não existe ou não foi encontrado. |
| 404 Not Found | Username.NoMatches | The 'Username' user does not exist or was not found. | O 'Username' não existe ou não foi encontrado. |
| 409 Conflict | AssignSeat.PassengerKey.Conflict | The PassengerKey does not exists in the order state. | O PassengerKey não existe na order do state. |
| 409 Conflict | AssignSeat.Seat.Conflict | Seat Already Assigned. | Assento já atribuído. |
| 409 Conflict | InvalidField.AssistanceCode | The assistance '{0}' is invalid for the Journey '{1}-{2} - {3}'. | A assistência '{0}' é inválida para a journey '{1}-{2} - {3}'. |
| 409 Conflict | InvalidField.AssistanceLimit | The count for the 'Assistances.key' {0} is greater than the specified limit. | A contagem de 'Assistances.key' {0} é maior que o limite especificado. |
| 409 Conflict | InvalidField.Assistanceskey | There are duplicated 'Assistances.key' {0}. | Existem 'Assistances.key' {0} duplicados. |
| 409 Conflict | InvalidField.PassengerKeyCache | The requested service is not available for the informed passenger. | O serviço solicitado não está disponível para o passageiro informado. |
| 409 Conflict | InvalidField.RecordLocator | The 'RecordLocator' must have 6 characters. | O 'RecordLocator' deve ter 6 caracteres. |
| 409 Conflict | InvalidField.ServiceLimit | The count for the 'Services.key' {0} is greater than the specified limit. | A contagem de 'Services.key' {0} é maior que o limite especificado. |
| 409 Conflict | InvalidField.Serviceskey | There are duplicated 'Services.key' {0}. | Existem 'Services.key' {0} duplicados. |
| 409 Conflict | InvalidToken.Expired | An error occurred while performing authentication. | Ocorreu um erro ao executar a autenticação. |
| 409 Conflict | InvalidToken.NotAuthenticated | The Bearer Token provided is invalid or expired. | O Bearer Token fornecido é inválido ou expirou. |
| 409 Conflict | LiableRecordLocator.UnaccopaniedMinor.NotMatchJourneys | Liable order and unaccompanied minors order flights must match. | Voos com menores desacompanhados devem coincidir. |
| 409 Conflict | NotEmpty.State | It's not possible to attach with an order already retrieved in the current state. Please execute an order delete before the order attach. | Não é possível anexar uma order já recuperada no estado atual.  |
| 409 Conflict | Order.HasRecordLocator | This method is for orders under creation process. If you want to checkout a previously created order, please use the equivalent method in the Order.Management.Api. | Este método é para orders em processo de criação.  |
| 409 Conflict | Order.Recordlocator.Empty | This method is for previously created orders. If you want to retrieve an order under creation, please use the equivalent method in the Order.Api. | Este método é para orders criadas anteriormente.  |
| 409 Conflict | Order.State.Change | Removing a journey after adding journeys is not allowed. Please confirm your changes or restart the process retrieving the order again. | Não é permitido remover uma journey após adicionar outra journey.  |
| 409 Conflict | Order.State.Modified | The order in state has been externally modified. Retrieve the order again with the GET Order methods and try again. | A order no state foi modificada externamente.  |
| 409 Conflict | Order.UnaccopaniedMinor.OperatedFligthAzul | Unaccompanied minors are allowed in Azul operated flights only. | Menores desacompanhados são permitidos apenas em voos operados pela Azul. |
| 409 Conflict | Order.UnderCreationException | This method is for orders under creation process. If you want to retrieve a previously created order, please use the equivalent method in the Order.Management.Api. | Este método é para orders em processo de criação.  |
| 409 Conflict | Refund.NotApplicable | There is no amount in the order to be refunded. | Não há valor na order a ser reembolsado. |
| 409 Conflict | RequestFailed.UnaccompaniedMinor.DomesticFligths | Unaccompanied minors are allowed in brazilian domestic flights only. | Menores desacompanhados são permitidos apenas em voos domésticos no Brasil. |
| 409 Conflict | RequestFailed.UnaccopaniedMinor.OnlyDirectFlight | Unaccompanied minors are allowed in direct flights only. | Menores desacompanhados são permitidos apenas em voos diretos. |
| 409 Conflict | RequiredField.LiableRecordLocator | A passenger over 18 years old is required in the liable order. | É necessário um passageiro maior de 18 anos na order |
| 422 Unprocessable Content | Assistance.SearchRequired | Retrieve a 'assistances/search' with journeyKey before execute this method. | Recupere uma 'assistência/pesquisa' com travelKey antes de executar este método. |
| 422 Unprocessable Content | Baggage.SearchRequired | Retrieve a 'baggage/search' with journeyKey before execute this method. | Recupere uma 'bagagem/pesquisa' com travelKey antes de executar este método. |
| 422 Unprocessable Content | NotMatch.Name | The names sent do not match those on the attached order. | Os nomes enviados não correspondem aos da order em anexo. |
| 422 Unprocessable Content | NotMatch.PassengerKey | An informed passenger key does not exists in the attached order or is invalid. | A chave do passageiro informada não existe em anexo na order ou é inválida. |
| 422 Unprocessable Content | Order.RetrieveRequired | The requested order was not found or does not exist. | A order solicitada não foi encontrada ou não existe. |
| 422 Unprocessable Content | Order.State.Timeout | The state time for this order has expired. Please retrieve the order again with the GET Order method. | O tempo estadual para este pedido expirou.  |
| 422 Unprocessable Content | SeatMapCache.SearchRequired | No seatmap found or generated in state. Please retrieve a seatmap before trying to assign a seat. | Nenhum mapa de assentos encontrado ou gerado no state.  |
| 422 Unprocessable Content | Service.SearchRequired | Retrieve a 'services/search' with journeyKey before execute this method. | Recupere um 'serviços/pesquisa' com travelKey antes de executar este método. |
| 422 Unprocessable Content | UnitKey.SearchRequired | The informed UnitKey does not belong to a previously retrieved SeatMap or the previous retrive is expired. | A UnitKey informada não pertence a um SeatMap recuperado anteriormente ou a recuperação anterior expirou. |
| 502 Bad Gateway | Agent.DefaultEmail.NotConfigured | The informed agent does not have a configured default email. | O agente informado não possui email padrão configurado. |
| 502 Bad Gateway | Agent.NotActive | The Agent is not active. | O Agente não está ativo. |
| 502 Bad Gateway | AuthorizationFailed.Credentials | Username or password is incorrect. | Nome de usuário ou senha está incorreta. |
| 502 Bad Gateway | Comarch.RequestFailed | An error occurred while retrieving the data in the commarch. | Ocorreu um erro ao recuperar os dados na commarch. |
| 502 Bad Gateway | Integration.Error | ServiceBus connection error! | Erro de conexão do ServiceBus! |
| 502 Bad Gateway | Integration.Failed | The request failed. | A solicitação falhou. |
| 502 Bad Gateway | Integration.InvalidFare | There is an error within the requested fares | Há um erro nas tarifas solicitadas |
| 502 Bad Gateway | Integration.InvalidField.CurrencyCode | The 'CurrencyCode' is invalid. | O 'CurrencyCode' é inválido. |
| 502 Bad Gateway | InvalidField.Account | The 'Account' is invalid. | A 'Conta' é inválida. |
| 502 Bad Gateway | InvalidField.Amount | The 'Amount' value must be equal or greater than zero. | O valor 'Quantidade' deve ser igual ou maior que zero. |
| 502 Bad Gateway | InvalidField.CountryCode | The 'CountryCode' must have 2 characters. | O 'CountryCode' deve ter 2 caracteres. |
| 502 Bad Gateway | InvalidField.CurrencyCode.Length | The 'CurrencyCode' has a maximum length of 3 characters. | O 'CurrencyCode' tem um comprimento máximo de 3 caracteres. |
| 502 Bad Gateway | InvalidField.DepartureDate | Arrival date may not be before Departure date. | A data de chegada não pode ser anterior à data de partida. |
| 502 Bad Gateway | InvalidField.Destination.Length | The 'Destination' station code has a maximum length of 3 characters. | O código de Destino tem um comprimento máximo de 3 caracteres. |
| 502 Bad Gateway | InvalidField.FareKey | The 'FareAvailabilityKey' is invalid! | O 'FareAvailabilityKey' é inválido! |
| 502 Bad Gateway | InvalidField.Installments | The 'Installments' cannot be zero or null. | As 'Parcelas' não podem ser zeradas ou nulas. |
| 502 Bad Gateway | InvalidField.MethodCode.Length | The 'MethodCode' must be 2 characters. | O 'MethodCode' deve ter 2 caracteres. |
| 502 Bad Gateway | InvalidField.Miscelaneous.Length | Check the length of fields 'GovId, AccountHolderName and VerificationCode'. | Verifique o comprimento dos campos 'GovId, AccountHolderName e VerificationCode'. |
| 502 Bad Gateway | InvalidField.Organization | The 'Organization' is invalid! | A 'Organização' é inválida! |
| 502 Bad Gateway | InvalidField.OrganizationCode | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. | O 'OrganizationCode' deve ser uma string com comprimento mínimo de 2 e máximo de 10. |
| 502 Bad Gateway | InvalidField.OrganizationCode.Length | The 'OrganizationCode' must be a string with a minimum length of 2 and a maximum length of 10. | O 'OrganizationCode' deve ser uma string com comprimento mínimo de 2 e máximo de 10. |
| 502 Bad Gateway | InvalidField.PassengerType.Length | The 'Passengers.Type' has a maximum length of 3 characters. | O 'Passengers.Type' tem no máximo 3 caracteres. |
| 502 Bad Gateway | InvalidField.Password | The given password violates the password policy. Policy: The password must be numeric, have at least 8 numbers and a maximum of 14. The password cannot contain numerical sequences of three or more digits or numbers repeated more than twice in a row. | A senha fornecida viola a política de senha.  |
| 502 Bad Gateway | InvalidField.PromotionCode | The 'PromotionCode' is invalid! | O 'PromotionCode' é inválido! |
| 502 Bad Gateway | InvalidField.PromotionCode.Length | The 'PromotionCode' has a maximum length of 8 characters. | O 'PromotionCode' tem no máximo 8 caracteres. |
| 502 Bad Gateway | Navitaire.Authenticated.NoAgentRoles | Unable to find valid role for agent. | Não foi possível encontrar uma role válida para o agente. |
| 502 Bad Gateway | Navitaire.Authenticated.Session | An agent is already authenticated. | O agente já está autenticado. |
| 502 Bad Gateway | Navitaire.GetBooking.Failed | The requested order was not found or does not exist. | A order solicitada não foi encontrada ou não existe. |
| 502 Bad Gateway | Navitaire.Request.Failed | The request failed with navitaire. | A solicitação falhou com a navitaire. |
| 502 Bad Gateway | Navitaire.SeatKey.Invalid | Invalid seat key for equipment. | Chave de assento inválida para o equipamento. |
| 502 Bad Gateway | Navitaire.SegmentKey.Invalid | The 'SegmentKey' is invalid. | O 'SegmentKey' é inválido. |
| 502 Bad Gateway | Order.RequestFailed | An error has ocurred retrieving the order from state. | Ocorreu um erro ao recuperar a order do state. |
| 502 Bad Gateway | Order.RequestFailed.Credits | An error occurred while searching for credit. | Ocorreu um erro ao procurar crédito. |
| 502 Bad Gateway | Order.RequestFailed.InsufficientFunds | Not enough funds available. | Não há saldo suficientes disponíveis. |
| 502 Bad Gateway | Order.RequestFailed.NoFunds | The Order in state has no funds. | A Ordem do state não tem saldo. |
| 502 Bad Gateway | Order.RequestFailed.NotUpdated | Unable to update booking. | Não foi possível atualizar a reserva. |
| 502 Bad Gateway | Organization.AuthorizationFailed.User | This user does not have access to the informed organization. | Este usuário não tem acesso à organização informada. |
| 502 Bad Gateway | Organization.NotActive | The Organization is not active. | A Organização não está ativa. |
| 502 Bad Gateway | Passengers.Count.OverMaximum | The sum of adult and child passenger must be less than or equal to 9. | A soma dos passageiros adultos e crianças deverá ser menor ou igual a 9. |
| 502 Bad Gateway | Passengers.Count.UnderMinimum | The minimum count of 'Passenger' array is 1. | A contagem mínima de 'Passageiro' é 1. |
| 502 Bad Gateway | RequestFailed | The request failed. | A solicitação falhou. |
| 502 Bad Gateway | RequestFailed.AssistanceCode.NotAllowed | The informed assistance code is invalid or cannot be added to this journey. | O código de assistência informado é inválido ou não pode ser adicionado a esta journey. |
| 502 Bad Gateway | RequestFailed.Authentication | An error occurred while validating the user authentication. | Ocorreu um erro ao validar a autenticação do usuário. |
| 502 Bad Gateway | RequestFailed.ChangeNotAllowed | The requested journey cannot be changed. | A journey solicitada não pode ser alterada. |
| 502 Bad Gateway | RequestFailed.Comarch | An error occurred while retrieving the data in the comarch. | Ocorreu um erro ao recuperar os dados na comarch. |
| 502 Bad Gateway | RequestFailed.CompletedPayment | The amounts for this order have already been totally paid. | Os valores desta order já foram integralmente pagos. |
| 502 Bad Gateway | RequestFailed.ContactError | Your Order request was succefully processed, but the informed booking contact has errors. | A reauisição foi processada com sucesso, mas o contacto de reserva informado apresenta erros. |
| 502 Bad Gateway | RequestFailed.DeletingError | An error occurred when deleting the order. | Ocorreu um erro ao excluir a order. |
| 502 Bad Gateway | RequestFailed.GetPayment | There was an error retrieving the payment. | Ocorreu um erro ao recuperar o pagamento. |
| 502 Bad Gateway | RequestFailed.IncompletePayment | The Payment must include at least the total amount of the order taxes. | O Pagamento deve incluir pelo menos o valor total dos impostos do pedido. |
| 502 Bad Gateway | RequestFailed.Installments | Installment payment available only for BRL currency code. | Pagamento parcelado disponível apenas para o código de moeda BRL. |
| 502 Bad Gateway | RequestFailed.NotAuthenticated | An error occurred while authenticating. | Ocorreu um erro durante a autenticação. |
| 502 Bad Gateway | RequestFailed.Order.AlreadyExistsInState | There is already an order created in state. | Já existe uma order criada no state. |
| 502 Bad Gateway | RequestFailed.OrderPayments | The order in the current state has not been checked out yet. The CreditType 'Order' only applies to created orders. | O pedido no estado atual ainda não foi verificado.  |
| 502 Bad Gateway | RequestFailed.OverPayment | The informed amount is greater than the balance due for this order. | O valor informado é superior ao saldo devido da order. |
| 502 Bad Gateway | RequestFailed.Payments | An error occurred with the order payments service. | Ocorreu um erro com o serviço de pagamentos de pedidos. |
| 502 Bad Gateway | RequestFailed.SSR.AddNotPossible | It was not possible to add an SSR to the order. | Não foi possível adicionar um SSR a order. |
| 502 Bad Gateway | RequestFailed.StatusAccount | Organization account is Closed/Blocked, please contact Azul's commercial team. | A conta da organização está Fechada/Bloqueada, entre em contato com a equipe comercial da Azul. |
| 502 Bad Gateway | RequestFailed.UnaccompaniedMinor.Information | There are unaccompanied minors in your order, please verify possible costs and required documentations. | Há menores desacompanhados na order, verifique possíveis custos e documentações exigidas. |
| 502 Bad Gateway | RequestFailed.Unexpected | An unexpected error has occurred. | Ocorreu um erro inesperado. |
| 502 Bad Gateway | RequiredField.Amount | The 'Amount' is required. | O 'Valor' é obrigatório. |
| 502 Bad Gateway | RequiredField.CreditCard.MethodCode | The 'MethodCode' is required. | O 'MethodCode' é obrigatório. |
| 502 Bad Gateway | RequiredField.Departure | The 'Departure' is required. | A 'Partida' é obrigatória. |
| 502 Bad Gateway | RequiredField.FareKey | The 'FareKey' is required. | O 'FareKey' é obrigatório. |
| 502 Bad Gateway | RequiredField.JourneyKey | The 'JourneyKey' is required. | A 'JourneyKey' é necessária. |
| 502 Bad Gateway | RequiredField.OrganizationCode | The 'OrganizationCode' is required. | O 'OrganizationCode' é obrigatório. |
| 502 Bad Gateway | RequiredField.PassengerType | The 'Passenger.Type' is required. | O 'Passenger.Type' é obrigatório. |
| 502 Bad Gateway | Resources.RequestFailed | The Resources request failed. | A solicitação do recurso falhou. |
| 502 Bad Gateway | UserOrganization.NotAllowed | The logged user organization does not have access to the requested order. | A organização do usuário logado não tem acesso ao pedido solicitado. |
