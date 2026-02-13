# Cratos UI

<div align="center">

**A modern, responsive web interface for the Cratos task scheduler**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![React](https://img.shields.io/badge/React-18.2+-61dafb.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.2+-3178c6.svg)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.0+-646cff.svg)](https://vitejs.dev/)

[Features](#-features) • [Quick Start](#-quick-start) • [Documentation](#-documentation) • [Contributing](#-contributing)

</div>

---

## 📖 Overview

Cratos UI is a beautiful, modern web interface for managing and monitoring tasks in the Cratos scheduler. Built with React, TypeScript, and Tailwind CSS, it provides an intuitive way to create, schedule, and monitor background jobs.

## ✨ Features

- 📋 **Task Management**
  - View all scheduled tasks with pagination
  - Create new tasks with intuitive forms
  - Edit and delete existing tasks
  - Filter tasks by status
  - Search tasks by name or ID

- 📊 **Dashboard & Metrics**
  - Real-time task statistics
  - Execution history charts
  - Service health monitoring
  - Recent executions table

- ⏱️ **Scheduling Options**
  - One-off tasks (run once)
  - Cron expressions with human-readable descriptions
  - Interval-based scheduling
  - Timezone support

- 🔄 **Task Controls**
  - Pause/resume recurring tasks
  - Cancel scheduled tasks
  - Retry failed tasks
  - View execution history

- 🎨 **Modern UI/UX**
  - Clean, responsive design
  - Dark mode support
  - Real-time updates
  - Auto-refresh toggle
  - Overdue task indicators

- 🔐 **Authentication**
  - Secure login system
  - API key management
  - Session-based authentication

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm
- Cratos backend running (see [Cratos](https://github.com/Ghiles1010/Cratos))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ghiles1010/Cratos-UI.git
   cd Cratos-UI
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   ```bash
   # Create .env file (optional, defaults to http://localhost:8001)
   echo "VITE_SCHEDULER_API_URL=http://localhost:8001" > .env
   ```

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Open in browser**
   - Navigate to http://localhost:3001
   - Login with your Cratos credentials

## 🐳 Docker Deployment

### Using Docker Compose

```bash
# Build and start
task build
task up

# Or using docker-compose directly
docker compose build
docker compose up -d
```

The UI will be available at `http://localhost:3001`.

### Environment Configuration

Set the Cratos API URL:

```bash
export VITE_SCHEDULER_API_URL=http://your-cratos-api:8001
docker compose build
docker compose up -d
```

## 📚 Documentation

### Available Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
npm run lint     # Run ESLint
```

### Taskfile Commands

```bash
task dev         # Start development server
task build       # Build Docker image
task up          # Start Docker container
task down        # Stop Docker container
task restart     # Restart container
task logs        # View container logs
task clean       # Remove containers and images
```

### Project Structure

```
cratos-ui/
├── src/
│   ├── components/    # Reusable UI components
│   │   ├── tasks/    # Task-related components
│   │   ├── metrics/  # Metrics and charts
│   │   └── ui/       # Base UI components
│   ├── pages/        # Page components
│   ├── hooks/        # React hooks
│   ├── contexts/     # React contexts
│   ├── lib/          # Utilities and API client
│   └── main.tsx      # Entry point
├── public/
├── Dockerfile
├── docker-compose.yml
└── package.json
```

## 🎨 UI Features

### Task Table
- Sortable columns
- Status badges with color coding
- Overdue indicators (red blinking dot)
- Quick actions (view, edit, delete)
- Pagination support

### Task Creation
- Step-by-step form
- Cron expression builder
- Timezone selector
- Retry policy configuration
- Payload editor (JSON)

### Metrics Dashboard
- Task count by status
- Execution success rate
- Average execution time
- Recent execution timeline

## 🔧 Configuration

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `VITE_SCHEDULER_API_URL` | Cratos backend API URL | `http://localhost:8001` |

### API Authentication

The UI uses session-based authentication for login. API requests are made with cookies automatically.

For programmatic access, use API key authentication:
```bash
Authorization: Api-Key YOUR_API_KEY
```

## 🧪 Development

### Tech Stack

- **React 18** - UI library
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **React Query** - Data fetching and caching
- **React Router** - Routing
- **shadcn/ui** - UI components
- **Recharts** - Data visualization

### Development Workflow

1. **Start development server**
   ```bash
   npm run dev
   ```

2. **Make changes**
   - Edit files in `src/`
   - Changes hot-reload automatically

3. **Build for production**
   ```bash
   npm run build
   ```

4. **Preview production build**
   ```bash
   npm run preview
   ```

### Code Style

- Follow TypeScript best practices
- Use functional components with hooks
- Follow React naming conventions
- Use Tailwind CSS for styling

## 🌐 Related Projects

- **[Cratos](https://github.com/Ghiles1010/Cratos)** - The backend task scheduler service

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines

- Follow TypeScript and React best practices
- Write clean, maintainable code
- Update documentation as needed
- Test your changes thoroughly
- Ensure the build passes before submitting

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [React](https://reactjs.org/) and [Vite](https://vitejs.dev/)
- UI components from [shadcn/ui](https://ui.shadcn.com/)
- Styling with [Tailwind CSS](https://tailwindcss.com/)
- Icons from [Lucide React](https://lucide.dev/)

## 📧 Support

- **Issues**: [GitHub Issues](https://github.com/Ghiles1010/Cratos-UI/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Ghiles1010/Cratos-UI/discussions)

---

<div align="center">

Made with ❤️ by the Cratos team

[⭐ Star us on GitHub](https://github.com/Ghiles1010/Cratos-UI) • [📖 Documentation](#-documentation) • [🐛 Report Bug](https://github.com/Ghiles1010/Cratos-UI/issues)

</div>
