# Business Blueprint

Business Blueprint is a web application designed to help users create and manage business plans and pitch decks efficiently.

## Features

- **Pitch Deck Generator**: Create professional pitch decks with customizable templates.
- **Business Plan Editor**: Edit and export business plans in Markdown format.
- **File Uploads**: Upload logos and other assets for your business plans.
- **Export Options**: Export pitch decks to PDF and business plans to Markdown.
- **Collaboration**: Share pitch decks with team members.

## Project Structure

### Key Directories

- **client/**: Contains the frontend code, including React components and pages.
- **server/**: Contains the backend code, including API routes and database logic.
- **shared/**: Contains shared code, such as schemas and utilities.
- **tests/**: Contains unit and integration tests.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/business-blueprint.git
   cd business-blueprint
   ```

2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Development

- **Frontend**: The frontend is built with React and Vite. The entry point is `client/index.html`.
- **Backend**: The backend is built with Node.js and TypeScript. The entry point is `server/index.ts`.

## Database Management

This project uses **Prisma** as the ORM for database management. Prisma provides a type-safe and modern way to interact with the database.

### Setup

1. Install Prisma CLI:
   ```bash
   npm install prisma --save-dev
   ```

2. Initialize Prisma:
   ```bash
   npx prisma init
   ```

3. Define your database schema in `prisma/schema.prisma`.

4. Run migrations to apply schema changes:
   ```bash
   npx prisma migrate dev
   ```

5. Generate Prisma Client:
   ```bash
   npx prisma generate
   ```

### Notes
- Prisma replaces Drizzlekit due to security vulnerabilities.
- Ensure your database connection string is correctly set in the `.env` file.

## Scripts

- `npm run dev`: Start the development server.
- `npm run build`: Build the project for production.
- `npm run test`: Run tests.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.