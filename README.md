
Built by https://www.blackbox.ai

---

# Fusion Starter

## Project Overview
Fusion Starter is a production-ready full-stack React application template, integrating an Express server with a modern tech stack featuring React Router 6 SPA mode, TypeScript, Vitest, Zod, and modern tooling. This template is designed to streamline development with an efficient routing system, styled components using TailwindCSS, and a robust API.

## Installation
To get started with the Fusion Starter, follow these steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/user/fusion-starter.git
   cd fusion-starter
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

## Usage
To run the application in development mode, you can use the following command:

```bash
npm run dev
```

This command starts the development servers for both the client and the server at port **8080**.

For a production build, execute:

```bash
npm run build
```

To start the production server, use:

```bash
npm run start
```

## Features
- **Single Page Application (SPA)**: Utilize React Router for dynamic routing.
- **Custom UI Components**: Rapidly build interfaces with a pre-built UI component library integrated with TailwindCSS.
- **Express Integration**: Seamlessly combine an Express backend with a Vite development server.
- **Hot Reloading**: Automatically refresh your app on code changes for both frontend and backend.
- **Type Safety**: Benefit from TypeScript across client-side, server-side, and shared code.
- **Testing Suite**: Leverage Vitest for running tests and checking code quality.
- **Shared Types**: Easily import shared TypeScript types between client and server.

## Dependencies
The project relies on the following dependencies (found in `package.json`):

- **Backend**:
  - `express`: ^4.18.2
  - `zod`: ^3.23.8

- **Development**:
  - `@hookform/resolvers`: ^3.9.0
  - All Radix UI Components: Various editions
  - `typescript`: ^5.5.3
  - `vite`: ^6.2.2
  - `vitest`: ^3.1.4

*For a complete list of dependencies, refer to the `package.json` file.*

## Project Structure
The folder structure is organized as follows:

```
client/                   # React SPA frontend
├── pages/                # Route components (Index.tsx = home)
├── components/ui/        # Pre-built UI component library
├── App.tsx               # App entry point and SPA routing setup
└── global.css            # TailwindCSS 3 theming and global styles

server/                   # Express API backend
├── index.ts              # Main server setup (express config + routes)
└── routes/               # API handlers

shared/                   # Types used by both client & server
└── api.ts                # Example of how to share API interfaces
```

## Development Commands
You can perform the following commands during development:

```bash
npm run dev        # Start dev server (client + server)
npm run build      # Production build
npm run start      # Start production server
npm run typecheck  # TypeScript validation
npm test           # Run Vitest tests
```

## Adding Features
### New API Route
To add a new API route:
1. Optionally, create a shared interface in `shared/api.ts`.
2. Implement the route in `server/routes/my-route.ts`.
3. Register the route in `server/index.ts`.
4. Use the route in React components with type safety.

### New Page Route
To add a new page route:
1. Create a component in `client/pages/MyPage.tsx`.
2. Add the route in `client/App.tsx`.

## Production Deployment
The application can be deployed using various methods:
- **Standard**: Run the commands `npm run build` followed by `npm start`.
- **Docker**: A Dockerfile is included for container-based deployment.
- **Binary**: Create self-contained executables for Linux, macOS, and Windows.

## Architecture Notes
- A single-port development setup combining Vite and Express.
- TypeScript is employed throughout the codebase.
- Hot reloading function for quick development cycles.
- Comprehensive deployment options for production-ready applications.
- Pre-built UI components and type-safe API communication.

---
Enjoy building your application with Fusion Starter!