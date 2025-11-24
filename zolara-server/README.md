<div align="center">
  <img src="../zolara-mobile/src/assets/images/brand/zolara.png" alt="Zolara Logo" width="200"/>
  
  # Zolara Server
  
  ### Backend API Server for Zolara Platform
  
  [![NestJS](https://img.shields.io/badge/NestJS-11.0.1-e0234e.svg)](https://nestjs.com/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.7.3-blue.svg)](https://www.typescriptlang.org/)
  [![Prisma](https://img.shields.io/badge/Prisma-6.19.0-2D3748.svg)](https://www.prisma.io/)
  [![Socket.IO](https://img.shields.io/badge/Socket.IO-4.8.1-010101.svg)](https://socket.io/)
  
  [🏠 Back to Main](../README.md)
  
</div>

---

## 👥 Team Members

- **Nguyễn Văn Minh**
- **Nguyễn Trung Nguyên**

---

## 📋 Overview

Zolara Server is a robust, scalable backend API built with NestJS that powers the Zolara communication platform. It provides RESTful APIs and WebSocket connections for real-time messaging, voice/video calls, user management, and AI-powered chatbot features.

---

## ✨ Features

- 🔐 **JWT Authentication** - Secure user authentication and authorization
- 💬 **Real-time Messaging** - WebSocket-based instant messaging with Socket.IO
- 📞 **Call Management** - Voice and video call signaling
- 👥 **User Management** - Complete user profile and settings management
- 🤖 **AI Chatbot** - Integrated Google Generative AI for intelligent conversations
- 👫 **Friend System** - Friend requests, acceptance, and management
- 👨‍👩‍👧 **Group Management** - Create, manage, and participate in group chats
- 📧 **Email Service** - SendGrid and Nodemailer integration
- 📱 **SMS Service** - Twilio SMS integration
- 📊 **Admin Dashboard API** - Analytics and user management endpoints
- 📁 **File Storage** - Supabase storage integration
- 🔄 **Event System** - Event-driven architecture with EventEmitter
- ⚡ **Redis Caching** - High-performance caching layer
- 📮 **Contact Management** - Phone contact synchronization

---

## 🛠️ Technology Stack

### Core Framework
- **NestJS** `11.0.1` - Progressive Node.js framework
- **TypeScript** `5.7.3` - Type-safe JavaScript
- **Node.js** - JavaScript runtime

### Database & ORM
- **Prisma** `6.19.0` - Next-generation ORM
- **PostgreSQL** - Primary database
- **Redis** `5.9.0` - Caching and session storage

### Real-time Communication
- **Socket.IO** `4.8.1` - WebSocket implementation
- **@nestjs/websockets** `11.1.8` - NestJS WebSocket support
- **@nestjs/platform-socket.io** `11.1.8` - Socket.IO platform adapter

### Authentication & Security
- **@nestjs/jwt** `11.0.1` - JWT token management
- **@nestjs/passport** `11.0.5` - Authentication strategies
- **passport-jwt** `4.0.1` - JWT passport strategy
- **bcrypt** `6.0.0` - Password hashing

### AI & Machine Learning
- **@ai-sdk/google** `2.0.31` - Google AI SDK
- **@google/generative-ai** `0.24.1` - Generative AI models
- **ai** `5.0.93` - AI utilities

### External Services
- **@supabase/supabase-js** `2.81.1` - Supabase client for storage
- **@sendgrid/mail** `8.1.6` - SendGrid email service
- **nodemailer** `7.0.10` - Email sending
- **twilio** `5.10.5` - SMS messaging
- **sharp** `0.34.5` - Image processing

### API Documentation
- **@nestjs/swagger** `11.2.1` - OpenAPI/Swagger documentation

### Utilities
- **axios** `1.13.2` - HTTP client
- **uuid** `13.0.0` - UUID generation
- **class-validator** `0.14.2` - DTO validation
- **class-transformer** `0.5.1` - Object transformation
- **cache-manager** `7.2.4` - Cache abstraction
- **rxjs** `7.8.1` - Reactive programming

### Development Tools
- **@nestjs/cli** `11.0.0` - NestJS CLI
- **jest** `30.0.0` - Testing framework
- **eslint** `9.18.0` - Code linting
- **prettier** `3.4.2` - Code formatting
- **husky** `9.1.7` - Git hooks
- **lint-staged** `16.2.6` - Lint staged files

---

## 📂 Project Structure

```
zolara-server/
├── prisma/
│   ├── schema.prisma          # Database schema
│   ├── seed.ts               # Database seeding
│   └── migrations/           # Database migrations
│
├── src/
│   ├── main.ts              # Application entry point
│   ├── app.module.ts        # Root module
│   │
│   ├── auth/                # Authentication module
│   │   ├── auth.controller.ts
│   │   ├── auth.service.ts
│   │   ├── auth.gateway.ts
│   │   ├── guards/          # Auth guards
│   │   └── dto/             # Data transfer objects
│   │
│   ├── user/                # User management
│   │   ├── user.controller.ts
│   │   ├── user.service.ts
│   │   └── dto/
│   │
│   ├── message/             # Messaging system
│   │   ├── message.controller.ts
│   │   ├── message.service.ts
│   │   ├── message.gateway.ts
│   │   ├── dtos/
│   │   └── interfaces/
│   │
│   ├── group/               # Group management
│   │   ├── group.controller.ts
│   │   ├── group.service.ts
│   │   ├── group.gateway.ts
│   │   └── dto/
│   │
│   ├── friend/              # Friend system
│   │   ├── friend.controller.ts
│   │   ├── friend.service.ts
│   │   ├── friend.gateway.ts
│   │   └── dto/
│   │
│   ├── agent/               # AI chatbot
│   │   ├── agent.controller.ts
│   │   ├── agent.service.ts
│   │   ├── agent.gateway.ts
│   │   ├── dto/
│   │   └── interfaces/
│   │
│   ├── dashboard/           # Admin dashboard
│   │   ├── dashboard.controller.ts
│   │   ├── dashboard.service.ts
│   │   └── dto/
│   │
│   ├── contact/             # Contact management
│   │   ├── contact.controller.ts
│   │   ├── contact.service.ts
│   │   └── dto/
│   │
│   ├── mail/                # Email service
│   │   ├── mail.service.ts
│   │   └── mail.module.ts
│   │
│   ├── cache/               # Redis caching
│   │   ├── cache.service.ts
│   │   └── cache.module.ts
│   │
│   ├── storage/             # File storage
│   │   └── storage.service.ts
│   │
│   ├── prisma/              # Prisma service
│   │   ├── prisma.service.ts
│   │   └── prisma-cleanup.service.ts
│   │
│   ├── qr-code/             # QR code generation
│   │   └── qr-code.cleanup.ts
│   │
│   ├── event/               # Event handling
│   │   ├── event.service.ts
│   │   └── event.module.ts
│   │
│   └── post/                # Post management
│       ├── post.controller.ts
│       ├── post.service.ts
│       └── dto/
│
├── test/                    # E2E tests
│   └── app.e2e-spec.ts
│
├── postman/                 # Postman collections
│   ├── Zolara API.postman_collection.json
│   └── Zolara - Group Management API Tests.postman_collection.json
│
├── docker-compose.yml       # Docker compose configuration
├── Dockerfile              # Docker image definition
└── railway.json            # Railway deployment config
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** 18.x or higher
- **npm** or **yarn** or **pnpm**
- **PostgreSQL** 14.x or higher
- **Redis** 6.x or higher

### Environment Variables

Create a `.env` file in the root directory:

```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/zolara"

# Redis
REDIS_HOST=localhost
REDIS_PORT=6379
REDIS_PASSWORD=

# JWT
JWT_SECRET=your-super-secret-jwt-key
JWT_EXPIRES_IN=7d

# Supabase
SUPABASE_URL=your-supabase-url
SUPABASE_KEY=your-supabase-key
SUPABASE_BUCKET=your-bucket-name

# SendGrid
SENDGRID_API_KEY=your-sendgrid-api-key
SENDGRID_FROM_EMAIL=noreply@zolara.com

# Twilio
TWILIO_ACCOUNT_SID=your-twilio-account-sid
TWILIO_AUTH_TOKEN=your-twilio-auth-token
TWILIO_PHONE_NUMBER=your-twilio-phone-number

# Google AI
GOOGLE_AI_API_KEY=your-google-ai-api-key

# Server
PORT=3000
NODE_ENV=development
```

### Installation

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Generate Prisma Client**
   ```bash
   npx prisma generate
   ```

3. **Run database migrations**
   ```bash
   npm run db:migrate
   ```

4. **Seed the database** (optional)
   ```bash
   npm run db:seed
   ```

### Running the Application

#### Development Mode
```bash
npm run dev
# or
npm run start:dev
```

#### Production Mode
```bash
npm run build
npm run start:prod
```

#### Debug Mode
```bash
npm run start:debug
```

The server will start at `http://localhost:3000`

---

## 📡 API Documentation

Once the server is running, access the Swagger API documentation at:

```
http://localhost:3000/api/docs
```

### Main API Endpoints

| Module | Endpoint | Description |
|--------|----------|-------------|
| **Auth** | `/api/auth/*` | Authentication & registration |
| **Users** | `/api/users/*` | User management |
| **Messages** | `/api/messages/*` | Message operations |
| **Groups** | `/api/groups/*` | Group management |
| **Friends** | `/api/friends/*` | Friend operations |
| **Agent** | `/api/agent/*` | AI chatbot |
| **Dashboard** | `/api/dashboard/*` | Admin analytics |
| **Contacts** | `/api/contacts/*` | Contact sync |
| **Posts** | `/api/posts/*` | Post management |

### WebSocket Events

The server supports real-time communication via Socket.IO:

- **Connection**: `ws://localhost:3000`
- **Events**: `message:new`, `message:read`, `user:status`, `call:*`, etc.

---

## 🧪 Testing

### Unit Tests
```bash
npm run test
```

### E2E Tests
```bash
npm run test:e2e
```

### Test Coverage
```bash
npm run test:cov
```

### Watch Mode
```bash
npm run test:watch
```

---

## 🗄️ Database Management

### Create Migration
```bash
npx prisma migrate dev --name migration_name
```

### Deploy Migrations
```bash
npm run db:migrate
```

### Seed Database
```bash
npm run db:seed
```

### Prisma Studio (Database GUI)
```bash
npx prisma studio
```

---

## 🐳 Docker Deployment

### Using Docker Compose

```bash
docker-compose up -d
```

This will start:
- PostgreSQL database
- Redis cache
- Zolara Server

### Build Docker Image

```bash
docker build -t zolara-server .
```

### Run Container

```bash
docker run -p 3000:3000 --env-file .env zolara-server
```

---

## 📊 Database Schema

The database schema is defined in `prisma/schema.prisma` with the following main models:

- **User** - User accounts and profiles
- **Message** - Chat messages
- **Group** - Group conversations
- **GroupMember** - Group membership
- **Friend** - Friend relationships
- **Call** - Call records
- **Post** - User posts
- **Contact** - Synced contacts
- **Agent** - AI chatbot configurations

---

## 🔧 Scripts Reference

| Script | Description |
|--------|-------------|
| `npm run build` | Build the application |
| `npm start` | Start production server |
| `npm run dev` | Start development server |
| `npm run start:debug` | Start in debug mode |
| `npm run lint` | Lint code |
| `npm run format` | Format code with Prettier |
| `npm test` | Run tests |
| `npm run test:e2e` | Run E2E tests |
| `npm run db:migrate` | Run database migrations |
| `npm run db:seed` | Seed database |

---

## 📄 License

This project is licensed under the MIT License.

---

## 🔗 Related Projects

- [Zolara Mobile](../zolara-mobile/README.md) - Mobile application
- [Zolara Admin](../zolara-admin/README.md) - Admin dashboard

---

<div align="center">
  
**Built with ❤️ by the Zolara Team**

[🏠 Back to Main](../README.md)

</div>
