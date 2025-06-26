# Express API Boilerplate

A modern Express.js API boilerplate with TypeScript, ESLint, Prettier, Jest, and Husky.

## Features

- ⚡ **Express.js** - Fast, unopinionated web framework
- 🔷 **TypeScript** - Type-safe JavaScript
- 🎯 **ESLint** - Code linting and quality
- 💅 **Prettier** - Code formatting
- 🧪 **Jest** - Testing framework with supertest
- 🐕 **Husky** - Git hooks for code quality
- 📦 **Modern tooling** - Hot reload, build optimization

## Quick Start

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone git@github.com:AngelRodRo/express-api-boilerplate.git
cd express-api-boilerplate

# Install dependencies
npm install

# Copy environment files
cp env.example .env
cp env.test.example .env.test

# Start development server
npm run dev
```

### Available Scripts

```bash
# Development
npm run dev          # Start development server with hot reload
npm run build        # Build for production
npm start           # Start production server

# Testing
npm test            # Run tests
npm run test:watch  # Run tests in watch mode
npm run test:coverage # Run tests with coverage

# Code Quality
npm run lint        # Run ESLint
npm run lint:fix    # Fix ESLint issues
npm run format      # Format code with Prettier
npm run format:check # Check code formatting
```

## Project Structure

```
├── src/
│   ├── app.ts              # Main application file
│   ├── app.test.ts         # Tests for app.ts
│   └── setupTests.ts       # Jest setup
├── .eslintrc.js            # ESLint configuration
├── .prettierrc             # Prettier configuration
├── .husky/                 # Git hooks
├── jest.config.js          # Jest configuration
├── tsconfig.json           # TypeScript configuration
├── env.example             # Environment variables example
├── env.test.example        # Test environment variables example
└── package.json            # Project dependencies and scripts
```

## Environment Configuration

Copy the example environment files and configure them for your environment:

```bash
cp env.example .env
cp env.test.example .env.test
```

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `NODE_ENV` | Environment mode | `development` |
| `PORT` | Server port | `3000` |
| `API_VERSION` | API version | `v1` |
| `API_PREFIX` | API route prefix | `/api` |
| `LOG_LEVEL` | Logging level | `info` |
| `CORS_ORIGIN` | CORS allowed origin | `http://localhost:3000` |

## API Endpoints

### Health Check
- **GET** `/health` - Returns server health status

### Root
- **GET** `/` - Returns API information

## Development

### Code Quality

This project uses:
- **ESLint** for code linting
- **Prettier** for code formatting
- **Husky** for pre-commit hooks

The pre-commit hook automatically runs:
- ESLint with auto-fix
- Prettier formatting

### Testing

Tests are written using Jest and supertest. Run tests with:

```bash
npm test
```

## Production

### Build

```bash
npm run build
```

### Start

```bash
npm start
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## License

ISC 