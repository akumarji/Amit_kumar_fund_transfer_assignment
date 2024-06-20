# Fund Transfer Service

This is fund transfer service with currency exchange

#### How to build the project

- Clone the project from git repository.
- Import as a maven project in IDE using pom.xml of the application
- Do a maven build with goal "clean install"


### Prerequisite
- Maven
- JDK 17+

  
### Data
Initial data (src\main\resources\data.sql) will be loaded in the H2 database when application start.
> INSERT INTO ACCOUNTS (ACCOUNT_ID, BALANCE, CURRENCY, DEBIT_CARD, CREDIT_CARD, VERSION)
> (1, 1000, 'EUR', 1, 1, 1),
> (2, 1000, 'INR', 1, 1, 1);


## Feature
This application is for demo only. It provides APIs for following 2 features
- Retrieve Account details
- Fund transfer with exchange rate

  ### Basic API Information
| Method | Path | Usage |
| --- | --- | --- |
| GET | /api/accounts/{accountId} | retrieve account details |
| POST | /api/transactions | create transfer transaction |


### Swagger-UI
API Specification is provided in the [swagger-ui page](http://localhost:8080/swagger-ui.html) after spring boot application start.
```
http://localhost:8080/swagger-ui.html
```
