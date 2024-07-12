# Largerly - A Clone of Medium

Largerly is a clone of the popular blogging platform Medium, built to showcase the ability to create a full-featured web application with user authentication, blog creation, and management. This project is developed using modern web technologies and frameworks to provide a seamless experience for both developers and users.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- User Authentication (Signup, Login)
- Create, Read, Update, Delete (CRUD) Blogs
- JWT-based Authorization
- User Profiles
- Blog Listings
- Responsive Design

## Technologies Used

- **Backend:**
  - [Hono](https://hono.dev/) - A small, simple, and fast web framework
  - [Prisma](https://www.prisma.io/) - Database toolkit and ORM
  - [JWT](https://jwt.io/) - JSON Web Tokens for secure authentication
  - [SQLite](https://www.sqlite.org/index.html) - Lightweight database for development

- **Frontend:**
  - [React](https://reactjs.org/) - JavaScript library for building user interfaces
  - [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework

## Installation



4. **Set up environment variables:**
    Create a `.env` file in the `server` directory and add the following variables:
    ```env
    DATABASE_URL="file:./dev.db"
    JWT_SECRET="your_jwt_secret"
    ```

5. **Run database migrations:**
    ```bash
    cd ../server
    npx prisma migrate dev
    ```


## Usage

Once the server and client are running, you can access the application at `http://localhost:3000`. Sign up for a new account or log in with an existing account to start creating and managing your blogs.

## API Endpoints

### User Routes

- `POST /api/v1/user/signup` - Sign up a new user
- `POST /api/v1/user/signin` - Sign in an existing user

### Blog Routes

- `POST /api/v1/blog` - Create a new blog post
- `PUT /api/v1/blog` - Update an existing blog post
- `GET /api/v1/blog/bulk` - Get all blog posts
- `GET /api/v1/blog/:id` - Get a specific blog post by ID

## Contributing

Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are warmly welcome.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README further to better match your project's specifics and structure.
