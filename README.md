# To-Do App 📝

A modern to-do application built with React Native and Expo. Manage your tasks with a clean, intuitive interface that works on iOS, Android, and Web.

## Features

- ✅ Create, edit, and delete todos
- ✅ Mark todos as completed/incomplete
- ✅ Persistent storage using AsyncStorage
- ✅ Track total and completed todos count
- ✅ Modern UI with styled components
- ✅ Cross-platform support (iOS, Android, Web)

## Tech Stack

- **React Native** - Mobile framework
- **Expo** - Development platform
- **Expo Router** - File-based routing
- **TypeScript** - Type safety
- **AsyncStorage** - Local data persistence
- **React Hooks** - State management

## Project Structure

```text
├── app/                    # Main application screens
│   ├── _layout.tsx        # Root layout
│   └── index.tsx          # Main to-do screen
├── components/            # Reusable styled components
│   ├── StyledButton.tsx
│   ├── StyledCheckbox.tsx
│   ├── StyledModal.tsx
│   ├── StyledText.tsx
│   └── StyledTextInput.tsx
├── layout/                # Feature-specific components
│   ├── Header/            # App header with todo stats
│   ├── TodoCreator/       # Todo creation form
│   ├── TodoItem/          # Individual todo item
│   ├── TodoList/          # Todo list container
│   └── Modals/            # Edit and delete modals
├── hooks/                 # Custom React hooks
│   └── useTodo.ts         # Todo state management
├── types/                 # TypeScript type definitions
│   └── todo.ts
├── constants/             # App constants
│   ├── storage.ts         # Storage keys
│   └── ui.ts              # UI constants (colors, etc.)
└── helpers/               # Utility functions
    └── date.ts
```

## Getting Started

### Prerequisites

- Node.js (v18 or later)
- npm or yarn
- Expo CLI (optional, but recommended)

### Installation

1. Clone the repository

   ```bash
   git clone <repository-url>
   cd example_to-do
   ```

2. Install dependencies

   ```bash
   npm install
   ```

3. Start the development server

   ```bash
   npm start
   ```

   Or use one of the platform-specific commands:

   ```bash
   npm run android    # Start on Android
   npm run ios        # Start on iOS
   npm run web        # Start on Web
   ```

### Running the App

After starting the development server, you can:

- Press `a` to open in Android emulator
- Press `i` to open in iOS simulator
- Press `w` to open in web browser
- Scan the QR code with Expo Go app on your device

## Available Scripts

- `npm start` - Start Expo development server
- `npm run android` - Start on Android emulator
- `npm run ios` - Start on iOS simulator
- `npm run web` - Start on web browser
- `npm run lint` - Run ESLint
- `npm test` - Run tests
- `npm run reset-project` - Reset to blank project (development only)

## Usage

1. **Add a Todo**: Type your task in the input field and press enter or tap the add button
2. **Complete a Todo**: Tap the checkbox next to a todo to mark it as completed
3. **Edit a Todo**: Tap on a todo item to edit its title
4. **Delete a Todo**: Long press on a todo item and confirm deletion

All todos are automatically saved to local storage and persist between app sessions.

## Development

The app uses:

- **File-based routing** with Expo Router
- **TypeScript** for type safety
- **Custom hooks** for state management
- **AsyncStorage** for data persistence
- **Styled components** for consistent UI

## Learn More

- [Expo Documentation](https://docs.expo.dev/)
- [React Native Documentation](https://reactnative.dev/)
- [Expo Router Documentation](https://docs.expo.dev/router/introduction/)
