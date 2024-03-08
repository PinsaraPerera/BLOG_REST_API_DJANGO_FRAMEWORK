# Django BlogPost API

## Introduction

Welcome to the Django BlogPost API repository. This REST API is developed using the Django Rest Framework (DRF) and allows users to perform CRUD operations on blog posts. It's designed for developers looking to integrate blog functionalities into their projects with minimal setup.

## Features

- **Create Blog Posts:** Users can create new blog posts by sending a POST request with the title, content, and author information.
- **Read Blog Posts:** Users can retrieve a list of all blog posts or a single post by its ID.
- **Update Blog Posts:** Existing blog posts can be updated by sending a PUT or PATCH request with new data.
- **Delete Blog Posts:** Any blog post can be removed from the database by sending a DELETE request.

## Installation

Follow these steps to set up the API in your local development environment:

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/PinsaraPerera/BLOG_REST_API_DJANGO_FRAMEWORK.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mysite
   ```
3. Install the required dependencies:
   ```bash
   python install -r requirements.txt
   ```
4. Run the migrations to create the database schema:
   ```bash
   python manage.py migrate
   ```
5. Finally, start the development server:
   ```bash
   python manage.py runserver
   ```

Now, the API should be accessible at `http://localhost:8000/`.

## API Endpoints

The following endpoints are available:

- **GET /blogposts/**: List all blog posts.
- **POST /blogposts/**: Create a new blog post.
- **GET /blogposts/<id>/**: Retrieve a blog post by ID.
- **DELETE /blogposts/<id>/**: Delete a blog post by ID.

## Usage Examples

Here are some example usages of the API:

### Creating a Blog Post

Request:

```http
POST /blogposts/
Content-Type: application/json

{
    "id": 1,
    "title": "testing",
    "content": "testing content",
    "published_date": "2024-03-08T05:45:57.498399Z"
}
```
