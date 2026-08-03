# Entities

Core domain entities in Kobflow.

## Expense
A single spending transaction. Belongs to an `ExpenseCategory` and is 
associated with a `Merchant` and a `Kobholder` (the account/wallet the 
money left from).

## Income
A single incoming money transaction. Belongs to an `IncomeCategory` and 
an `IncomeSource`, and is associated with a `Kobholder` (the account/
wallet the money landed in).

## ExpenseCategory
Classification for expenses (e.g. groceries, rent, transport).

## IncomeCategory
Classification for incomes (e.g. salary, freelance, gift).

## IncomeSource
Where an income originates from — e.g. an employer, a client, a 
platform. Distinct from `IncomeCategory`, which classifies the *type* 
of income rather than its origin.

## Merchant
Where an expense was made — a store, vendor, or service.

## Kobholder
An account or wallet that money flows through — e.g. a bank account, 
cash wallet, or mobile money account. Every expense and income is tied 
to a kobholder representing where the money moved from or to.

---

*Definitions above are a first draft based on API/entity names — please 
correct any that don't match the actual intended meaning, especially 
the relationships between entities (e.g. does Expense really link to 
both Merchant and Kobholder, or just one of them?).*