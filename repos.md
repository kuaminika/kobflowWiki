# Kobflow Repos

Map of all repos that make up the Kobflow project, and what each one owns.

## Clients

### kobflow-web
Main frontend (react website). Started as a standalone log viewer 
(`kobFlow.LogManagement`) and grew into the full rebuild after the 
original React app was found to have too much coupling and didn't scale.

- **Stack:** React
- **Status:** WIP
- **Repo:** https://github.com/kuaminika/kobFlow.LogManagement

### kobflow-mobile
Mobile app (Ionic).

- **Stack:** Ionic (React)
- **Status:** not started / planned
- **Repo:** N/A

## Gateway

### kobflow-gateway *(placeholder name — confirm actual repo name)*
`phpGateway` — handles routing and (currently) authentication.

- **Stack:** PHP
- **Status:** WIP
- **Repo:**  https://github.com/kuaminika/KobFlowAPI

## .NET Services

### kobflow-api *(placeholder name — confirm actual repo name)*
Single repo containing all .NET domain APIs, each running as an 
independent service on the VPS:

  - Expense API
  - Income API
  - Kobholder API
  - IncomeSource API
  - ExpenseCategory API
  - IncomeCategory API
  - Merchant API

- **Stack:** .NET (C#)
- **Depends on:** kobflow-Database
- **Status:** stable - subject to change
- **Repo:** https://github.com/kuaminika/Kuaminika.KobFlow

## Node.js Services

### kobflow-log-service
- **Stack:** Node.js
- **Depends on:** kobflow-Database
- **Status:** WIP
- **Repo:**  https://github.com/kuaminika/kobflow.LogManagementService

### kobflow-user-module
- **Stack:** Node.js
- **Depends on:** MongoDB
- **Notes:** will eventually receive delegated auth from phpGateway
- **Status:** 
- **Repo:** https://github.com/kuaminika/kobFLow.UserService

### kobflow-import-service
Handles bulk inserts of expenses from CSVs.

- **Stack:** Node.js
- **Depends on:** MongoDB
- **Status:** 
- **Repo:** https://github.com/kuaminika/kobFlow.import



### kobflow-email-service
- **Stack:** Node.js
- **Notes:** triggered by kobflow-user-module on registration
- **Status:** not yet started
- **Repo:** N/A

### kobflow-payment-service
- **Stack:** Node.js
- **Depends on:** MongoDB, external Payment Provider (TBD)
- **Status:** not yet started
- **Repo:** N/A

## Docs

### kobflow-wiki
This repo. Documentation only, no code.

- **Repo:**