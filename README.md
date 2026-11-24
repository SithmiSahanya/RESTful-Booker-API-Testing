# RESTful Booker API Testing

## Project Overview

This project focuses on testing the RESTful Booker API using Postman. The objective is to validate API functionality, verify responses, test authentication, and identify potential issues through positive and negative testing.

## API Under Test

- **API:** RESTful Booker API
- **Base URL:** https://restful-booker.herokuapp.com
- **Documentation:** https://restful-booker.herokuapp.com/apidoc/index.html

## Tools & Technologies

- Postman
- JavaScript (Postman test scripts)
- REST API
- JSON
- Microsoft Excel
- Git and GitHub (for version control and project sharing)

## Testing Scope

### Functional Testing
- API health check
- Retrieve all booking IDs
- Retrieve booking details
- Create a booking
- Update a booking using PUT
- Partially update a booking using PATCH
- Delete a booking
- Verify deleted bookings

### Authentication Testing
- Generate authentication token
- Authenticate with invalid username
- Authenticate with incorrect password
- Verify authenticated requests

### Negative Testing
- Missing required fields
- Invalid data types
- Invalid Boolean values
- Invalid date format

## Project Structure

```text
RESTful-Booker-API-Testing/
├── Postman/
│   ├── RESTful_Booker_Collection.json
│   └── RESTful_Booker_Environment.json
├── Test-Cases/
│   └── RESTful_Booker_API_Test_Cases.xlsx
├── Test-Reports/
├── Screenshots/
└── README.md
```

## Test Documentation

The Excel workbook contains:
- API test cases
- Preconditions and test steps
- Expected and actual results
- Test execution status
- Potential bug reports
- Test execution summary

## Potential Defects Identified

The following behaviours were observed and documented for further review:

1. API returns 500 Internal Server Error when firstname is missing.
2. API accepts an invalid data type for totalprice.
3. API converts an invalid depositpaid value into a Boolean.
4. API accepts an invalid check-in date format.

These are documented as potential defects requiring further review against the API requirements.

## How to Run the Tests

1. Install Postman.
2. Import the collection JSON file.
3. Import the environment JSON file.
4. Select the RESTful Booker environment.
5. Run the authentication request to generate a token.
6. Execute the required API requests.
7. Review the response status codes, response bodies, and test results.

## Disclaimer

This project uses the publicly available RESTful Booker demo API for educational and portfolio purposes.