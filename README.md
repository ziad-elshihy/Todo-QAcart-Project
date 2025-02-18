# Todo-QAcart-Project

## Overview

This project is an API testing suite for the Todo application hosted at [`https://todo.qacart.com`](https://todo.qacart.com). The tests are created using **Postman** and include various test cases for user authentication and task management.

## Project Structure

This repository contains the following key files:

- **`Todo_QACart_Project.postman_collection.json`** - The main Postman collection containing all API requests and tests.
- **`stage.postman_environment.json`** - Environment file with variables for the staging environment.
- **`workspace.postman_globals.json`** - Global variables used across all requests.

## Prerequisites

To use this project, you need:

- [Postman](https://www.postman.com/downloads/)
- A valid account on [`https://todo.qacart.com`](https://todo.qacart.com)
- Basic knowledge of API testing

## Setup Instructions

1. **Import the Postman Collection and Environment**
   - Open Postman.
   - Go to `File -> Import`.
   - Select the `Todo_QACart_Project.postman_collection.json` file.
   - Import the `stage.postman_environment.json` file.

2. **Set Up Environment Variables**
   - Open the **"Environments"** tab in Postman.
   - Select the "stage" environment.
   - Fill in the required values such as `email`, `token`, and `task_id` if applicable.

3. **Run the API Tests**
   - Open the `Collections` tab.
   - Select `Todo_QACart_Project`.
   - Click `Run` to execute all test cases.

## Test Cases

### User Authentication
- **User Registration**
  - Happy Path: Register a new user successfully.
  - Email Validation: Check for duplicate, empty, or invalid email formats.
  - Password Validation: Ensure password meets length requirements.

- **User Login**
  - Happy Path: Log in with valid credentials.
  - Invalid Login: Handle wrong email, empty password, or incorrect password attempts.

### Task Management
- **Task Creation**
  - Add a valid task.
  - Prevent adding empty or invalid tasks.

- **Task Completion**
  - Mark a task as completed.
  - Revert a task to incomplete status.

- **Task Update**
  - Modify an existing task.