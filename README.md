# Postman Collection README

## Overview
This repository contains a Postman collection designed to **test and interact with the PetStore API**. The collection includes pre-configured requests for various API endpoints, enabling quick and easy testing.

## Prerequisites
- [Postman](https://www.postman.com/downloads/): Ensure Postman is installed on your machine.
- API credentials (if required): Make sure you have the necessary tokens, API keys, or authentication details.

## How to Use

### 1. Import the Collection
1. Download the `collection.json` file from this repository.
2. Open Postman and click on the **Import** button.
3. Select the `Test_CRUD.postman_collection` file and click **Open**.

### 2. Set Up Environment (if applicable)
1. If the collection uses variables, set up a new environment in Postman:
   - Go to the **Environments** tab in Postman.
   - Create a new environment and define the required variables (e.g., `{{pet_url}}`, `{{apiKey}}`).

### 3. Execute Requests
- Browse the collection in Postman to view the available requests.
- Each request is pre-configured with parameters and example data.
- Click **Send** to execute the request and view the response.

## Endpoints
The collection includes the following endpoints:
### Positives

- **GET `/user/test21`**: [Get user infos]
- **POST `/user`**: [Create user (eg. 'test21')]
- **PUT `/user/test2`**: [Update user password]
- **DELETE `/user/test21`**: [Remove user record]

  ### Negatives

- **GET `/user/test22`**: [Get non existing user infos]
- **POST `/user`**: [Create user already created (eg. 'test21')]
- **PUT `/user/test22`**: [Update non existing user password]
- **DELETE `/user/test21`**: [Remove non existing user record]

## Variables
Define the following variables in your Postman environment:

| Variable       | Description                        | Example                     |
|----------------|------------------------------------|-----------------------------|
| `{{pet_url}}`  | Pet URL of the API               | `https://petstore.swagger.io/v2`  |
| `{{apiKey}}`   | API key for authentication        | `12345abcdef`              |
