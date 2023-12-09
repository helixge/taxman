# taxman.ge
Tiny tax manager

## Summary

- Static client-side CRUD web application.

- Uses public Google APIs.

- Gets exchange rates from the National Bank of Georgia public API.

- Save data in the Google Sheets document as sheets.


## Pages

### 1. Welcome page
<img width="596" alt="image" src="https://github.com/helixge/taxman/assets/132610/0981ddb7-c458-407a-a915-53ce93d80166">

Create or select Google Sheets documents.

Buttons:

- Create a new

- Open existing


### 2. Dashboard page
<img width="595" alt="image" src="https://github.com/helixge/taxman/assets/132610/46d9c546-0c8a-4d94-9530-6a34e2b99d48">

Monthly income report.

Fields:

- Year

- Month

- Monthly Income

- Monthly VAT

- Monthly Income Tax

- Monthly Amount after taxes.


### 3. Income page
<img width="598" alt="image" src="https://github.com/helixge/taxman/assets/132610/a75e66fb-9e8c-4865-bf41-418ffc73809d">

Add, edit and delete income entries

List Entries.

<img width="602" alt="image" src="https://github.com/helixge/taxman/assets/132610/1d6e7c1d-a9fc-4b91-b38b-2257aeaad8e3">

In edit mode, Senders can be added without leaving the form.

Auto-calculated Amount in GEL by integrating with National Bank of Georgia API for exchange rates.


### 4. Settings page
<img width="597" alt="image" src="https://github.com/helixge/taxman/assets/132610/74be01cf-e9b8-439c-af20-f576899509b2">

Edit income tax and VAT percentages.


## Data Sources

### 1. Senders sheet

- Name\
  Non-empty text

- Tax Code\
  Text of length between 9 and 11


### 2. Income sheet

- Date

- Sender\
  Reference selector to a sender in the Senders sheet

- Amount\
  Numeric, greater than 0

- Currency Name\
  Text field, three letter currency ISO code

- Currency Rate\
  Numeric, greater than 0


### 3. Settings Sheet

- Income Tax Percent\
  Numeric field,  greater than or equal to 0

- VAT Percent\
  Numeric field,  greater than or equal to 0


## Integrations

- Google API\
  Managing Google Sheets and Drive functionalities

- National Bank of Georgia API\
  Provides daily exchange rates.
