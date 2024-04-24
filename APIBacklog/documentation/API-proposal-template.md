# API Proposal Template
This template captures all the information that a partner should fill out when proposing a new API (or API family) to CAMARA.


| **Field** | Description | 
| ---- | ----- |
| API family name | Tenure |
| API family owner | Vodafone |
| API summary | Establish a level of trust against mobile ID by verifying the length of tenure for a mobile user bound to a mobile number; tenure means the period of time a MSISDN has been associated with a specific user. API checks whether the lifetime tenure of a given MSISDN is longer than an input date. [Use Case] Enterprises can use Tenure API to gauge and establish a level of trust (or Trust Score) with a mobile user who is associated with a specific mobile number, based on how long they have been associated with that number. |
| Technical viability | The data for this API comes from backend systems/sources (i.e. CRM). 
| Commercial viability | To Establish level of trust (or Trust Score) against a mobile ID (MSISDN). The the Tenure API will return a True or False answer as to whether the customer's tenure with an operator has been longstanding.[Sample Request]: * Customer Request: Customer submits MSISDN to understand if the mobile number has been registered to a CSP for longer than a specific date * Request: {"tenure_before_date":{"value": "2019-01-15"}} * API   Response: True/False -  if tenure is longer than specified date + billing segment  (PAYG/PAYM/Business) * Sample   Response: "tenure_before_date_check":   true,    "billing_segment":   "PAYM"|
| YAML code available? | YES |
| Validated in lab/productive environments? | YES |
| Validated with real customers? | YES - TMT Analysis |
| Validated with operators? | YES - Telefonica, Hutchinson Group |
| Supporters in API Backlog Working Group | List of supporters. <br><em> NOTE: That shall be added by the Working Group. </em> |
