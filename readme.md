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
<img width="1137" alt="image" src="https://github.com/helixge/taxman/assets/132610/9ceded8a-9357-4c62-b9e0-fbe487231a98">


Add, edit and delete income entries

List Entries.

<img width="1232" alt="image" src="https://github.com/helixge/taxman/assets/132610/a3f5fe7e-0d46-4f94-a68d-0688c8605967">


### 4. Settings page
<img width="728" alt="image" src="https://github.com/helixge/taxman/assets/132610/d24d5ee7-9480-4dcd-86f8-35566eb44f01">


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
