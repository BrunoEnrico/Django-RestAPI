# Simple Blog REST API

This repository contains a simple REST API for a blog built using Django and deployed on Heroku. The API allows users to add and delete blog posts, offering a basic yet functional backend for blog management.

## Features

- Add new blog posts with a title, content, and publication date.
- Delete existing blog posts by their unique ID.
- RESTful architecture for seamless integration with frontend applications or other services.

## Technologies Used

- **Django**: Backend framework for rapid development and clean design.
- **Django REST Framework (DRF)**: For building RESTful APIs.
- **Heroku**: Cloud platform for deployment.
- **Python**: Core programming language.


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/BrunoEnrico/Django-RestAPI
   cd Django-RestAPI
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the database:
   ```bash
   python manage.py migrate
   ```

5. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Deployment

This application is deployed on Heroku. To deploy it yourself:
1. Set up a Heroku account and install the Heroku CLI.
2. Create a new Heroku app:
   ```bash
   heroku create
   ```
3. Push your code to Heroku:
   ```bash
   git push heroku main
   ```
4. Set up environment variables (e.g., `DJANGO_SECRET_KEY`) in your Heroku dashboard.

## Usage

Once the API is running, use tools like `Postman` or `curl` to interact with the endpoints. For example, to list all blog posts:
```bash
curl -X GET https://bfernandes-djangoapi-21613d605475.herokuapp.com
```

## Future Improvements

- Implement user authentication and permissions.
- Add update functionality for blog posts.
- Include pagination for large datasets.
