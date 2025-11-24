<div align="center">
  <img src="../zolara-mobile/src/assets/images/brand/zolara.png" alt="Zolara Logo" width="200"/>
  
  # Zolara Admin
  
  ### Admin Dashboard for Zolara Platform
  
  [![React](https://img.shields.io/badge/React-19.2.0-61dafb.svg)](https://reactjs.org/)
  [![Vite](https://img.shields.io/badge/Vite-7.2.2-646cff.svg)](https://vitejs.dev/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.9.3-blue.svg)](https://www.typescriptlang.org/)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4.1.17-38bdf8.svg)](https://tailwindcss.com/)
  
  [🏠 Back to Main](../README.md)
  
</div>

---

## 👥 Team Members

- **Nguyễn Văn Minh**
- **Nguyễn Trung Nguyên**

---

## 📋 Overview

Zolara Admin is a powerful, responsive admin dashboard built with React and Vite. It provides comprehensive user management, analytics, and monitoring capabilities for the Zolara platform. The dashboard features real-time data visualization, user statistics, and administrative controls.

---

## ✨ Features

- 📊 **Real-time Analytics** - Live statistics and performance metrics
- 👥 **User Management** - Comprehensive user administration
- 📈 **Data Visualization** - Interactive charts and graphs
- 🔐 **Secure Authentication** - JWT-based admin authentication
- 🌙 **Dark Mode Support** - Toggle between light and dark themes
- 📱 **Responsive Design** - Works on desktop, tablet, and mobile
- 🔍 **Search & Filter** - Advanced user search and filtering
- 📋 **User Actions** - Block, unblock, and manage user accounts
- 📊 **Dashboard Overview** - Key metrics at a glance
- 📉 **User Statistics** - Detailed user activity analytics
- ⚡ **Fast Performance** - Optimized with Vite for lightning-fast builds
- 🎨 **Modern UI** - Clean and intuitive interface with Tailwind CSS

---

## 🛠️ Technology Stack

### Core Framework
- **React** `19.2.0` - UI library with latest features
- **Vite** `7.2.2` - Next-generation frontend build tool
- **TypeScript** `5.9.3` - Type-safe JavaScript
- **React DOM** `19.2.0` - React rendering

### Routing
- **React Router DOM** `7.9.6` - Declarative routing for React

### UI & Styling
- **Tailwind CSS** `4.1.17` - Utility-first CSS framework
- **@tailwindcss/vite** `4.1.17` - Vite plugin for Tailwind
- **tailwind-merge** `3.4.0` - Merge Tailwind classes
- **class-variance-authority** `0.7.1` - Variant utilities
- **clsx** `2.1.1` - Conditional classnames
- **Lucide React** `0.553.0` - Beautiful icon library
- **@radix-ui/react-icons** `1.3.2` - Radix UI icons

### Data Visualization
- **Chart.js** `4.5.1` - Powerful charting library
- **react-chartjs-2** `5.3.1` - React wrapper for Chart.js

### UI Components
- **react-loading-skeleton** `3.5.0` - Loading skeletons

### HTTP Client
- **Axios** `1.13.2` - Promise-based HTTP client

### Development Tools
- **@vitejs/plugin-react** `5.1.0` - Vite React plugin
- **ESLint** `9.39.1` - Code linting
- **@eslint/js** `9.39.1` - ESLint JavaScript configs
- **eslint-plugin-react-hooks** `5.2.0` - React Hooks linting
- **eslint-plugin-react-refresh** `0.4.24` - React Refresh linting
- **TypeScript ESLint** `8.46.3` - TypeScript linting
- **globals** `16.5.0` - Global variables

---

## 📂 Project Structure

```
zolara-admin/
├── public/
│   └── env-config.template.js   # Runtime env config template
│
├── src/
│   ├── main.tsx                 # Application entry point
│   ├── App.tsx                  # Root component
│   ├── index.css                # Global styles
│   │
│   ├── pages/                   # Page components
│   │   ├── Dashboard.tsx        # Main dashboard page
│   │   ├── Login.tsx            # Admin login page
│   │   └── NotFound.tsx         # 404 page
│   │
│   ├── components/              # Reusable components
│   │   ├── DashboardHeader.tsx  # Dashboard header
│   │   ├── DashboardSidebar.tsx # Sidebar navigation
│   │   ├── OverviewSection.tsx  # Overview section
│   │   ├── AnalyticsSection.tsx # Analytics section
│   │   ├── UserManagementSection.tsx # User management
│   │   ├── UserStatisticsSection.tsx # User statistics
│   │   │
│   │   └── ui/                  # UI components
│   │       ├── AnalyticsDashboard.tsx
│   │       ├── Button.tsx
│   │       ├── Card.tsx
│   │       ├── Charts.tsx
│   │       ├── ConfirmDialog.tsx
│   │       ├── Input.tsx
│   │       └── Skeleton.tsx
│   │
│   ├── contexts/                # React contexts
│   │   ├── AuthContext.tsx      # Auth context provider
│   │   ├── AuthContext.context.ts
│   │   └── AuthContext.types.ts
│   │
│   ├── hooks/                   # Custom hooks
│   │   ├── useAuth.ts           # Authentication hook
│   │   ├── useDashboard.ts      # Dashboard data hook
│   │   └── useUserStatistics.ts # User statistics hook
│   │
│   ├── services/                # API services
│   │   └── api.ts               # API client
│   │
│   ├── lib/                     # Utilities
│   │   ├── config.ts            # App configuration
│   │   └── utils.ts             # Utility functions
│   │
│   ├── types/                   # TypeScript types
│   │   └── auth.types.ts        # Auth types
│   │
│   └── assets/                  # Static assets
│       └── ...
│
├── index.html                   # HTML entry point
├── vite.config.ts              # Vite configuration
├── tailwind.config.js          # Tailwind CSS config
├── tsconfig.json               # TypeScript config
├── tsconfig.app.json           # App TypeScript config
├── tsconfig.node.json          # Node TypeScript config
├── eslint.config.js            # ESLint configuration
├── package.json                # Dependencies
├── Dockerfile                  # Docker image
├── nginx.conf                  # Nginx configuration
├── docker-entrypoint.sh        # Docker entrypoint
└── railway.json                # Railway deployment config
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** 18.x or higher
- **npm** or **yarn** or **pnpm**

### Environment Variables

Create a `.env` file in the root directory:

```env
VITE_API_URL=http://localhost:3000
```

For production, the environment variables are injected at runtime via `env-config.js`.

### Installation

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Start development server**
   ```bash
   npm run dev
   ```

The app will be available at `http://localhost:5173`

---

## 🎯 Features Overview

### Dashboard Overview Section
- **Total Users** - Count of all registered users
- **Active Users** - Currently active users
- **Blocked Users** - Number of blocked accounts
- **New Users** - Recent registrations
- **Quick Actions** - Common admin tasks

### Analytics Section
- **User Growth Chart** - Visual representation of user growth over time
- **Activity Metrics** - User engagement statistics
- **Message Statistics** - Messaging activity data
- **Call Statistics** - Voice/video call analytics
- **Real-time Updates** - Live data refresh

### User Management Section
- **User List** - Comprehensive table of all users
- **Search & Filter** - Find users quickly
- **User Details** - View complete user profiles
- **User Actions**:
  - Block/Unblock users
  - View user activity
  - Manage permissions
  - Reset passwords (future feature)
- **Pagination** - Handle large user lists efficiently
- **Sorting** - Sort by various criteria

### User Statistics Section
- **Demographic Data** - User distribution by age, location, etc.
- **Activity Patterns** - When users are most active
- **Feature Usage** - Which features are most popular
- **Retention Metrics** - User retention analysis
- **Interactive Charts** - Drill down into data

---

## 📊 Dashboard Components

### Overview Cards
Display key metrics with icons and trend indicators:
```tsx
- Total Users with growth percentage
- Active Sessions
- Message Volume
- System Status
```

### Charts & Graphs
Powered by Chart.js:
- **Line Charts** - User growth over time
- **Bar Charts** - Daily/weekly/monthly comparisons
- **Pie Charts** - User distribution
- **Area Charts** - Cumulative statistics

### Data Tables
Feature-rich user management tables:
- Search functionality
- Column sorting
- Pagination
- Row actions (block, view, edit)
- Bulk operations
- Export capabilities

---

## 🎨 Styling & Theming

### Tailwind CSS Configuration

The app uses Tailwind CSS 4.1.17 with custom configuration:

```javascript
// tailwind.config.js
export default {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {
      colors: {
        // Custom color palette
      },
    },
  },
  plugins: [],
}
```

### Component Variants

Using `class-variance-authority` for component variants:

```tsx
const buttonVariants = cva(
  "inline-flex items-center justify-center rounded-md",
  {
    variants: {
      variant: {
        default: "bg-primary text-white",
        outline: "border border-gray-300",
      },
      size: {
        sm: "h-9 px-3",
        lg: "h-11 px-8",
      },
    },
  }
)
```

---

## 🔐 Authentication

### Admin Login
- Email and password authentication
- JWT token storage
- Auto-refresh tokens
- Protected routes
- Session management

### Auth Context

```tsx
const { login, logout, isAuthenticated, user } = useAuth();
```

---

## 📡 API Integration

### API Client Configuration

```typescript
// services/api.ts
import axios from 'axios';

const api = axios.create({
  baseURL: import.meta.env.VITE_API_URL,
  headers: {
    'Content-Type': 'application/json',
  },
});

// Request interceptor for auth token
api.interceptors.request.use((config) => {
  const token = localStorage.getItem('token');
  if (token) {
    config.headers.Authorization = `Bearer ${token}`;
  }
  return config;
});
```

### API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/login` | POST | Admin login |
| `/api/dashboard/stats` | GET | Dashboard statistics |
| `/api/dashboard/users` | GET | User list |
| `/api/dashboard/analytics` | GET | Analytics data |
| `/api/dashboard/user/:id/block` | POST | Block user |
| `/api/dashboard/user/:id/unblock` | POST | Unblock user |

---

## 🧪 Development

### Running in Development Mode

```bash
npm run dev
```

### Building for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

### Linting

```bash
npm run lint
```

---

## 🐳 Docker Deployment

### Using Docker

```bash
docker build -t zolara-admin .
docker run -p 80:80 zolara-admin
```

### Docker Compose

```yaml
version: '3.8'
services:
  admin:
    build: .
    ports:
      - "80:80"
    environment:
      - API_URL=https://api.zolara.com
```

### Nginx Configuration

The app includes production-ready Nginx configuration with:
- SPA routing support
- Gzip compression
- Security headers
- API proxy configuration (optional)

---

## 🚀 Deployment

### Railway Deployment

The project includes `railway.json` configuration:

```json
{
  "build": {
    "builder": "DOCKERFILE",
    "dockerfilePath": "Dockerfile"
  },
  "deploy": {
    "startCommand": "nginx -g 'daemon off;'",
    "healthcheckPath": "/",
    "healthcheckTimeout": 100
  }
}
```

### Environment Variables at Runtime

The app uses a runtime configuration system via `env-config.js`:

```javascript
window._env_ = {
  API_URL: "${API_URL}",
};
```

This is replaced by the actual values at container startup via `docker-entrypoint.sh`.

---

## 📊 Dashboard Metrics

### Real-time Statistics
- User count updates
- Active sessions
- System health
- API response times

### Historical Data
- User growth trends
- Activity patterns
- Feature usage
- Performance metrics

---

## 🔧 Configuration Files

### Vite Configuration (`vite.config.ts`)

```typescript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

export default defineConfig({
  plugins: [react()],
  server: {
    port: 5173,
    host: true,
  },
})
```

### TypeScript Configuration

Three configuration files for different contexts:
- `tsconfig.json` - Base configuration
- `tsconfig.app.json` - App-specific settings
- `tsconfig.node.json` - Node environment settings

---

## 🎨 UI Components

### Button Component
```tsx
<Button variant="default" size="lg">
  Click Me
</Button>
```

### Card Component
```tsx
<Card>
  <CardHeader>Title</CardHeader>
  <CardContent>Content here</CardContent>
</Card>
```

### Charts
```tsx
<LineChart data={userData} />
<BarChart data={activityData} />
<PieChart data={distributionData} />
```

---

## 🔧 Scripts Reference

| Script | Description |
|--------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Lint code |

---

## 📱 Responsive Design

The dashboard is fully responsive with breakpoints for:
- **Mobile** (< 640px)
- **Tablet** (640px - 1024px)
- **Desktop** (> 1024px)

Sidebar converts to mobile menu on small screens.

---

## 🔍 Advanced Features

### Search Functionality
- Real-time user search
- Multi-field search (name, email, phone)
- Debounced input for performance

### Filtering
- Filter by user status
- Filter by registration date
- Filter by user role
- Combine multiple filters

### Sorting
- Sort by username
- Sort by registration date
- Sort by activity level
- Ascending/descending order

---

## 🐛 Troubleshooting

### Common Issues

**Port already in use:**
```bash
# Change port in vite.config.ts or use:
npm run dev -- --port 3001
```

**API connection issues:**
- Check `.env` file has correct API URL
- Verify CORS settings on backend
- Check network/firewall settings

**Build errors:**
```bash
rm -rf node_modules dist
npm install
npm run build
```

---

## 📄 License

This project is licensed under the MIT License.

---

## 🔗 Related Projects

- [Zolara Server](../zolara-server/README.md) - Backend API server
- [Zolara Mobile](../zolara-mobile/README.md) - Mobile application

---

<div align="center">
  
**Built with ❤️ by the Zolara Team**

[🏠 Back to Main](../README.md)

</div>
