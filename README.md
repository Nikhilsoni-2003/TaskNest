# TaskNest 🪺

_A modern and responsive task manager built with Next.js, designed to keep your life organized and productive._

[![Next.js](https://img.shields.io/badge/Next.js-13-black?style=flat&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat&logo=typescript)](https://www.typescriptlang.org/)
[![Redux](https://img.shields.io/badge/Redux-Toolkit-764abc?style=flat&logo=redux)](https://redux-toolkit.js.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3-38BDF8?style=flat&logo=tailwindcss)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## ✨ Overview
**TaskNest** is a modern, responsive web application built with **Next.js** and **TypeScript**.  
It helps you organize tasks efficiently with smart reminders, weather insights, and a customizable UI featuring dark/light themes.

---

## 🚀 Features

### 📋 Task Management
- Add, delete, and mark tasks as complete.
- Filter tasks by **Today**, **Upcoming**, or **Important**.
- Search tasks by title, location, or reminder time.

### 🔔 Smart Reminders
- Set reminders with **audio alerts** and **browser notifications**.
- Reminders auto-dismiss when tasks are completed or expired.

### 🌦 Weather Integration
- Real-time weather for outdoor tasks via OpenWeatherMap API.
- Visual icons (☀️, 🌧️, ⛅) for quick reference.

### 🎨 User Interface
- Responsive design with collapsible sidebar (mobile + desktop).
- Light/Dark mode toggle using `next-themes`.
- Progress tracking with a circular completion chart.

### 🧑‍💻 User Experience
- Personalized avatars with DiceBear.
- Smooth animations & hover effects via Tailwind CSS.

### ⚒️ Developer Tools
- **TypeScript** for static typing.
- **Redux Toolkit** for state management.
- **ESLint + Prettier** for clean, consistent code.

---

## Technologies Used
- **Framework:** Next.js (React framework with App Router)
- **Language:** TypeScript
- **State Management:** Redux with Redux Toolkit
- **Styling:** Tailwind CSS
- **Theming:** next-themes
- **UI Components:** shadcn/ui
- **Icons:** Lucide React
- **Avatar Generation:** DiceBear Avatars
- **Linting:** ESLint with `eslint-plugin-next`, `@typescript-eslint`, and `eslint-config-prettier`
- **Build Tool:** Node.js with npm
- **Miscellaneous:** Web APIs for browser notifications and audio playback, Weather data integration

## Prerequisites
- Node.js (v18.x or later recommended)
- npm (v9.x or later, comes with Node.js)
- A code editor like VS Code
- (Optional) Git for cloning the repository

## Setup Project Environment

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/task-manager.git
cd task-manager
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables
Create a `.env.local` file in the root directory:
```env
NEXT_PUBLIC_WEATHER_API_KEY=your_openweathermap_api_key
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```
- `NEXT_PUBLIC_WEATHER_API_KEY`: Required for weather data (get one from OpenWeatherMap).
- `NEXT_PUBLIC_BASE_URL`: Base URL for the app (optional, adjust for production).

### 4. Run the Development Server
```bash
npm run dev
```
Open your browser and navigate to `http://localhost:3000`.

### 5. Build for Production
```bash
npm run build
```
Then start the production server:
```bash
npm start
```

### 6. Lint and Format Code (Optional)
Run ESLint to check for linting issues:
```bash
npm run lint
```
Fix linting issues automatically (if configured):
```bash
npm run lint -- --fix
```

## Project Structure
```
task-manager/
├── public/              # Static assets (e.g., alert.mp3)
├── src/
│   ├── app/            # Next.js App Router pages (e.g., page.tsx)
│   ├── components/     # Reusable components (e.g., TaskList.tsx, TaskInput.tsx)
│   ├── lib/            # Utility functions (e.g., cn.ts for Tailwind)
│   ├── redux/          # Redux store, actions, and reducers
│   ├── types/          # TypeScript type definitions (e.g., task.ts)
│   └── styles/         # Global styles (if any)
├── eslint.config.mjs    # ESLint configuration
├── next.config.js       # Next.js configuration
├── package.json         # Dependencies and scripts
├── tsconfig.json        # TypeScript configuration
└── README.md            # This file
```

## Usage
- **Add a Task:** Click "Add Task" to create a new task with optional reminder and location.
- **Set Reminders:** Specify a date/time for reminders; you’ll hear an audio alert and see a notification when due.
- **View Weather:** For outdoor tasks, enter a location to see current weather conditions.
- **Toggle Theme:** Switch between light and dark modes using the theme button (☀️/🌙).
- **Filter Tasks:** Use the sidebar to filter tasks by category or search via the top bar.



