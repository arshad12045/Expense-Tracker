# Expense Tracker Application

This is a full-stack expense tracker application built with React for the frontend and Node.js with Express for the backend. The application allows users to track their expenses, providing a user-friendly interface to add, view, and manage expenses.

## Project Structure

The project is divided into two main parts: the client and the server.

### Client

The client is built using React and TypeScript. It includes the following key components:

- **`public/index.html`**: The main HTML file that serves as the entry point for the React application.
- **`src/index.tsx`**: The entry point for the React application, rendering the App component.
- **`src/App.tsx`**: The main App component that sets up routing and layout.
- **`src/api/apiClient.ts`**: Functions for making API requests to the backend server.
- **`src/components/ExpenseList.tsx`**: Displays a list of expenses.
- **`src/components/ExpenseForm.tsx`**: Provides a form for adding new expenses.
- **`src/components/Header.tsx`**: Displays the application title and navigation.
- **`src/pages/Dashboard.tsx`**: Shows the dashboard with expense statistics and the expense list.
- **`src/pages/Settings.tsx`**: A page for user settings.
- **`src/hooks/useExpenses.ts`**: A custom hook for managing expenses state and logic.
- **`src/services/expenseService.ts`**: Functions for interacting with expense-related API endpoints.
- **`src/styles/index.css`**: Global styles for the application.
- **`src/types/index.ts`**: TypeScript types and interfaces used throughout the client application.

### Server

The server is built using Node.js, Express, and Prisma. It includes the following key components:

- **`src/index.ts`**: The entry point for the backend server, initializing the Express app.
- **`src/app.ts`**: Sets up middleware, routes, and error handling.
- **`src/controllers/expenses.controller.ts`**: Handles expense-related requests.
- **`src/routes/expenses.routes.ts`**: Sets up routes for expense-related endpoints.
- **`src/services/expenses.service.ts`**: Business logic related to expenses.
- **`src/models/expense.model.ts`**: Defines the data model for expenses.
- **`src/db/prismaClient.ts`**: Exports an instance of the Prisma client for database interactions.
- **`src/middleware/auth.ts`**: Middleware for authentication and authorization.
- **`src/types/index.ts`**: TypeScript types and interfaces used throughout the server application.
- **`prisma/schema.prisma`**: Defines the Prisma schema for the database.

## Getting Started

### Prerequisites

- Node.js
- npm or yarn
- Docker (optional, for containerized deployment)

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd expense-tracker-app
   ```

2. Install dependencies for the client:
   ```
   cd client
   npm install
   ```

3. Install dependencies for the server:
   ```
   cd server
   npm install
   ```

### Running the Application

To run the application in development mode:

1. Start the server:
   ```
   cd server
   npm run dev
   ```

2. Start the client:
   ```
   cd client
   npm start
   ```

### Docker

To run the application using Docker, you can use the provided `docker-compose.yml` file. Run the following command in the root directory of the project:

```
docker-compose up
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.