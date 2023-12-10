# taxman.ge
Tiny tax manager

## Summary

- Static client-side CRUD web application.

- Uses public Google APIs.

- Gets exchange rates from the National Bank of Georgia public API.

- Save data in the Google Sheets document as sheets.


## Pages

### 1. Welcome page
<img width="795" alt="image" src="https://github.com/helixge/taxman/assets/132610/6917c1bf-02ae-4907-89cb-6a7a402f3936">



Create or select Google Sheets documents.

Buttons:

- Create a new

- Open existing


### 2. Dashboard page
<img width="914" alt="image" src="https://github.com/helixge/taxman/assets/132610/296b5951-e7e3-44c2-85a8-049add0d05eb">



Monthly income report.

Fields:

- Year

- Month

- Monthly Income

- Monthly VAT

- Monthly Income Tax

- Monthly Amount after taxes.


### 3. Income page
<img width="959" alt="image" src="https://github.com/helixge/taxman/assets/132610/b6a58d00-88e0-4413-bd4b-07be576944b4">


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
