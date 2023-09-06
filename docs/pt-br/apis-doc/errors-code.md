# Códigos de Erro e Mensagens

Nosso barramento tem diversas regras e tratativas para garantir a integridade do fluxo. Abaixo estão mapeados todos códigos de resposta HTTP, possíveis códigos de erro e suas respectivas mensagens de erro:

## Erros Gerais

| Código HTTP       | Código Interno | Mensagem de Erro                               |
| ----------------- | -------------- | ----------------------------------------------
| 400 Requisição inválida | Agent.DefaultEmail.NotConfigured | O agente informado não possui email padrão configurado. |
| 400 Requisição inválida | Agent.NotActive | O Agente não está ativo. |
| 400 Requisição inválida | AgentOrder.NotAuthorized | O agente não está autorizado a confirmar reservas com status de preço inválido sem solicitar a substituição das restrições. |
| 400 Requisição inválida | CreditNoMatches | Não há crédito disponível para o tipo informado. |
| 400 Requisição inválida | Dates.Range.OverMaximum | A diferença de dias entre 'DepartureBegin' e 'DepartureEnd' não pode ser superior a {0} dias. |
| 400 Requisição inválida | DiscountPayment.TudoAzul | Foi aplicado um desconto na sua reserva pela utilização do cartão TudoAzul. |
| 400 Requisição inválida | FlexibleDays.Disabled | Não é possível obter dias flexíveis porque esse recurso está desativado. |
| 400 Requisição inválida | Infant.Request.Failed | Ocorreu um erro no envio do documento do passageiro. |
| 400 Requisição inválida | Integration.EnterpriseStation | Ocorreu um erro ao retornar as estações. |
| 400 Requisição inválida | Integration.Error | O 'RecordLocator' informado é inválido! |
| 400 Requisição inválida | Integration.Failed | A requisição falhou. |
| 400 Requisição inválida | Integration.InvalidFare | Há um erro nas tarifas solicitadas |
| 400 Requisição inválida | Integration.InvalidField.CurrencyCode | O 'CurrencyCode' é inválido. |
| 400 Requisição inválida | InvalidField.Account | A 'Account' é inválida. |
| 400 Requisição inválida | InvalidField.Account.Length | A 'Account' tem um comprimento máximo de 16 caracteres. |
| 400 Requisição inválida | InvalidField.Address.City | O 'Address.City' possui no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.Address.Country | O 'Address.CountryCode' possui no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.Address.LineOne | O 'Address.LineOne' possui no máximo 128 caracteres. |
| 400 Requisição inválida | InvalidField.Address.LineThree | O 'Address.LineThree' possui no máximo 128 caracteres. |
| 400 Requisição inválida | InvalidField.Address.LineTwo | O 'Address.LineTwo' possui no máximo 128 caracteres. |
| 400 Requisição inválida | InvalidField.Address.PostalCode | O 'Address.PostalCode' tem no máximo 10 caracteres. |
| 400 Requisição inválida | InvalidField.Address.ProvinceState | O 'Address.ProvinceState' possui no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.Amount | O 'Amount' deve ser igual ou maior que zero. |
| 400 Requisição inválida | InvalidField.AssistanceArray | A contagem mínima da lista 'Assistances' é 1. |
| 400 Requisição inválida | InvalidField.AssistancesCount | O 'Assistances.Count' deve ser maior que 0. |
| 400 Requisição inválida | InvalidField.BaggageAllowance | O 'BaggageAllowance' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.Bin | O 'BIN' não é um número válido. |
| 400 Requisição inválida | InvalidField.Bin.Length | O 'BIN' deve ter 6 caracteres. |
| 400 Requisição inválida | InvalidField.Code | O 'Code' deve ter no máximo 4 caracteres. |
| 400 Requisição inválida | InvalidField.Codes | A contagem mínima da lista de 'Codes' é 1. |
| 400 Requisição inválida | InvalidField.Contact.AddressCity | O 'Contact.Address.City' tem no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.Contact.CompanyName | O 'Contact.CompanyName' possui no máximo 64 caracteres. |
| 400 Requisição inválida | InvalidField.Contact.Email | O 'Contact.Email' é inválido. |
| 400 Requisição inválida | InvalidField.Contact.FirstName | O 'Name.First' possui no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.Contact.LastName | O 'Name.Last' possui no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddress.LineOne | O 'Contact.Address.LineOne' tem comprimento máximo de 52 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddress.LineThree | O 'Contact.Address.LineThree' tem comprimento máximo de 52 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddress.LineTwo | O 'Contact.Address.LineTwo' tem comprimento máximo de 52 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddress.PostalCode | O 'Contact.Address.PostalCode' tem no máximo 10 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddress.ProviceState | O 'Contact.Address.ProvinceState' tem no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.ContactAddressLineCountry | O 'Contact.Address.Country' tem no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.ContactName.First | O 'Contact.Name.First' tem comprimento máximo de 32 caracteres. |
| 400 Requisição inválida | InvalidField.ContactName.Last | O 'Contact.Name.Last' tem no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.ContactName.Middle | O 'Contact.Name.Middle' tem comprimento máximo de 32 caracteres. |
| 400 Requisição inválida | InvalidField.ContactName.Suffix | O 'Contact.Name.Suffix' deve ser um enum válido. |
| 400 Requisição inválida | InvalidField.ContactNameT.itle | O 'Contact.Name.Title' deve ser um enum válido. |
| 400 Requisição inválida | InvalidField.ContactPhones.Number | O 'Contact.Phones.Number' tem no máximo 20 caracteres. |
| 400 Requisição inválida | InvalidField.ContactPhones.Type | O 'Contact.Phones.Type' deve ser um enum válido. |
| 400 Requisição inválida | InvalidField.Count.Infant | A contagem de passageiros do tipo 'ADT' deve ser maior que a contagem de passageiros do tipo 'INF'. |
| 400 Requisição inválida | InvalidField.Count.OverMaximum | A soma de 'Passengers.Count' do tipo ADT e CHD deve ser menor ou igual a {0} passageiros. |
| 400 Requisição inválida | InvalidField.Count.UnderMinimum | O valor mínimo de 'Passengers.Count' é 1. |
| 400 Requisição inválida | InvalidField.CountryCode | Ocorreu um erro ao solicitar a reserva. |
| 400 Requisição inválida | InvalidField.CreditAmount.Empty | O valor 'CreditAmount' deve ser maior que zero. |
| 400 Requisição inválida | InvalidField.CriteriaType | O 'CriteriaType' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.CurrencyCode.Length | O 'CurrencyCode' tem um comprimento máximo de 3 caracteres. |
| 400 Requisição inválida | InvalidField.customerProgram.number | Cartas não são permitidas. |
| 400 Requisição inválida | InvalidField.CustomerProgram.Number | O 'Passengers.CustomerProgram.Number' tem no máximo 20 caracteres. |
| 400 Requisição inválida | InvalidField.DateOfBirth | Passageiros menores de 18 anos não são permitidos com bebês. |
| 400 Requisição inválida | InvalidField.DepartureBegin | O 'DepartureBegin' deve ser maior que a data de hoje. |
| 400 Requisição inválida | InvalidField.DepartureDate | A data de chegada não pode ser anterior à data de partida. |
| 400 Requisição inválida | InvalidField.DepartureEnd | O 'DepartureBegin' deve ser maior que 'DepartureEnd'. |
| 400 Requisição inválida | InvalidField.Destination.Length | O código da estação 'Destination' tem um comprimento máximo de 3 caracteres. |
| 400 Requisição inválida | InvalidField.EquipmentCode | O 'EquipmentCode' deve ter no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.ExpirationDate | Data de validade do cartão de crédito inválida. |
| 400 Requisição inválida | InvalidField.ExpirationMonth | O 'ExpirationMonth' deve estar vazio quando MethodCode for {0} |
| 400 Requisição inválida | InvalidField.ExpirationYear | O 'ExpirationYear' deve estar vazio quando MethodCode for {0} |
| 400 Requisição inválida | InvalidField.FareKey | O 'FareKey' é inválido. |
| 400 Requisição inválida | InvalidField.FeeCode | O 'FeeCode' deve ter no máximo 6 caracteres. |
| 400 Requisição inválida | InvalidField.Filter | Só pode ser filtrado por 'Nome de usuário' ou 'Nome'. |
| 400 Requisição inválida | InvalidField.FirstName.Length | O 'Nome' deve ser uma string com comprimento máximo de 128. |
| 400 Requisição inválida | InvalidField.FirstNameMatching | O 'FirstNameMatching' não pode ser inserido com 'Nome de usuário'. |
| 400 Requisição inválida | InvalidField.FlexibleDays.Ahead | O valor mínimo de 'FlexibleDays.Ahead' é {0}. |
| 400 Requisição inválida | InvalidField.FlexibleDays.Behind | O valor mínimo de 'FlexibleDays.Behind' é {0}. |
| 400 Requisição inválida | InvalidField.FlightNumber | Alguns segmentos da Jornada '{0}-{1} - {2}' não suportam a assistência '{3}'.  |
| 400 Requisição inválida | InvalidField.GovId | O 'GovId' é inválido. |
| 400 Requisição inválida | InvalidField.GovId.Length | O 'GovId' tem no máximo 11 caracteres. |
| 400 Requisição inválida | InvalidField.HolderName | O 'HolderName' deve estar vazio quando MethodCode for {0} |
| 400 Requisição inválida | InvalidField.HolderName.Length | O 'HolderName' tem um comprimento máximo de 255 caracteres. |
| 400 Requisição inválida | InvalidField.Infant.DateOfBirth | O 'Infant.DateOfBirth' é inválido. |
| 400 Requisição inválida | InvalidField.Infant.Nationality | A 'Nacionalidade Infantil' tem no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.Installments | As 'Parcelas' não podem ser zero ou nulas. |
| 400 Requisição inválida | InvalidField.IropContact.Email | O 'Passengers.IropContact.Email' tem um comprimento máximo de 128 caracteres. |
| 400 Requisição inválida | InvalidField.IropContact.Mobile | O 'Passengers.IropContact.Mobile' não pode ser informado quando Passengers.IropContact.Refused for True. |
| 400 Requisição inválida | InvalidField.Journey | O Journey.Key '{0}' está duplicado. |
| 400 Requisição inválida | InvalidField.JourneyKey | O 'JourneyKey' é inválido. |
| 400 Requisição inválida | InvalidField.Journeys | A contagem mínima da lista 'Journeys' é 1. |
| 400 Requisição inválida | InvalidField.Journeys.Count | O número máximo de jornadas permitidas em uma reserva é {0}. |
| 400 Requisição inválida | InvalidField.Journeys.OverMaximum | O número de 'Viagens' deve ser menor que {0}. |
| 400 Requisição inválida | InvalidField.Journeys.UnderMinimum | O número de 'Viagens' deve ser maior que {0}. |
| 400 Requisição inválida | InvalidField.LastName | O 'Sobrenome' não pode ser inserido com 'Nome de usuário'. |
| 400 Requisição inválida | InvalidField.LastName.Length | O 'OrganizationCode' deve ser uma string com comprimento máximo de 64. |
| 400 Requisição inválida | InvalidField.LiableRecordLocator | O 'LiableRecordLocator' deve ter 6 caracteres. |
| 400 Requisição inválida | InvalidField.MethodCode | O 'MethodCode' deve ser igual a {0}, {1}. |
| 400 Requisição inválida | InvalidField.MethodCode.Length | O 'MethodCode' deve ter 2 caracteres. |
| 400 Requisição inválida | InvalidField.MiddleName.Length | O 'Nome.Middle' possui no máximo 32 caracteres. |
| 400 Requisição inválida | InvalidField.Miscelaneous.Length | Verifique o comprimento dos campos 'GovId, AccountHolderName e VerificationCode'. |
| 400 Requisição inválida | InvalidField.Name.First | O 'Nome.Primeiro' tem comprimento máximo de 32 caracteres. |
| 400 Requisição inválida | InvalidField.Name.Last | O 'Nome.Último' tem comprimento máximo de 32 caracteres. |
| 400 Requisição inválida | InvalidField.Name.Suffix | O 'Name.Sufix' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.Name.Title | O 'Name.Title' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.Nationality.Length | A 'Nationality' tem um comprimento máximo de 2 caracteres. |
| 400 Requisição inválida | InvalidField.NewPassword | A 'NewPassword' deve ser diferente da 'CurrentPassword'. |
| 400 Requisição inválida | InvalidField.NoFilter | Filtre por 'Nome de usuário' ou 'Nome'. |
| 400 Requisição inválida | InvalidField.Offers | A contagem mínima da lista 'Ofertas' é 1. |
| 400 Requisição inválida | InvalidField.Offers.OverMaximum | A contagem máxima da lista 'oferta' é 4 |
| 400 Requisição inválida | InvalidField.Offers.UnderMinimum | A contagem mínima da lista 'oferta' é 1. |
| 400 Requisição inválida | InvalidField.Organization | A 'Organização' é inválida! |
| 400 Requisição inválida | InvalidField.OrganizationCode.Length | O 'OrganizationCode' deve ser uma string com comprimento mínimo de 2 e máximo de 10. |
| 400 Requisição inválida | InvalidField.OrganizationFeeOverride.Amount | O valor 'Quantidade' deve ser igual ou maior que zero. |
| 400 Requisição inválida | InvalidField.Origin.Length | O código da estação 'Origem' tem um comprimento máximo de 3 caracteres. |
| 400 Requisição inválida | InvalidField.PageNumber | O número da 'Página' deve estar entre {0} e {1}. |
| 400 Requisição inválida | InvalidField.PageSize | O número 'PageSize' deve estar entre {0} e {1}. |
| 400 Requisição inválida | InvalidField.Passenger | A contagem mínima da lista 'passageiros' é 1. |
| 400 Requisição inválida | InvalidField.Passenger.Email | O 'Passenger.Email' é inválido. |
| 400 Requisição inválida | InvalidField.Passenger.IssuingCountry | O 'InvalidField.Passenger.IssuingCountry' possui no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.Passenger.Name | O 'Passengers.Name' é obrigatório. |
| 400 Requisição inválida | InvalidField.Passenger.Nationality | O 'Passageiro.Nacionalidade' tem no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.Passenger.OverMaximum | A contagem máxima da lista 'Passageiro' é 3. |
| 400 Requisição inválida | InvalidField.Passenger.Phone | O 'PassengerAddress.Phone' possui no máximo 20 caracteres. |
| 400 Requisição inválida | InvalidField.Passenger.Type | O 'PassengerRequest.PassengerTypeCode' possui no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.Passenger.UnderMinimum | A contagem mínima da lista 'Passageiro' é 1. |
| 400 Requisição inválida | InvalidField.PassengerAddress.CultureCode | O 'PassengerAddress.CultureCode' possui no máximo 17 caracteres. |
| 400 Requisição inválida | InvalidField.PassengerAddress.StationCode | O 'PassengerAddress.StationCode' possui no mínimo 3 e no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.PassengerCount.UnderMinimum | O 'Passengers.Count' deve ser maior que 0. |
| 400 Requisição inválida | InvalidField.PassengerKeys.Empty | A lista 'PassengerKeys' não pode conter valores vazios. |
| 400 Requisição inválida | InvalidField.PassengerType | O 'Passengers.Type' deve ser igual a 'ADT', 'CHD' ou 'INF'. |
| 400 Requisição inválida | InvalidField.PassengerType.Length | O 'Passengers.Type' tem no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.PassengerType.Repeated | Deve ter apenas um 'Passenger.Type' do tipo ADT. |
| 400 Requisição inválida | InvalidField.Password | A senha fornecida viola a política de senha.  |
| 400 Requisição inválida | InvalidField.ProductClass | O 'ProductClass' deve ter no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.ProgramNumber | O 'ProgramNumber' tem um comprimento máximo de 20 caracteres. |
| 400 Requisição inválida | InvalidField.Promotion.Code | O 'PromotionCode' é inválido. |
| 400 Requisição inválida | InvalidField.PromotionCode | O 'PromotionCode' é inválido! |
| 400 Requisição inválida | InvalidField.PromotionCode.Length | O 'PromotionCode' tem no máximo 8 caracteres. |
| 400 Requisição inválida | InvalidField.ProviderType | O 'ProviderType' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.RefundType | O 'RefundType' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.ServicesCount | O 'Services.Count' deve ser maior que 0. |
| 400 Requisição inválida | InvalidField.StationCode | O 'StationCode' deve ter 3 caracteres. |
| 400 Requisição inválida | InvalidField.TaxAmount | O 'TaxAmount' deve ser maior ou igual a 0. |
| 400 Requisição inválida | InvalidField.TravelDocument.BirthCountry | O 'TravelDocuments.BirthCountry' tem no máximo 2 caracteres. |
| 400 Requisição inválida | InvalidField.TravelDocument.IssuingCountry | O 'TravelDocuments.IssuingCountry' tem no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.TravelDocument.Number | O 'TravelDocuments.Number' tem no máximo 35 caracteres. |
| 400 Requisição inválida | InvalidField.TravelDocument.Type | O 'TravelDocuments.Type' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.TravelDocuments.IssuingCountry | O 'TravelDocuments.IssuingCountry' tem no máximo 3 caracteres. |
| 400 Requisição inválida | InvalidField.TravelDocuments.Type | O 'TravelDocuments.Type' possui no máximo 4 caracteres. |
| 400 Requisição inválida | InvalidField.Type | O 'Tipo' deve ser um Enum válido. |
| 400 Requisição inválida | InvalidField.Username.Length | O 'Nome de usuário' deve ser uma string com comprimento máximo de 128. |
| 400 Requisição inválida | InvalidField.UsernameMatching | O 'UsernameMatching' não pode ser inserido com 'FirstName'. |
| 400 Requisição inválida | InvalidField.VerificationCode | O 'VerificationCode' é inválido. |
| 400 Requisição inválida | InvalidField.VerificationCode.Length | O 'VerificationCode' tem comprimento máximo de 4 caracteres. |
| 400 Requisição inválida | JourneyKey.Decoding.Error | Ocorreu um erro ao decodificar um JourneyKey. |
| 400 Requisição inválida | Journeys.Overlap | Há viagens sobrepostas. |
| 400 Requisição inválida | LiableRecordLocator.UnaccompaniedMinor.Issuing | O 'LiableRecordLocator' só poderá ser informado para emissão de reserva com menores desacompanhados. |
| 400 Requisição inválida | Loyalty.Request.Failed | A solicitação de fidelidade falhou. |
| 400 Requisição inválida | Market.Unavailable | O mercado de origem/destino informado não está atualmente disponível para pesquisa de estimativas de tarifas baixas. |
| 400 Requisição inválida | Navitaire.Authenticated.NoAgentRoles | Não foi possível encontrar uma função válida para o agente. |
| 400 Requisição inválida | Navitaire.Authenticated.Session | Um agente já está autenticado. |
| 400 Requisição inválida | Navitaire.GetBooking.Failed | A reserva solicitado não foi encontrado ou não existe. |
| 400 Requisição inválida | Navitaire.SeatCreate.Failed | A solicitação não conseguiu atribuir assento. |
| 400 Requisição inválida | Navitaire.SeatKey.Invalid | Chave de assento inválida para equipamento. |
| 400 Requisição inválida | Navitaire.SegmentKey.Invalid | O 'SegmentKey' é inválido. |
| 400 Requisição inválida | NotAvailable.Credit | O 'RecordLocator' informado não possui crédito disponível. |
| 400 Requisição inválida | Offer.UnaccompaniedMinor.AdditionalFees | Menores desacompanhados poderão incorrer em taxa adicional, de acordo com a política da empresa. |
| 400 Requisição inválida | Order.Calculation.NotPending | O reserva no estado não tem cálculos a serem feitos. |
| 400 Requisição inválida | Order.Journeys.Count | O número máximo de jornadas permitidas em um reserva é {0}. |
| 400 Requisição inválida | Order.PendingCalculation | Existem cálculos pendentes a serem realizados.  |
| 400 Requisição inválida | Order.RequestFailed | Ocorreu um erro ao recuperar o reserva do estado. |
| 400 Requisição inválida | Order.RequestFailed.Credits | Ocorreu um erro ao procurar crédito. |
| 400 Requisição inválida | Order.RequestFailed.InsufficientFunds | Não há fundos suficientes disponíveis. |
| 400 Requisição inválida | Order.RequestFailed.NoFunds | A Ordem no estado não tem fundos. |
| 400 Requisição inválida | Order.RequestFailed.NotUpdated | Não foi possível atualizar a reserva. |
| 400 Requisição inválida | Order.State.Modified | A ordem no estado foi modificada externamente.  |
| 400 Requisição inválida | OrderDivide.BalanceDue.Positive | O reserva no estado tem saldo devedor positivo. |
| 400 Requisição inválida | OrderDivide.CreditAmount.invalid | O 'creditAmount' informado é inválido por ser maior que o valor disponível no reserva informado. |
| 400 Requisição inválida | OrderDivide.DivideCredit.Failed | Ocorreu um erro ao dividir o crédito do reserva.  |
| 400 Requisição inválida | OrderDivide.PassengerKeys.InvalidAmount | A quantidade de 'passengerKeys' na solicitação deverá ser menor que a quantidade de passageiros do reserva informado. |
| 400 Requisição inválida | OrderDivide.Payments.Empty | O reserva no estado não possui pagamentos informados. |
| 400 Requisição inválida | OrderDivide.Unaccompanied.NotAllowed | Não é permitida a divisão de um reserva quando isso resultar em reservas onde haja apenas menores desacompanhados (menores de {0} anos).  |
| 400 Requisição inválida | Organization.Request.Failed | A solicitação da organização falhou. |
| 400 Requisição inválida | Passenger.DocumentTypeMatch.NotAllowed | Não são permitidos vários passageiros com o mesmo tipo e número de documento de viagem, incluindo bebês. |
| 400 Requisição inválida | Passenger.InvalidAge | Passageiro menor de 12 anos na data do embarque não poderá ser considerado adulto (ADT). |
| 400 Requisição inválida | Passenger.NameMatch.NotAllowed | Não são permitidos vários passageiros com exatamente o mesmo nome, nome do meio, sobrenome e sufixo, incluindo bebês. |
| 400 Requisição inválida | Passenger.TraveDocument.Expired | O documento de viagem informado expirará na data da partida. |
| 400 Requisição inválida | Passenger.Unaccompanied.InvalidAge | Menores devem ter mais de 8 anos para viajar desacompanhados. |
| 400 Requisição inválida | Passengers.Count.OverMaximum | A soma do passageiro adulto e criança deverá ser menor ou igual a 9. |
| 400 Requisição inválida | Passengers.Count.UnderMinimum | A contagem mínima da lista 'Passageiro' é 1. |
| 400 Requisição inválida | Payments.Credit.Failed | Ocorreu um erro ao usar o crédito. |
| 400 Requisição inválida | Payments.ValidationError | Erro de validação de checkout.  |
| 400 Requisição inválida | Refund.NotApplicable | Não há valor no reserva a ser reembolsado. |
| 400 Requisição inválida | RequiredField.Account | A 'Conta' é obrigatória. |
| 400 Requisição inválida | RequiredField.Amount | O 'Valor' é obrigatório. |
| 400 Requisição inválida | RequiredField.AssistanceArray | A lista 'Assistências' é obrigatória. |
| 400 Requisição inválida | RequiredField.AssistancesCount | O 'Assistances.Count' é obrigatório. |
| 400 Requisição inválida | RequiredField.AssistancesKey | A 'Assistências.Key' é necessária. |
| 400 Requisição inválida | RequiredField.Code | O 'Código' é obrigatório. |
| 400 Requisição inválida | RequiredField.Contact.FirstName | O 'Contact.FirstName' é obrigatório. |
| 400 Requisição inválida | RequiredField.Contact.LastName | O 'Contact.LastName' é obrigatório. |
| 400 Requisição inválida | RequiredField.Contact.Phones | O 'Contact.Phones' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactAddress.LineOne | O 'Contact.Address.LineOne' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactName | O objeto 'Contact.Name' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactName.First | O 'Contact.Name.First' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactName.Last | O 'Contact.Name.Last' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactPhones.Number | O 'Contact.Phones.Number' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactPhones.Type | O 'Contact.Phones.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.ContactPhonesHome | O objeto 'Contact.Phones' é necessário. |
| 400 Requisição inválida | RequiredField.CreditCard.ExpirationMonth | O 'ExpirationMonth' é obrigatório. |
| 400 Requisição inválida | RequiredField.CreditCard.ExpirationYear | O 'ExpirationYear' é obrigatório. |
| 400 Requisição inválida | RequiredField.CreditCard.GovId | O 'GovId' é necessário para este código de método devido ao código da moeda do reserva. |
| 400 Requisição inválida | RequiredField.CreditCard.HolderName | O 'HolderName' é obrigatório. |
| 400 Requisição inválida | RequiredField.CreditCard.MethodCode | O 'MethodCode' é obrigatório. |
| 400 Requisição inválida | RequiredField.CreditCard.Type | O 'CreditCard.Type' é obrigatório |
| 400 Requisição inválida | RequiredField.CreditCard.VerificationCode | O 'VerificationCode' é obrigatório. |
| 400 Requisição inválida | RequiredField.Criteria | Os 'Critérios' só são necessários para 'CriteriaType': 'Telefone', 'E-mail', 'DocumentNumber', 'CardNumber' e 'CustomerNumber'. |
| 400 Requisição inválida | RequiredField.CriteriaType | O 'CriteriaType' só é necessário para 'Tipo': 'Organização'. |
| 400 Requisição inválida | RequiredField.CurrencyCode | O 'CurrencyCode' é obrigatório. |
| 400 Requisição inválida | RequiredField.CurrentPassword | Usuário não autenticado.  |
| 400 Requisição inválida | RequiredField.DateOfBirth | O 'DateOfBirth' é obrigatório. |
| 400 Requisição inválida | RequiredField.Departure | A 'Partida' é obrigatória. |
| 400 Requisição inválida | RequiredField.DepartureBegin | O 'DepartureBegin' é obrigatório. |
| 400 Requisição inválida | RequiredField.DepartureDate | A 'Partida' é obrigatória. |
| 400 Requisição inválida | RequiredField.DepartureEnd | O 'DepartureEnd' é obrigatório. |
| 400 Requisição inválida | RequiredField.Destination | O 'Destino' é obrigatório. |
| 400 Requisição inválida | RequiredField.Document.Type | É necessário apresentar CPF, RNE ou PASSAPORTE 'Tipo.Documento.Infantil'. |
| 400 Requisição inválida | RequiredField.DocumentType | O 'DocumentType' é obrigatório para o 'CriteriaType' informado. |
| 400 Requisição inválida | RequiredField.FareKey | O 'FareKey' é obrigatório. |
| 400 Requisição inválida | RequiredField.FirstName | O 'FirstName' é obrigatório para o campo 'FirstNameMatching'. |
| 400 Requisição inválida | RequiredField.FirstNameMatching | O 'FirstNameMatching' é obrigatório para o campo 'FirstName'. |
| 400 Requisição inválida | RequiredField.Gender | O 'Gênero' é obrigatório. |
| 400 Requisição inválida | RequiredField.Infant.FirstName | O 'Infant.FirstName' é obrigatório. |
| 400 Requisição inválida | RequiredField.Infant.Gender | O 'Infantil:Gênero' é obrigatório. |
| 400 Requisição inválida | RequiredField.Infant.LastName | O 'Infant.LastName' é obrigatório. |
| 400 Requisição inválida | RequiredField.IropContact | O 'Passengers.IropContact' é obrigatório. |
| 400 Requisição inválida | RequiredField.IropContact.EmailMobile | O 'Passengers.IropContact.Email' ou 'Passengers.IropContact.Mobile é obrigatório. |
| 400 Requisição inválida | RequiredField.IropContact.Refused | O 'Passengers.IropContact.Refused' é obrigatório. |
| 400 Requisição inválida | RequiredField.JourneyKey | A 'JourneyKey' é necessária. |
| 400 Requisição inválida | RequiredField.Journeys | A lista 'Journeys' é obrigatória. |
| 400 Requisição inválida | RequiredField.Key | A 'Chave' é necessária. |
| 400 Requisição inválida | RequiredField.LastName | O 'Sobrenome' só é necessário para 'CriteriaType': 'PassengerName' ou 'ContactName'. |
| 400 Requisição inválida | RequiredField.Name | O 'Nome' é obrigatório. |
| 400 Requisição inválida | RequiredField.Name.First | O 'Nome.Primeiro' é obrigatório. |
| 400 Requisição inválida | RequiredField.Name.Last | O 'Nome.Último' é obrigatório. |
| 400 Requisição inválida | RequiredField.Name.Middle | O 'Nome.Middle' é obrigatório. |
| 400 Requisição inválida | RequiredField.Nationality | A 'Nacionalidade' é obrigatória. |
| 400 Requisição inválida | RequiredField.NewPassword | A 'Nova Senha' é necessária. |
| 400 Requisição inválida | RequiredField.Offers | A lista 'Ofertas' é obrigatória. |
| 400 Requisição inválida | RequiredField.Offers.FareKey | O 'Offers.FareKey' é obrigatório. |
| 400 Requisição inválida | RequiredField.Offers.JourneyKey | O 'Offers.JouneyKey' é obrigatório. |
| 400 Requisição inválida | RequiredField.OrganizationGroupCode | O 'OrganizationGroupCode' é obrigatório. |
| 400 Requisição inválida | RequiredField.Origin | A 'Origem' é obrigatória. |
| 400 Requisição inválida | RequiredField.Passenger | O 'Passageiro' é obrigatório. |
| 400 Requisição inválida | RequiredField.Passenger.DateOfBirth | O 'Passenger.DateOfBirth' é obrigatório. |
| 400 Requisição inválida | RequiredField.Passenger.Gender | O 'Passenger.Gender' é obrigatório. |
| 400 Requisição inválida | RequiredField.Passenger.Key | A 'PassengerKey' é necessária. |
| 400 Requisição inválida | RequiredField.Passenger.PhoneEmail | O 'Passengers.Phone' ou 'Passengers.Email' é obrigatório. |
| 400 Requisição inválida | RequiredField.Passenger.Type | O 'Passengers.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.PassengerKey | A 'PassengerKey' é necessária. |
| 400 Requisição inválida | RequiredField.PassengerKeys | As 'passengerKeys' informadas na solicitação não existem no reserva informado. |
| 400 Requisição inválida | RequiredField.Passengers | A lista 'Passageiros' é obrigatória. |
| 400 Requisição inválida | RequiredField.PassengerType | O 'Passenger.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.PassengerType.Adult | O valor 'Passengers.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.Password | A 'Senha' é necessária. |
| 400 Requisição inválida | RequiredField.PhonesNumber | O 'Phones.Number' é obrigatório. |
| 400 Requisição inválida | RequiredField.PhonesType | O 'Phones.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.ProviderType | O 'ProviderType' é obrigatório. |
| 400 Requisição inválida | RequiredField.RecordLocator | O 'RecordLocator' é necessário. |
| 400 Requisição inválida | RequiredField.SegmentKey | A 'segmentkey' é necessária. |
| 400 Requisição inválida | RequiredField.Services | A lista 'Serviços' é obrigatória. |
| 400 Requisição inválida | RequiredField.ServicesCount | O 'Services.Count' é obrigatório. |
| 400 Requisição inválida | RequiredField.ServicesKey | O 'Services.Key' é obrigatório. |
| 400 Requisição inválida | RequiredField.SessionContext | O 'SessionContext' é obrigatório. |
| 400 Requisição inválida | RequiredField.Status | O 'Status' é obrigatório. |
| 400 Requisição inválida | RequiredField.TravelDocument | A contagem mínima da lista 'TravelDocument' é 1. |
| 400 Requisição inválida | RequiredField.TravelDocument.ExpirationDate | O 'TravelDocuments.ExpirationDate' é obrigatório. |
| 400 Requisição inválida | RequiredField.TravelDocument.Number | O 'TravelDocuments.Number' é obrigatório. |
| 400 Requisição inválida | RequiredField.TravelDocument.Type | É necessário o CPF, RNE ou PASSAPORTE 'TravelDocuments.Type'. |
| 400 Requisição inválida | RequiredField.TravelDocuments.IssuingCountry | O 'TravelDocuments.IssuingCountry' é obrigatório. |
| 400 Requisição inválida | RequiredField.TravelDocuments.Type | O 'TravelDocuments.Type' é obrigatório. |
| 400 Requisição inválida | RequiredField.UnitKey | A 'unitkey' é necessária. |
| 400 Requisição inválida | RequiredField.UserKey | A 'UserKey' é necessária. |
| 400 Requisição inválida | RequiredField.Username | O 'Username' é obrigatório. |
| 400 Requisição inválida | Resources.RequestFailed | A solicitação de recursos falhou. |
| 400 Requisição inválida | Shopping.Request.Failed | A solicitação do Shopping falhou. |
| 400 Requisição inválida | Stations.NotAllowed | Estas estações solicitadas são inválidas: |
| 400 Requisição inválida | TudoAzul.Categorization.Failed | Houve falha na categorização do TudoAzul de 'passageiros.customerProgram.number': {0}.  |
| 400 Requisição inválida | User.CannotBeUnlocked | Somente usuários da API podem ser desbloqueados. |
| 400 Requisição inválida | User.Password.Expired | Senha expirada, o usuário deve alterar a senha. |
| 400 Requisição inválida | Warning.OrganizationFeeOverride | A substituição da taxa de organização não se aplica a este reserva. |
| 401 Não Autorizado | InvalidToken.Expired | Ocorreu um erro ao executar a autenticação. |
| 401 Não Autorizado | InvalidToken.NotAuthenticated | O Bearer Token fornecido é inválido ou expirou. |
| 401 Não Autorizado | RequestFailed.Authentication | Ocorreu um erro durante a autenticação. |
| 403 Proibido | Agent.NoAccess | O agente não tem acesso ao usuário informado. |
| 403 Proibido | AssignSeat.UnitKey.Blocked | A solicitação não conseguiu atribuir o assento, pois este assento está bloqueado pelas regras do passageiro (idade, SSR ou equipamento). |
| 404 Não encontrado | Assistance.NoMatches | Esta assistência não existe ou não foi encontrada. |
| 404 Não encontrado | Assistances.NoMatches | Assistência não encontrada na viagem especificada. |
| 404 Não encontrado | AssistancesKey.NoMatches | A 'Assistances.Key' informada não existe ou não pertence a uma 'assistência/busca' recuperada anteriormente. |
| 404 Não encontrado | BagKey.NoMatches | A 'Chave' informada não existe ou não pertence a uma 'bagagem/busca' previamente recuperada. |
| 404 Não encontrado | Code.NoMatches | O serviço informado é inválido. |
| 404 Não encontrado | Countries.NoMatches | Não foi possível recuperar os dados dos países. |
| 404 Não encontrado | Country.NoMatches | Este país não existe ou não foi encontrado. |
| 404 Não encontrado | CustomerNumber.NoMatches | O 'CustomerProgram' não encontrado. |
| 404 Não encontrado | CustomerProgram.NoMatches | O Programa do Cliente não foi encontrado. |
| 404 Não encontrado | CustomProgram.NotMatch | O nome do passageiro não corresponde ao Programa do Cliente informado. |
| 404 Não encontrado | Equipment.NoMatches | Este equipamento não existe ou não foi encontrado. |
| 404 Não encontrado | Fare.NoMatches | Esta tarifa não existe ou não foi encontrada. |
| 404 Não encontrado | Fares.NoMatches | Não foi possível recuperar os dados das tarifas. |
| 404 Não encontrado | Fee.NoMatches | Esta taxa não existe ou não foi encontrada. |
| 404 Não encontrado | Fees.NoMatches | Não foi possível recuperar os dados de taxas. |
| 404 Não encontrado | JourneyKey.NoMatches | O 'JourneyKey' é inválido ou não existe no estado atual. |
| 404 Não encontrado | NoMatches | O usuário informado não existe ou não foi encontrado. |
| 404 Não encontrado | Order.NoMatches | O reserva solicitado não foi encontrado ou não existe. |
| 404 Não encontrado | OrderCache.NoMatches | Um reserva deve ser anexado. |
| 404 Não encontrado | OrderSearch.NoMatches | Não foram encontrados reservas para os filtros de busca informados. |
| 404 Não encontrado | Organization.NoMatches | A organização informada é inválida ou o usuário logado não tem permissão para utilizá-la! |
| 404 Não encontrado | OrganizationGroup.NoMatches | O grupo organizacional informado não existe ou não foi encontrado. |
| 404 Não encontrado | PassengerKey.NoMatches | A 'PassengerKey' informada não corresponde àquelas do reserva em estado. |
| 404 Não encontrado | PassengerName.NoMatches | O Passageiro não corresponde ao número de cliente TudoAzul. |
| 404 Não encontrado | Payments.NoMatches | Nenhum pagamento foi encontrado para o reserva no estado. |
| 404 Não encontrado | RecordLocator.NoMatches | Seu reserva deve ser criado para utilizar seus créditos. |
| 404 Não encontrado | Seat.NoMatches | Assento não encontrado. |
| 404 Não encontrado | SeatMap.NoMatches | Não há assentos correspondentes. |
| 404 Não encontrado | SegmentKey.NoMatches | O 'SegmentKey' é inválido ou não existe no estado atual. |
| 404 Não encontrado | Service.NoMatches | Serviço não encontrado na jornada especificada. |
| 404 Não encontrado | ServiceKey.NoMatches | O 'Services.Key' informado não existe ou não pertence a um 'serviço/busca' recuperado anteriormente. |
| 404 Não encontrado | SessionContextToken.NoMatches | Nenhuma sessão encontrada para o provedor fornecido. |
| 404 Não encontrado | Station.NoMatches | Esta estação não existe ou não foi encontrada. |
| 404 Não encontrado | Stations.NoMatches | Não foi possível recuperar os dados das estações. |
| 404 Não encontrado | TudoAzul.NoMatches | O 'passengers.customerProgram.number' informado: {0} não existe ou não foi encontrado. |
| 404 Não encontrado | TudoAzulNames.NoMatches | Os nomes dos 'passageiros.customerProgram.number' informados: {0} não correspondem aos cadastrados no TudoAzul. |
| 404 Não encontrado | UnitKey.NoMatches | O 'UnitKey' é inválido ou não existe no estado atual. |
| 404 Não encontrado | User.NoMatches | O usuário informado não existe ou não foi encontrado. |
| 409 Conflito | AssignSeat.PassengerKey.Conflict | O PassengerKey não existe no estado do reserva. |
| 409 Conflito | AssignSeat.Seat.Conflict | Assento já atribuído. |
| 409 Conflito | InvalidField.AssistanceCode | A assistência '{0}' é inválida para a Jornada '{1}-{2} - {3}'. |
| 409 Conflito | InvalidField.AssistanceLimit | A contagem de 'Assistances.key' {0} é maior que o limite especificado. |
| 409 Conflito | InvalidField.Assistanceskey | Existem 'Assistances.key' {0} duplicados. |
| 409 Conflito | InvalidField.PassengerKeyCache | O serviço solicitado não está disponível para o passageiro informado. |
| 409 Conflito | InvalidField.RecordLocator | O 'RecordLocator' deve ter 6 caracteres. |
| 409 Conflito | InvalidField.ServiceLimit | A contagem de 'Services.key' {0} é maior que o limite especificado. |
| 409 Conflito | InvalidField.Serviceskey | Existem 'Services.key' {0} duplicados. |
| 409 Conflito | LiableRecordLocator.UnaccopaniedMinor.NotMatchJourneys | reservas responsáveis \u200b\u200be voos de reservas de menores desacompanhados devem coincidir. |
| 409 Conflito | NotEmpty.State | Não é possível anexar um reserva já recuperado no estado atual.  |
| 409 Conflito | Order.HasRecordLocator | Este método é para reservas em processo de criação.  |
| 409 Conflito | Order.Recordlocator.Empty | Este método é para reservas criados anteriormente.  |
| 409 Conflito | Order.State.Change | Não é permitido remover uma viagem após adicionar viagens.  |
| 409 Conflito | Order.UnaccopaniedMinor.OperatedFligthAzul | Menores desacompanhados são permitidos apenas em voos operados pela Azul. |
| 409 Conflito | Order.UnderCreationException | Este método é para reservas em processo de criação.  |
| 409 Conflito | RequestFailed.UnaccompaniedMinor.DomesticFligths | Menores desacompanhados são permitidos apenas em voos domésticos brasileiros. |
| 409 Conflito | RequestFailed.UnaccompaniedMinor.Information | Há menores desacompanhados em seu reserva, verifique possíveis custos e documentações exigidas. |
| 409 Conflito | RequestFailed.UnaccopaniedMinor.OnlyDirectFlight | Menores desacompanhados são permitidos apenas em voos diretos. |
| 409 Conflito | RequiredField.LiableRecordLocator | É necessário um passageiro maior de 18 anos na ordem responsável. |
| 412 Falha na pré-condição | Quote.UnaccompaniedMinor.NotAllowed | O 'JourneyKeys' {0} não permite menores desacompanhados. |
| 422 Conteúdo não processável | Assistance.SearchRequired | Recupere uma 'assistência/pesquisa' com travelKey antes de executar este método. |
| 422 Conteúdo não processável | Baggage.SearchRequired | Recupere uma 'bagagem/pesquisa' com travelKey antes de executar este método. |
| 422 Conteúdo não processável | NotMatch.Name | Os nomes enviados não correspondem aos do reserva em anexo. |
| 422 Conteúdo não processável | NotMatch.PassengerKey | A chave do passageiro informada não existe no reserva anexo ou é inválida. |
| 422 Conteúdo não processável | Order.RetrieveRequired | O reserva solicitado não foi encontrado ou não existe. |
| 422 Conteúdo não processável | Order.State.Timeout | O tempo estadual para este reserva expirou.  |
| 422 Conteúdo não processável | SeatMapCache.SearchRequired | Nenhum mapa de assentos encontrado ou gerado no estado.  |
| 422 Conteúdo não processável | Service.SearchRequired | Recupere um 'serviços/pesquisa' com travelKey antes de executar este método. |
| 422 Conteúdo não processável | UnitKey.SearchRequired | A UnitKey informada não pertence a um SeatMap recuperado anteriormente ou a recuperação anterior expirou. |
| 502 Bad Gateway | AuthorizationFailed.Credentials | Ocorreu um erro durante a autenticação. |
| 502 Bad Gateway | InvalidField.OrganizationCode | O 'OrganizationCode' é inválido. |
| 502 Bad Gateway | Navitaire.Request.Failed | A solicitação falhou. |
| 502 Bad Gateway | Organization.AuthorizationFailed.User | Este usuário não tem acesso à organização informada. |
| 502 Bad Gateway | Organization.NotActive | A Organização não está ativa. |
| 502 Bad Gateway | RequestFailed | A solicitação falhou. |
| 502 Bad Gateway | RequestFailed.AssistanceCode.NotAllowed | O código de assistência informado é inválido ou não pode ser adicionado a esta viagem. |
| 502 Bad Gateway | RequestFailed.ChangeNotAllowed | A viagem solicitada não pode ser alterada. |
| 502 Bad Gateway | RequestFailed.Comarch | Ocorreu um erro ao recuperar os dados no comarch. |
| 502 Bad Gateway | RequestFailed.CompletedPayment | Os valores deste reserva já foram integralmente pagos. |
| 502 Bad Gateway | RequestFailed.ContactError | O seu reserva de encomenda foi processado com sucesso, mas o contacto de reserva informado apresenta erros. |
| 502 Bad Gateway | RequestFailed.CreditCard.Expired | Cartão de crédito expirado. |
| 502 Bad Gateway | RequestFailed.DeletingError | Ocorreu um erro ao excluir o reserva. |
| 502 Bad Gateway | RequestFailed.Enterprise | Ocorreu um erro ao validar os nomes dos passageiros do reserva. |
| 502 Bad Gateway | RequestFailed.GetPayment | Ocorreu um erro ao recuperar o pagamento. |
| 502 Bad Gateway | RequestFailed.IncompletePayment | O Pagamento deve incluir pelo menos o valor total dos impostos do reserva. |
| 502 Bad Gateway | RequestFailed.Installments | Pagamento parcelado disponível apenas para o código de moeda BRL. |
| 502 Bad Gateway | RequestFailed.International.Required | O cancelamento da taxa de organização só é permitido para encomendas com viagens internacionais. |
| 502 Bad Gateway | RequestFailed.Journeys.NotAllowed | A substituição da taxa de organização só é permitida ao adicionar novas viagens ao reserva. |
| 502 Bad Gateway | RequestFailed.NotAuthenticated | Ocorreu um erro durante a autenticação. |
| 502 Bad Gateway | RequestFailed.Order.AlreadyExistsInState | Já existe um reserva criado no estado. |
| 502 Bad Gateway | RequestFailed.OrderPayments | O reserva no estado atual ainda não foi verificado.  |
| 502 Bad Gateway | RequestFailed.OverPayment | O valor informado é superior ao saldo devido deste reserva. |
| 502 Bad Gateway | RequestFailed.PassengerMinor.NotAllowedInfants | Passageiros menores de 18 anos não podem ter crianças como acompanhantes. |
| 502 Bad Gateway | RequestFailed.Passengers.WithoutFee | Nenhum passageiro nesta ordem tem cobrança de taxas de organização. |
| 502 Bad Gateway | RequestFailed.Payments | Ocorreu um erro com o serviço de pagamentos de reservas. |
| 502 Bad Gateway | RequestFailed.SSR.AddNotPossible | Não foi possível adicionar uma SSR ao reserva. |
| 502 Bad Gateway | RequestFailed.TudoAzul.Retrieve | Ocorreu um erro ao recuperar o programa TudoAzul. |
| 502 Bad Gateway | RequestFailed.Unexpected | Ocorreu um erro inesperado. |
| 502 Bad Gateway | RequiredField.OrganizationCode | O 'OrganizationCode' é obrigatório. |
| 502 Bad Gateway | UserOrganization.NotAllowed | A organização do usuário logado não tem acesso ao reserva solicitado. |