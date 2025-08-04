
# Backend Project

This is a TypeScript-based backend project using Express.js and Prisma ORM.

## Project Structure

```
backend/
├── .env                   # Environment variables
├── package.json           # Node.js dependencies and scripts
├── tsconfig.json          # TypeScript configuration
├── prisma/                # Prisma ORM setup and migrations
│   ├── schema.prisma
│   └── migrations/
├── src/                   # Source code
│   ├── config.ts          # Configuration file
│   ├── index.ts           # Entry point
│   ├── middleware.ts      # Middleware setup
│   └── router/            # Route definitions
│       ├── merchant.ts
│       └── user.ts
```

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd backend
```

### 2. Install Dependencies

Using npm:

```bash
npm install
```

Or using yarn:

```bash
yarn install
```

### 3. Configure Environment Variables

Create a `.env` file in the root of the `backend/` directory with the necessary environment variables.

### 4. Prisma Setup

Generate Prisma client and apply migrations:

```bash
npx prisma generate
npx prisma migrate dev
```

### 5. Run the Project

To run in development mode:

```bash
npx ts-node src/index.ts
```

Or if compiled to JavaScript:

```bash
node dist/index.js
```

## Scripts

Refer to the `package.json` file for available scripts.

## Technologies Used

- TypeScript
- Express.js
- Prisma ORM
- Node.js

## License

This project is licensed under the MIT License.
