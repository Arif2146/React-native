
# Movie — React Native Expo App

A compact, modern React Native mobile app built with Expo, TypeScript and Expo Router. This repository contains the Movie app (under the `Movie/` directory) — a small starter demonstrating navigation via expo-router, NativeWind (Tailwind for React Native), and a clean component + asset structure.

---

## Table of contents

- [Demo / overview](#demo--overview)
- [Tech stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Quick start](#quick-start)
	- [Install dependencies](#install-dependencies)
	- [Run locally (development)](#run-locally-development)
	- [Run on device / simulator](#run-on-device--simulator)
- [Project structure](#project-structure)
- [Key concepts & components](#key-concepts--components)
- [Styling & Assets](#styling--assets)
- [Contributing](#contributing)
- [Troubleshooting](#troubleshooting)
- [License & contact](#license--contact)

---

## Demo / overview

This project demonstrates a simple movie UI built with Expo and the expo-router file-based navigation. It includes a top-level layout, tab layout under `(tabs)`, a movie details route, and a reusable `Search` component.

The source app files live inside `Movie/` — open that folder to run and work on the app.

---

## Tech stack

- Expo (managed workflow)
- React 19
- React Native 0.81.x
- expo-router (file-based routing)
- Nativewind (Tailwind-like styling for RN)
- TypeScript

---

## Prerequisites

- Node.js (16.x or later recommended)
- npm or yarn
- Expo CLI (optional; you can use the built-in package scripts)
- A phone with Expo Go or a local Android/iOS simulator

---

## Quick start

All project files are contained in the `Movie/` folder. A common workflow is to open a terminal at the repository root and change into that folder before running commands.

Install dependencies

PowerShell example:

```powershell
cd Movie
npm install
```

or using yarn:

```powershell
cd Movie
yarn install
```

Run locally (development)

Start the Expo dev server (Metro) with the default script:

```powershell
cd Movie; npm run start
```

Common platform-specific scripts (from `package.json`):

- npm run android — open on Android device / emulator
- npm run ios — open on iOS simulator (macOS only)
- npm run web — run as web app (react-native-web)
- npm run lint — run ESLint checks
- npm run reset-project — helper script included in repository

---

## Project structure (high level)

Top-level (inside `Movie/`):

- app/ — expo-router file-based pages and layouts
	- _layout.tsx — root layout (registers stack)
	- (tabs)/ — tabbed layout and screens
	- movie/ — details route for a movie (example: `movie/[id]`)
- assets/ — fonts, icons, images used by the app
- component/ — local reusable components, e.g., `searchBar.tsx`
- constants/ — images.ts, icons.ts
- package.json — scripts & dependency manifest
- tsconfig.json — TypeScript configuration

---

## Key concepts & components

- File-based routing: `expo-router` uses files in `app/` to define navigation. Layout files such as `_layout.tsx` and `(tabs)/_layout.tsx` control structure and shared UI.
- Reusable component example: `component/searchBar.tsx` — a simple search UI element used on the home screen.
- Assets: icons and images are stored under `assets/` and exported via `constants/icons.ts` and `constants/images.ts` for convenience.

---

## Styling & Assets

This project uses Nativewind (Tailwind style classes for React Native) and includes a `globals.css` file for global styles used by the router entry.

Fonts and images should be imported via the `assets/` folder and referenced using the constants files for consistency.

---

## Contributing

Contributions are welcome. Suggested steps for contributing:

1. Fork the repo
2. Create a feature branch (feature/your-feature)
3. Make your change with tests (if relevant)
4. Open a pull request describing the change and motivation

Please run `npm run lint` and ensure formatting is clean before submitting.

---

## Troubleshooting

- If you run into problems with the dev server, try clearing Metro cache by running: `expo start -c` or the included `npm run reset-project` script.
- Make sure your Node version is compatible and that you installed dependencies from inside the `Movie/` folder.

---

## License & contact

This repo doesn't explicitly include a license file (add one if you'd like to change the project's license). For questions or help, open an issue or contact the repository owner.

---

Happy hacking! 🎬

# React-Native Project

## 🔎 Overview  
This project contains a React Native application developed by me.  
It is intended to serve as a demo / template / starter project (modify as appropriate) — containing core functionality and setup to get started quickly with React Native.  

## 🚀 Features  
- Basic React Native setup (TypeScript + JavaScript + styling)  
- Cross-platform support (Android, iOS) *(if applicable — update accordingly)*  
- Modular code structure to facilitate easy development and extension  

## 🧰 Technologies Used  
- React Native  
- TypeScript / JavaScript  
- CSS / React Native Stylesheets  

## 📥 Installation & Running the Project  

```bash
# Clone the repository  
git clone https://github.com/Arif2146/React-native.git  
cd React-native

# Install dependencies  
npm install  
# or  
yarn install

# Run on Android (or iOS emulator / device)  
npm run android  
# or  
yarn android
