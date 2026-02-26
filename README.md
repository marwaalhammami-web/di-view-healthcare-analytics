# DI-VIEW Integrated Setup

This project consists of two Next.js applications:
- **frontend**: The main DI-VIEW application
- **landing**: The landing page that directs users to the main application

## Setup Instructions

The setup is configured to allow both applications to work together seamlessly, with the landing page being served at the root path and the main application accessible via links from the landing page.

### Running the Applications

1. Install dependencies for both applications:
   ```
   # In the frontend directory
   cd frontend
   npm install --legacy-peer-deps
   
   # In the landing directory
   cd ../landing
   npm install --legacy-peer-deps
   ```

2. Start both applications with a single command:
   ```
   # In the frontend directory
   cd frontend
   npm run dev:all
   ```

This will start:
- The landing page app on port 3001
- The main frontend app on port 3000
- The frontend app will proxy requests to the landing page for the root URL path

### How It Works

- When you visit `http://localhost:3000/`, you'll see the landing page
- When you click "Get Started" or any login-related buttons, you'll be directed to the main app's login page at `http://localhost:3000/auth/login`
- The main app handles all non-landing page routes

## Development

- To modify the landing page, edit files in the `landing` directory
- To modify the main application, edit files in the `frontend` directory

The configuration in `frontend/next.config.mjs` handles the proxy setup, and the links in the landing page are configured to point to the main application's login page. 
