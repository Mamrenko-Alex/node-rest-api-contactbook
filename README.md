# ContactBook

ContactBook is a web application that allows users to add, edit, and delete contacts through an API interface. Additionally, it supports adding images to contacts and email verification.

## Description

ContactBook offers the following features:
- Adding new contacts
- Editing existing contacts
- Deleting contacts
- Adding contacts to favorites
- Adding images to contacts
- Email verification for user accounts

## Technologies

The project is built using the following technologies:
- MongoDB
- Node.js
- Express
- Nodemailer

## Installation

To install and run the project, follow these steps:

1. Clone the repository:

    ```sh
    git clone https://github.com/your_username/ContactBook.git
    ```

2. Navigate to the project directory:

    ```sh
    cd ContactBook
    ```

3. Install the dependencies:

    ```sh
    npm install
    ```

4. Create a `.env` file in the root directory of the project and add your environment variables:

    ```plaintext
    JWT_SECRET=your_jwt_secret
    PORT=your_port
    UKRNET_EMAIL_FROM=your_ukrnet_email
    UKRNET_EMAIL_PASSWORD=your_ukrnet_email_password
    HOST_URL=your_host_url
    DB_HOST=your_mongodb_uri
    ```

## Usage

To run the project, use one of the following commands:

- To run in development mode with automatic server restarts on file changes:

    ```sh
    npm run dev
    ```

- To run in normal mode:

    ```sh
    npm start
    ```

- To run tests:

    ```sh
    npm test
    ```

## API Routes

### Contacts

- `GET /contacts` - Get all contacts (requires token)
- `GET /contacts/:id` - Get contact by ID (requires token)
- `POST /contacts` - Create a new contact (requires token)
- `PUT /contacts/:id` - Update contact by ID (requires token)
- `DELETE /contacts/:id` - Delete contact by ID (requires token)
- `PATCH /contacts/:id/favorite` - Add/remove contact from favorites (requires token)

### Users

- `POST /users/register` - Register a new user
- `POST /users/login` - User login
- `POST /users/logout` - User logout (requires token)
- `GET /users/current` - Get current user information (requires token)
- `PATCH /users` - Change user subscription (requires token)
- `GET /users` - Get all users (admin route)
- `POST /users/verify` - Verify user email

## Contact

If you have any questions, please contact me at:

- [LinkedIn](https://www.linkedin.com/in/oleksandr-mamrenko-ab845426b/)
- Email - mamrenko.dev@gmail.com
- Telegram - @mamrenko_dev
