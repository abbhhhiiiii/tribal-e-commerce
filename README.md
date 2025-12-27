# Tribal E-Commerce Platform

A full-stack e-commerce platform for tribal products with separate client and server architecture.

## Project Structure

```
tribal-e-commerce/
├── client/          # React frontend application
├── server/          # Express backend API
└── package.json     # Root package.json for running both
```

## Quick Start

### Installation

1. **Install all dependencies:**
   ```bash
   npm run install-all
   ```

   Or install separately:
   ```bash
   npm run install-server
   npm run install-client
   ```

### Running the Application

1. **Development mode (runs both client and server):**
   ```bash
   npm run dev
   ```

2. **Run server only:**
   ```bash
   npm run server
   ```

3. **Run client only:**
   ```bash
   npm run client
   ```

## Server Configuration

Navigate to the `server` folder and create/update `.env` file with your configuration:

```env
PORT=8080
NODE_ENV=development
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLIENT_URL=http://localhost:3000
```

## Available Scripts

- `npm run dev` - Run both client and server concurrently
- `npm run client` - Start React development server
- `npm run server` - Start Express server with nodemon
- `npm run install-all` - Install dependencies for both client and server
- `npm run build` - Build React app for production

## Tech Stack

### Frontend (Client)
- React
- React Router
- Axios
- CSS

### Backend (Server)
- Node.js
- Express
- MongoDB with Mongoose
- JWT Authentication
- Bcrypt
- Multer (file uploads)

## API Endpoints

- `/api/v1/auth` - Authentication routes
- `/api/v1/category` - Category management
- `/api/v1/product` - Product management
- `/api/v1/order` - Order management
- `/api/v1/middleman` - Middleman routes

## License

ISC
