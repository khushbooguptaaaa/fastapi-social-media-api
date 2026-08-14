# FastAPI Social Media API 🚀

A backend REST API for a social media application, built with FastAPI, PostgreSQL and SQLAlchemy.

The project supports user registration, JWT-based authentication and CRUD operations for posts. It was developed to strengthen my understanding of backend architecture, relational databases, API security and request validation.

## Features

* User registration
* Secure password hashing
* JWT-based login and authentication
* Protected API routes
* Create, read, update and delete posts
* PostgreSQL database integration
* SQLAlchemy ORM
* Request and response validation with Pydantic
* Interactive Swagger API documentation
* Postman collection for API testing
* Environment variables for sensitive configuration

## Tech Stack

* **Language:** Python
* **Framework:** FastAPI
* **Database:** PostgreSQL
* **ORM:** SQLAlchemy
* **Authentication:** JWT and OAuth2
* **Validation:** Pydantic
* **API Testing:** Postman and Swagger UI
* **Version Control:** Git and GitHub

## Project Structure

```text
fastapi-social-media-api/
├── app/                 # FastAPI application
├── .postman/            # Postman configuration
├── postman/             # Postman globals
├── .gitignore
└── README.md
```

## API Functionality

### Authentication

* Register a new user
* Log in with user credentials
* Generate a JWT access token
* Authenticate requests using a Bearer token

### Users

* Create a user
* Retrieve user information

### Posts

* Create a post
* Retrieve all posts
* Retrieve a post by ID
* Update a post
* Delete a post
* Restrict protected operations to authenticated users

## Running the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/khushbooguptaaaa/fastapi-social-media-api.git
cd fastapi-social-media-api
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Activate it on macOS or Linux:

```bash
source venv/bin/activate
```

### 3. Install the dependencies

Add a `requirements.txt` file to the repository, then run:

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file and add the database and JWT configuration expected by the application.

Never commit the `.env` file or expose passwords and secret keys publicly.

### 5. Start the development server

Run the application using the module path configured in the project. For example:

```bash
uvicorn app.main:app --reload
```

### 6. Open the API documentation

After starting the server, visit:

```text
http://127.0.0.1:8000/docs
```

## API Testing

The endpoints can be explored through:

* Swagger UI at `/docs`
* Postman using the collection included in the repository

For protected routes, log in first and pass the generated JWT as a Bearer token.

## What I Learned

Through this project, I gained hands-on experience with:

* Designing RESTful APIs
* Connecting FastAPI with PostgreSQL
* Modelling relational data using SQLAlchemy
* Implementing JWT authentication
* Protecting routes and managing authenticated users
* Validating API data with Pydantic
* Testing and debugging APIs with Postman and Swagger
* Managing secrets safely through environment variables

## Planned Improvements

* Add automated tests with Pytest
* Add database migrations with Alembic
* Improve exception handling and validation
* Add pagination and filtering
* Containerize the application with Docker
* Deploy the API
* Add CI/CD with GitHub Actions

## Author

**Khushboo Gupta**

* GitHub: https://github.com/khushbooguptaaaa
* LinkedIn: www.linkedin.com/in/khushboogupta0305

---

If you find this project useful, feel free to explore the repository and share your feedback.
