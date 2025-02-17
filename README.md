<div align="center">
  <img src="assets/wallzen-logo.png" alt="Wallzen Logo" width="200" height="200" style="border-radius: 20px;">

  <h1>🖼️ Wallzen</h1>
  <p>A modern, high-performance wallpaper platform with AI-powered search and organization</p>

  <p>
    <a href="#overview">Overview</a> •
    <a href="#architecture">Architecture</a> •
    <a href="#getting-started">Getting Started</a> •
    <a href="#features">Features</a> •
    <a href="#development">Development</a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version">
    <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">
    <img src="https://img.shields.io/badge/typescript-%5E5.0.0-blue.svg" alt="TypeScript">
    <img src="https://img.shields.io/badge/node-%5E18.0.0-green.svg" alt="Node.js">
  </p>
</div>

---

## 📖 Overview

Wallzen is a comprehensive wallpaper management platform that combines a high-performance backend API with a modern, responsive frontend interface. The project is structured as a monorepo using Git submodules for better code organization and maintenance.

### Repository Structure
```
wallzen/
├── frontend/          # Next.js frontend application
├── backend/          # Express.js backend API
├── docs/            # Project documentation
└── scripts/         # Development and deployment scripts
```

## 🏗️ Architecture

```mermaid
graph TD
    A[Client] --> B[Frontend - Next.js]
    B --> C[Backend API - Express.js]
    C --> D[PostgreSQL Database]
    C --> E[File Storage]
    C --> F[Image Processing]
```

## ✨ Features

### Frontend Features
- 🎨 Modern, responsive UI built with Next.js 13
- 📱 Mobile-first design approach
- 🔍 Real-time search with debouncing
- 🖼️ Dynamic image grid with lazy loading
- 💡 Advanced filtering and sorting options
- ❤️ User favorites management
- 🔄 Infinite scroll support

### Backend Features
- 🚀 High-performance Express.js API
- 📊 PostgreSQL with Prisma ORM
- 🔒 Rate limiting and security features
- 📸 Image processing and optimization
- 🏷️ Automatic tag generation
- 📈 Analytics and statistics tracking

## 🚀 Getting Started

1. **Clone the repository with submodules**
```bash
git clone --recursive https://github.com/justkelvin/wallzen.git
cd wallzen
```

2. **Initialize and update submodules**
```bash
git submodule init
git submodule update
```

3. **Set up environment variables**
```bash
# Root directory
cp .env.example .env

# Frontend
cd frontend
cp .env.example .env.local

# Backend
cd ../backend
cp .env.example .env
```

4. **Install dependencies**
```bash
# Install root dependencies
npm install

# Install frontend dependencies
cd frontend
npm install

# Install backend dependencies
cd ../backend
npm install
```

5. **Start development servers**
```bash
# Start both frontend and backend
npm run dev
```

## 🔧 Development

### Prerequisites
- Node.js >= 18.0.0
- PostgreSQL >= 14
- npm >= 8.0.0

### Available Scripts
```bash
# Start development servers
npm run dev

# Build for production
npm run build

# Run tests
npm run test

# Lint code
npm run lint

# Format code
npm run format
```

### Environment Variables

```env
# Root .env
NODE_ENV=development
PROJECT_NAME=wallzen

# Frontend specific
NEXT_PUBLIC_API_URL=http://localhost:3001/api
NEXT_PUBLIC_SITE_URL=http://localhost:3000

# Backend specific
PORT=3001
DATABASE_URL="postgresql://user:password@localhost:5432/wallzen"
```

## 📚 Documentation

- [Frontend Documentation](./frontend/README.md)
- [Backend Documentation](./backend/README.md)
- [API Documentation](./docs/api.md)
- [Development Guide](./docs/development.md)
- [Deployment Guide](./docs/deployment.md)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📈 Project Status

- **Last Updated**: 2025-02-17 14:24:52 UTC
- **Maintained by**: [@justkelvin](https://github.com/justkelvin)
- **Status**: Active Development

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) for the frontend framework
- [Express.js](https://expressjs.com/) for the backend API
- [Prisma](https://www.prisma.io/) for database ORM
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [TypeScript](https://www.typescriptlang.org/) for type safety

---

<div align="center">
  <p>Built with ❤️ by <a href="https://github.com/justkelvin">justkelvin</a></p>
  <p>
    <a href="https://github.com/justkelvin">GitHub</a> •
    <a href="https://twitter.com/alias_notfound">Twitter</a>
  </p>

  <br>
  
  <p>
    <sub>
      Started on 2025 • Updated on 2025-02-17
    </sub>
  </p>
</div>