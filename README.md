# Query Master

A lightweight client for working with REST APIs, created as an alternative to Postman. The project was developed by a team of 3 people using Firebase for authentication.

## 📋 Project Description

Query Master is a full-featured web application that allows users to:
- Send HTTP requests (GET, POST, PUT, DELETE, PATCH, etc.)
- Edit request headers and body
- View server responses
- Generate request code in various programming languages
- Manage variables for reuse in requests
- Save the history of executed requests
- Work with the app in English or German

## 🚀 Technology Stack

- **Frontend Framework**: Next.js 15.2.3 with Turbopack
- **UI Libraries**: React 19, TailwindCSS 4, React Icons
- **State Management**: Redux Toolkit
- **Authentication**: Firebase 11.5.0
- **Validation**: Zod, React Hook Form
- **Internationalization**: next-intl
- **Styling**: Tailwind CSS, PostCSS, SASS
- **Testing**: Jest, React Testing Library
- **Linting**: ESLint, Prettier
- **Git Hooks**: Husky

## 📦 Installation and Setup

### Prerequisites
- Node.js (version 18+)
- npm or yarn

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Barvinko/rest-client-app.git
   cd rest-client-app
   ```

2. **Switch to the development branch** (if required)
   ```bash
   git checkout develop
   ```

3. **Install dependencies**
   ```bash
   npm install
   ```

4. **Set up environment variables**
   - Create a `.env.local` file in the root folder
   - Copy the contents from the `envsample` file into `.env.local`
   - Fill in the necessary environment variables (Firebase configuration, etc.)

5. **Run the app in development mode**
   ```bash
   npm run dev
   ```
   The app will be available at: `http://localhost:3000`

## 📖 Available Commands

```bash
# Run in development mode with Turbopack
npm run dev

# Build the app for production
npm run build

# Start the production version
npm start

# Check code with ESLint
npm run lint

# Format code with Prettier
npm run format:fix

# Run Jest tests
npm run test

# Generate test coverage report
npm run coverage

# Clean coverage folder
npm run clean-coverage

# Install Git hooks (Husky)
npm run prepare
```

## ✨ Key Features

### 🔐 Authentication and Authorization
- New user registration
- Login via Firebase
- Protected routes (accessible only to authenticated users)
- Secure storage of authentication tokens

### 🌐 REST Client
- Selection of HTTP methods (GET, POST, PUT, DELETE, PATCH, HEAD, OPTIONS, etc.)
- API URL input
- Request headers editor
- Request body editor with JSON and text support
- Server response viewer with status information

### 💻 Code Generation
Automatic generation of request code in the following languages:
- cURL
- JavaScript (Fetch API)
- JavaScript (XHR)
- Node.js
- Python
- Java
- C#
- Go

### 📝 Request History
- Automatic saving of executed requests
- Quick access to previously executed requests
- Restoration of all request parameters upon clicking on a history item

### 🔤 Variables
- Creation and management of variables
- Use of variables in URL, headers, and request body
- Syntax: `{{variableName}}`
- Automatic substitution of values during request execution

### 🌍 Internationalization
- Support for Russian and English languages
- Easy language switching via the header control element

## 🏗️ Project Structure

```
rest-client-app/
├── src/                    # App source code
├── public/                 # Static files
├── __mocks__/              # Mock data for tests
├── messages/               # Translation files (i18n)
├── tests/                  # App tests
├── jest.config.ts          # Jest configuration
├── next.config.ts          # Next.js configuration
├── tsconfig.json           # TypeScript configuration
├── tailwind.config.ts      # Tailwind CSS configuration
├── eslint.config.mjs       # ESLint configuration
├── .prettierrc             # Prettier configuration
├── .husky/                 # Git hooks
├── package.json            # Dependencies and scripts
├── requirements.md         # Project requirements
└── README.md               # This file
```

## 🧪 Testing

The project includes a full set of tests with at least 80% coverage:

```bash
# Run all tests
npm run test

# Run tests with coverage report
npm run coverage
```

## 🔍 Code Quality

- **ESLint**: Code checking for compliance with standards
- **Prettier**: Automatic code formatting
- **Husky**: Git hooks for automatic code checking before commits
  - Pre-commit: run `npm run lint`
  - Pre-push: run `npm run test`

## 👥 Development Team

* **Irakli Gogicha:** [@gogicha007](https://github.com/gogicha007)
* **Vladyslav Barvinko:** [@Barvinko](https://github.com/Barvinko)
* **Oleg Polovinko:** [@sheritsh](https://github.com/sheritsh)

## 📞 Support

If you encounter issues:
1. Check that all environment variables are correctly set in `.env.local`
2. Ensure all dependencies are installed: `npm install`
3. Clear the cache: `npm run clean-coverage`
4. Restart the development server: `npm run dev`