# Development Guide

This document contains development-related information for the Pregnify project.

## 🛠️ Setup Instructions

### Prerequisites
- Node.js (v18 or higher)
- MySQL (v8.0 or higher)
- Git

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Copy `.env.example` to `.env` and configure your environment variables:
   ```bash
   cp .env.example .env
   ```

4. Set up the database:
   ```bash
   npx prisma migrate reset
   npx prisma generate
   npx prisma db push
   ```

5. Start the backend server:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Copy `.env.example` to `.env` and configure your environment variables:
   ```bash
   cp .env.example .env
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

## 🔐 Environment Variables

### Backend (.env)
- `PORT`: Server port (default: 8080)
- `NODE_ENV`: Environment (development/production)
- `MYSQL_DATABASE_URL`: MySQL connection string
- `ACCESS_TOKEN_SECRET`: JWT access token secret
- `REFRESH_TOKEN_SECRET`: JWT refresh token secret
- `SMTP_*`: Email configuration
- `OPENAI_API_KEY`: OpenAI API key
- `OPENAI_API_URL`: OpenAI API URL
- `OPENAI_MODEL`: OpenAI model name

### Frontend (.env)
- `VITE_API_URL`: Backend API URL
- `VITE_ENCRYPTION_KEY`: Frontend encryption key

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
