# Hero Flat Application - Backend

This is the backend part of the Hero Flat Application, a fully-fledged, full-stack dynamic web app built with Prisma, Express, TypeScript, PostgreSQL, and other modern technologies. The backend provides features like authentication, validation, filtering, and CRUD operations, which are consumed by the frontend.

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js
- npm or yarn
- Prisma
- TypeScript
- PostgreSQL
- Cors
- Validation Packages (Zod)
- ExpressJS
- JWT

## Project Structure

```
Hero Flat Application Backend/
├── src/
│   ├── app/
│   ├── config/
│   ├── modules/
│   ├── app.ts
│   └── server.ts
├── .env
├── .gitignore
├── package.json
├── tsconfig.json
└── README.md
```

## Getting Started

### Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/KawsarCoder/Hero-Flat-Backend
cd hero-flat-backend
npm install
# or
yarn install
```

### Database Setup

1. Ensure PostgreSQL is installed and running.
2. Create a new database for the application.
3. Configure the database connection in the `.env` file.

Example `.env` file:

```
DATABASE_URL="postgresql://username:password@localhost:5432/hero_flat_db"
JWT_SECRET="your_jwt_secret"
PORT=4000
```

### Running the Project

**Development:**

```bash
npm run start:dev
# or
yarn start:dev
```

The development server will start on `http://localhost:4000`.

**Production:**

```bash
npm run build
# or
yarn build
```

After building, you can start the production server with:

```bash
npm start
# or
yarn start
```

### Available Scripts

- `start:dev`: Runs the application in development mode.
- `build`: Builds the application for production.
- `start`: Starts the application in production mode.
- `lint`: Runs ESLint for code quality checks.

### Prisma Migrations

To apply database migrations:

```bash
npx prisma migrate dev
```

To generate Prisma client:

```bash
npx prisma generate
```

## Features

- **Authentication**: Secure user authentication with JWT.
- **Role Management**: Different functionalities for Admin, Super Admin, and User roles.
- **CRUD Operations**: Create, read, update, and delete flats.
- **Filtering**: Filter flats based on various criteria.
- **Validation**: Input validation using Zod.
- **ORM**: Database management with Prisma.

## Role Features

### Admin

- Manage users (edit, delete, role change, status change).
- Manage all flat requests.
- Add, edit, delete flats.

### User

- View all flats and details.
- Request available flats.
- Update profile.
- Check flat and request status from the dashboard.

## URLs

- **Frontend**: [Hero Flat Frontend](https://hero-flat-frontend.vercel.app/)
- **Backend**: [Hero Flat Backend](https://hero-flat-backend.vercel.app/)

## Video Overview

For a comprehensive overview of the application features, please watch the [full overview video](https://drive.google.com/file/d/1uOCoHrM12E6NOYDOs-EX1GGgLE-2iY9n/view?usp=sharing).
