# Intro to Backend

A backend development project built using **Node.js, Express.js, and MongoDB**. This project demonstrates user authentication and CRUD operations through REST APIs.

## Technologies Used

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* bcrypt
* Postman
* Git & GitHub

## Project Structure

```text
Backend/
└── src/
    ├── config/
    │   ├── constants.js
    │   └── database.js
    ├── controllers/
    │   ├── post.controller.js
    │   └── user.controller.js
    ├── models/
    │   ├── post.model.js
    │   └── user.model.js
    ├── routes/
    │   ├── post.route.js
    │   └── user.route.js
    ├── app.js
    └── index.js
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/prakharjain-cell/Intro-to-Backend.git
```

2. Navigate to the project directory:

```bash
cd Intro-to-Backend
```

3. Install dependencies:

```bash
npm install
```

## Environment Configuration

Create a `.env` file in the root directory:

```env
MONGODBURI=your_mongodb_connection_string
PORT=8000
```

Replace the MongoDB connection string with your own Atlas connection string.

**Never upload your `.env` file or database credentials to GitHub.**

## Run the Project

Start the development server:

```bash
npm run dev
```

The server runs on:

```text
http://localhost:8000
```

## API Endpoints

### User APIs

| Method | Endpoint                 | Description         |
| ------ | ------------------------ | ------------------- |
| POST   | `/api/v1/users/register` | Register a new user |
| POST   | `/api/v1/users/login`    | Login user          |

### Post APIs

| Method | Endpoint                   | Description        |
| ------ | -------------------------- | ------------------ |
| POST   | `/api/v1/posts/create`     | Create a post      |
| GET    | `/api/v1/posts/getPosts`   | Retrieve all posts |
| PATCH  | `/api/v1/posts/update/:id` | Update a post      |
| DELETE | `/api/v1/posts/delete/:id` | Delete a post      |

## Testing

All APIs were tested using Postman, and successful responses were received for registration, login, and post CRUD operations.

## Author

**Prakhar Jain**

B.Tech Computer Science Engineering
