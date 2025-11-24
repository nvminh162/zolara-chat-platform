
<div align="center">
  <img src="./zolara-mobile/src/assets/images/brand/zolara.png" alt="Zolara Logo" width="200"/>
  
  # Zolara
  
  ### Modern Real-Time Communication Platform
  
  *Empowering real-time communication through modern technology*
  
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
  [![React](https://img.shields.io/badge/React-19.2.0-61dafb.svg)](https://reactjs.org/)
  [![React Native](https://img.shields.io/badge/React%20Native-0.81.5-61dafb.svg)](https://reactnative.dev/)
  [![NestJS](https://img.shields.io/badge/NestJS-11.0.1-e0234e.svg)](https://nestjs.com/)
  
</div>

---

## 👥 Team Members

- **Nguyễn Văn Minh**
- **Nguyễn Trung Nguyên**

---

## 📱 Project Overview

Zolara is a comprehensive real-time communication platform consisting of three main components:

### 🔗 Project Components

| Component | Description | Documentation |
|-----------|-------------|---------------|
| **[Zolara Server](./zolara-server/README.md)** | Backend API server built with NestJS | [📖 Read More](./zolara-server/README.md) |
| **[Zolara Mobile](./zolara-mobile/README.md)** | Cross-platform mobile app with Expo & React Native | [📖 Read More](./zolara-mobile/README.md) |
| **[Zolara Admin](./zolara-admin/README.md)** | Admin dashboard for managing users and analytics | [📖 Read More](./zolara-admin/README.md) |

---

## ✨ Key Features

- 💬 **Real-time Messaging** - Instant chat with Socket.IO
- 📞 **Voice & Video Calls** - WebRTC-powered communication
- 👥 **Group Management** - Create and manage group conversations
- 🤖 **AI Chatbot** - Integrated AI assistant powered by Google Generative AI
- 📊 **Admin Dashboard** - Comprehensive user and analytics management
- 🔐 **Secure Authentication** - JWT-based auth with secure storage
- 📱 **Cross-Platform** - iOS, Android, and Web support
- 🌙 **Dark Mode** - Full theme customization
- 📸 **Media Sharing** - Images, videos, documents, and voice messages
- 🔔 **Push Notifications** - Real-time notification system

---

## 🛠️ Technology Stack

### Backend (Server)
- **Framework:** NestJS 11.0.1
- **Language:** TypeScript 5.7.3
- **Database:** PostgreSQL with Prisma ORM
- **Cache:** Redis
- **Real-time:** Socket.IO
- **AI:** Google Generative AI
- **Storage:** Supabase
- **Email:** SendGrid, Nodemailer
- **SMS:** Twilio

### Mobile App
- **Framework:** Expo 54.0.25 & React Native 0.81.5
- **Language:** TypeScript 5.9.2
- **Navigation:** Expo Router 6.0.15
- **UI Library:** GlueStack UI, NativeWind
- **State Management:** Zustand
- **Real-time:** Socket.IO Client
- **Media:** Expo AV, Camera, Image Picker
- **Calls:** React Native WebRTC

### Admin Dashboard
- **Framework:** React 19.2.0 & Vite 7.2.2
- **Language:** TypeScript 5.9.3
- **Routing:** React Router DOM 7.9.6
- **UI:** Tailwind CSS 4.1.17
- **Charts:** Chart.js & React-ChartJS-2
- **Icons:** Lucide React

---

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm/pnpm/yarn
- PostgreSQL database
- Redis server
- Expo CLI (for mobile development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/NguyenNguyen0/zolara.git
   cd zolara
   ```

2. **Setup Server**
   ```bash
   cd zolara-server
   npm install
   cp .env.example .env
   # Configure your .env file
   npm run db:migrate
   npm run db:seed
   npm run dev
   ```

3. **Setup Mobile App**
   ```bash
   cd zolara-mobile
   npm install
   cp .env.example .env
   # Configure your .env file
   npm start
   ```

4. **Setup Admin Dashboard**
   ```bash
   cd zolara-admin
   npm install
   cp .env.example .env
   # Configure your .env file
   npm run dev
   ```

---

## 📂 Project Structure

```
zolara/
├── zolara-server/          # Backend API (NestJS)
│   ├── src/
│   │   ├── auth/          # Authentication module
│   │   ├── user/          # User management
│   │   ├── message/       # Messaging system
│   │   ├── group/         # Group management
│   │   ├── agent/         # AI chatbot
│   │   └── ...
│   └── prisma/            # Database schema & migrations
│
├── zolara-mobile/         # Mobile App (Expo/React Native)
│   ├── app/              # Expo Router screens
│   │   ├── (auth)/       # Authentication flows
│   │   ├── (tabs)/       # Main tab navigation
│   │   └── (user)/       # User-specific screens
│   └── src/
│       ├── components/   # Reusable components
│       ├── services/     # API services
│       ├── store/        # State management
│       └── ...
│
└── zolara-admin/         # Admin Dashboard (React/Vite)
    └── src/
        ├── components/   # UI components
        ├── pages/        # Page components
        ├── services/     # API services
        └── ...
```

---

## 📄 License

This project is licensed under the MIT License.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

---

## 📞 Contact

For any questions or support, please contact the development team.

---

<div align="center">
  
**Built with ❤️ by the Zolara Team**

</div>
