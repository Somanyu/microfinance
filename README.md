# Microfinance Tracker
Microfinance Tracker is a web application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It allows users to track their microfinance expenses by sending WhatsApp messages. The application provides features like authentication, validation, and data visualization.

## Features

- User registration and login: Users can create an account and log in to access their personal dashboard.
- JWT authentication: JSON Web Tokens (JWT) are used to authenticate users and protect routes.
- Password encryption: User passwords are securely encrypted using bcrypt.js before storing them in the database.
- WhatsApp integration: Users can send messages to a WhatsApp number to add expenses, which are then stored in the database.
- Expense tracking: Users can view their expense history, filter expenses by month or year, and visualize data using charts.
- Form validation: User input is validated on both the client and server sides to ensure data integrity.
- Responsive UI: The user interface is designed using Flowbite and Tailwind CSS, making it mobile-friendly and visually appealing.

## Technologies Used

### Client-side

- React: JavaScript library for building user interfaces.
- Redux Toolkit: State management library for managing user authentication status.
- Axios: Promise-based HTTP client for making API requests.
- Chart.js: JavaScript charting library for data visualization.
- Formik: Form library for handling form validation and submission.
- Yup: JavaScript schema builder for form validation.
- React Router DOM: Library for declarative routing in React.
- React Icons: Collection of popular icon libraries as React components.
- React Paginate: Pagination component for React.
- React Toastify: Notification library for displaying user-friendly toast messages.
- Animate.css: CSS animation library.

### Server-side

- Node.js: JavaScript runtime environment for server-side development.
- Express.js: Web application framework for Node.js.
- MongoDB: NoSQL database for storing user information and expense data.
- Mongoose: Object Data Modeling (ODM) library for MongoDB.
- Bcrypt.js: Library for password hashing and encryption.
- Joi: Schema validation library for JavaScript.
- JSON Web Tokens (JWT): Authentication mechanism for securing routes.
- Twilio: API for integrating WhatsApp messaging functionality.

## Getting Started

### Prerequisites

- Node.js and npm: Make sure you have Node.js and npm installed on your machine.

### Installation

1. Clone the repository:
```cmd 
git clone https://github.com/Somanyu/finproject.git
```

2. Navigate to the project directory:
```cmd
cd finproject
```

3. Install the dependencies for the client-side and server-side:

```cmd
cd client
npm install
cd ../server
npm install
```

4. Configure environment variables:

- Create a `.env` file in the server directory.
- Define the required environment variables (e.g., database connection string, Twilio credentials).

5. Start the server side:
```cmd
cd ../client
npm run devstart
```
6. Open a new terminal and start the client:
```cmd
cd server
npm start
```
7. Open your browser and access the application at `http://localhost:3000`.

8. Connect to the Twilio WhatsApp Sandbox:

- Send a WhatsApp message from your phone to the Twilio WhatsApp sandbox number.
- In the message body, send the command: `join discover-series`.
- You will receive a confirmation message once you have successfully connected to the sandbox.

## Usage

1. Register a new account using your email, full name, phone and password.
2. Log in to your account using your credentials.
3. Send WhatsApp messages to the specified number in the required format (e.g., "Add soap 20").
4. See your total expenses in WhatsApp message by sending a text "Show"
5. View your expense history and charts on the dashboard.

## Contributing

Contributions to Microfinance Tracker are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](https://github.com/Somanyu/microfinance/blob/master/LICENSE).
