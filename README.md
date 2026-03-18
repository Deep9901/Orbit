
---

# Orbit
### Enterprise-Grade Real-Time Video & Study Platform

A high-performance, cross-platform mobile application built with Expo SDK 55. Featuring a native Liquid Glass UI, serverless API routes, and production-ready real-time infrastructure.

---

## Key Features

* **Native Liquid Glass UI:** High-fidelity aesthetic using expo-glass-effect and NativeWind v4.
* **Pro Video Calling:** 1-on-1 video calls with ringing UI, powered by Stream Video SDK.
* **Rich Messaging:** Real-time chat with support for images, videos, GIFs, and threaded replies.
* **Seamless Auth:** Multi-provider social login (Google, Apple, GitHub) integrated via Clerk.
* **Edge API Routes:** Built-in serverless functions (+api.ts) for user syncing and token generation.
* **Reliable Architecture:** Full TypeScript support, ESLint configuration, and Sentry error monitoring.

---

## Project Structure

```text
├── 📁 .vscode              # Editor settings & snippets
├── 📁 assets               # Static assets (images, fonts, icons)
├── 📁 src                  # Main source code
│   ├── 📁 app              # Expo Router (Tabs, Auth, API, Call logic)
│   ├── 📁 components       # Reusable UI (VideoProvider, ChatWrapper)
│   ├── 📁 contexts         # Global State (AppProvider)
│   ├── 📁 hooks            # Custom Logic (Auth & Stream hooks)
│   └── 📁 lib              # Utilities & Theme definitions
├── 📄 app.json             # Expo configuration
├── 📄 eas.json             # Expo Application Services (Build/Submit)
├── 📄 metro.config.js      # Metro Bundler configuration
├── 📄 tailwind.config.js   # NativeWind / Tailwind CSS setup
└── 📄 tsconfig.json        # TypeScript configuration
```

---

## Quick Start

### 1. Clone & Install
```bash
npm install
```

### 2. Setup Environment Variables
Create a .env file in the root directory:
```env
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
EXPO_PUBLIC_STREAM_API_KEY=your_stream_key
# Required for serverless API routes (+api.ts)
STREAM_SECRET_KEY=your_stream_secret
```

### 3. Run the App
```bash
npx expo start
```
* Press i for iOS Simulator.
* Press a for Android Emulator.
* Use the Expo Go app to test on physical devices.

---

## Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Framework** | Expo SDK 55 (React Native) |
| **Styling** | NativeWind v4 (Tailwind CSS) |
| **Auth** | Clerk Expo |
| **Real-Time** | Stream Video & Chat SDK |
| **Navigation** | Expo Router (File-based) |
| **Monitoring** | Sentry for React Native |

---
