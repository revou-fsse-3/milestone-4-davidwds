# Milestone 4 - Revo U

## Banking App Documentation

[Postman Documentation](https://documenter.getpostman.com/view/32204090/2sA358cQVw)

### User Management:

- **POST /users:** Create a new user account.
- **GET /users/id:** Retrieve the profile of the currently authenticated user.
- **PUT /users/id:** Update the profile information of the currently authenticated user.

### Account Management:

- **GET /accounts:** Retrieve a list of all accounts belonging to the currently authenticated user.
- **GET /accounts/:id:** Retrieve details of a specific account by its ID. (Authorization required for account owner)
- **POST /accounts:** Create a new account for the currently authenticated user.
- **PUT /accounts/:id:** Update details of an existing account. (Authorization required for account owner)
- **DELETE /accounts/:id:** Delete an account. (Authorization required for account owner)

### Transaction Management:

- **GET /transactions:** Retrieve a list of all transactions for the currently authenticated user's accounts. (Optional: filter by account ID, date range)
- **GET /transactions/:id:** Retrieve details of a specific transaction by its ID. (Authorization required for related account owner)
- **POST /transactions:** Initiate a new transaction (deposit, withdrawal, or transfer). (Authorization required for related account owner)
