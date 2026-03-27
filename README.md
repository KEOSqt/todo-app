# Todo App

A lightweight, modern todo application built with **React**, **TypeScript**, and **Vite**.

This app helps you quickly capture tasks, track progress, and keep your list organized with simple filters. Todos are persisted in the browser using `localStorage`, so your tasks remain available after refresh.

## Features

- Add new tasks from the input form
- Mark tasks as complete/incomplete
- Delete tasks
- Filter tasks by:
  - **All**
  - **Active**
  - **Completed**
- Automatic persistence with `localStorage`
- Empty-state messaging for each filter
- Keyboard support for toggling task completion (`Enter` / `Space`)
- Responsive layout with light/dark color-scheme support

## Tech Stack

- **React 19**
- **TypeScript**
- **Vite**
- **ESLint**

## Getting Started

### Prerequisites

- Node.js (LTS recommended)
- npm

### Installation

```bash
npm ci
```

### Run in Development

```bash
npm run dev
```

Then open the local URL shown in your terminal (usually `http://localhost:5173`).

## Available Scripts

- `npm run dev` — start the Vite development server
- `npm run build` — type-check and create a production build
- `npm run lint` — run ESLint across the project
- `npm run preview` — preview the production build locally

## How It Works

- Todos are stored as an array of objects:
  - `id` (number)
  - `text` (string)
  - `completed` (boolean)
- Initial state loads from `localStorage` key `todos`
- Any update to the todo list is saved back to `localStorage`
- Filtering is done client-side in React state

## Project Structure

```text
.
├── public/
├── src/
│   ├── App.tsx        # Main todo application logic and UI
│   ├── App.css        # Component-specific styles
│   ├── index.css      # Global styles and theme variables
│   └── main.tsx       # React entry point
├── index.html
├── package.json
└── vite.config.ts
```

## Build Output

Running `npm run build` generates optimized files in the `dist/` directory for deployment.
