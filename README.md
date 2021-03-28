# Exercise 1: Submit a pull request to OpenFIGI

### About
You will need to write an example that is able to make use of the OpenFigi API.

### Pre-requisites
* Get familiar with the openFIGI API

### Instructions
1. Clone the openFIGI examples API repository
2. Write an example in a language that hasnt been implimented yet
3. Submit pull request


### Example inputs
As inputs, your program should take in a list of job objects eg:

```
[
    { 
        "idType": "ID_ISIN", 
        "idValue": "US4592001014" 
    },
    { 
        "idType": "ID_WERTPAPIER", 
        "idValue": "851399", 
        "exchCode": "US" 
    },
    { 
        "idType": "ID_BB_UNIQUE", 
        "idValue": "EQ0010080100001000", 
        "currency": "USD" 
    },
    { 
        "idType": "ID_SEDOL", 
        "idValue": "2005973", 
        "micCode": "EDGX", 
        "currency": "USD"
    },
    ...
]     
```
### Example outputs

As outputs, your program should print the response object to the console. eg

```
[{
    "data": [{
        "figi": "BBG000NHN466",
        "securityType": "Common Stock",
        "marketSector": "Equity",
        "ticker": "IBMGBX",
        "name": "INTL BUSINESS MACHINES CORP",
        "uniqueID": "EQ0000000005051123",
        "exchCode": "EU",
        "shareClassFIGI": "BBG001S5S399",
        "compositeFIGI": "BBG000NHN304",
        "securityType2": "Common Stock",
        "securityDescription": "IBMGBX",
        "uniqueIDFutOpt": null
    }, {
        "figi": "BBG000NRMJ71",
        "securityType": "Common Stock",
        "marketSector": "Equity",
        "ticker": "IBMGBX",
        "name": "INTL BUSINESS MACHINES CORP",
        "uniqueID": "EQ0000000005140428",
        "exchCode": "XL",
        "shareClassFIGI": "BBG001S5S399",
        "compositeFIGI": "BBG000NRMD01",
        "securityType2": "Common Stock",
        "securityDescription": "IBMGBX",
        "uniqueIDFutOpt": null
    }]
}, {
    "data": [{
        "figi": "BBG009R4CLR3",
        "marketSector": "Govt",
        "securityType": "US GOVERNMENT",
        "ticker": "T 2 08/15/25",
        "name": "US TREASURY N/B",
        "exchCode": "BERLIN",
        "securityDescription": "T 2 08/15/25",
        "securityType2": "Note",
        "uniqueID": null,
        "compositeFIGI": null,
        "shareClassFIGI": null,
        "uniqueIDFutOpt": null
    }]
},
{
    "error": "No identifier found."
},
...
]      
```