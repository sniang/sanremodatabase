
# Sanremo Database

A multi-interface project for exploring the history, songs, and artists of the Sanremo Music Festival. Includes a React web app, a React Native mobile app, and a Node.js API, all powered by a curated dataset of festival performances.

---

## Table of Contents
- [About](#about)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Quick Start](#quick-start)
- [Development Notes](#development-notes)
- [Contact](#contact)

---

## About
Sanremo Database is an open-source project dedicated to making the history of the Sanremo Music Festival accessible and searchable. It provides:
- A modern web app for browsing songs, artists, and festival editions
- A mobile app for on-the-go exploration
- A simple API for programmatic access to the data

## Features
- Multilingual support (Italian, English, French)
- Search by year, singer, or song title
- Random song discovery
- Detailed festival rankings and categories
- Direct links to music platforms (YouTube, Spotify, Apple Music, Amazon Music, Deezer)
- Embedded YouTube videos for instant playback

## Repository Structure
Top-level folders:
- `web/` – Vite/React web app and static site files
- `app/` – React Native (Expo) mobile app
- `api/` – Node.js microservice for data access
- `admin/` – static admin pages

## Quick Start
Each part of the project runs independently. Choose one to get started:

### API (Node.js)
```bash
cd api
npm install
node index.js
```
See `api/README.md` for endpoint details.
Is currently running on the VPS using `pm2`.

### Web (Vite React)
```bash
cd web
npm install
npm run dev # Start in localhost for test
```
Build for production:
```bash
npm run build
npm run preview
```

### Mobile App (Expo)
```bash
cd app
npm install
npx expo start # Open on a device using Expo Go or run on simulator
```

## Development Notes
- The `web` app uses Vite and React. See `web/package.json` for scripts.
- The `app` directory is an Expo project (React Native).
- The `api` folder contains a minimal Node.js server for development.
- Static site folders for multiple languages: `en/`, `fr/`, `it/`.

## Contact
Maintainer: Samuel Niang ([Portfolio](https://samuelniang.eu))
Email: [contact@sanremodatabase.eu](mailto:contact@sanremodatabase.eu)

