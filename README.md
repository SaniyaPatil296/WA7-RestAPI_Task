# REST API Testing Suite

## Project Overview

This project contains a testing suite for a Django REST Framework API. It tests authentication and task management functionality using pytest.

## Technologies Used

- Python
- Django
- Django REST Framework
- Pytest
- Pytest-Django
- Pytest-Cov
- SQLite

## Project Features Tested

### Authentication API

- User registration
- Login with valid and invalid credentials
- Duplicate username and email validation
- Password mismatch validation
- Authenticated user profile
- Logout and token invalidation

### Task Management API

- Create, list, retrieve, update, and delete tasks
- Task validation for title, status, and priority
- Authentication and authorization
- User-specific task access
- Task filtering and searching
- Unauthorized access handling

## Testing Approach

- API integration tests using Django REST Framework APITestCase.
- Tests cover successful operations and failure scenarios.
- Coverage measurement using pytest-cov.

## Installation

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd RestAPI_Task
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run database migrations:

```bash
python manage.py migrate
```

## Run Tests

```bash
pytest
```

## Run Tests with Coverage

```bash
pytest --cov=authentication --cov=tasks --cov-report=term-missing
```

## Test Results

- Total tests: 26
- Passed: 26
- Failed: 0
- Application code coverage: 92%
- Required coverage: 80%

## Conclusion

The testing suite successfully tests authentication and task management API functionality. All 26 tests pass, and the application code achieves 92% test coverage, exceeding the required 80% threshold.
