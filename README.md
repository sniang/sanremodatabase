
# Sanremo Database

A multi-interface project for exploring the history, songs, and artists of the Sanremo Music Festival. Includes a React web app, a Capacitor-based lite app, a React Native mobile app, and a Node.js API, all powered by a curated MySQL dataset of festival performances.

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Quick Start](#quick-start)
- [Development Notes](#development-notes)
- [Contact](#contact)
- [License](#license)

---

## About

Sanremo Database is a project dedicated to making the history of the Sanremo Music Festival accessible and searchable. It provides:

- A modern **web app** for browsing songs, artists, and festival editions
- A **lite mobile app** (Capacitor) for iOS and Android
- A **React Native app** (Expo) for a richer mobile experience
- A **REST API** for programmatic access to the data

## Features

- Multilingual support (Italian, English, French)
- Search by year, singer, or song title
- Random song discovery
- Detailed festival rankings and categories
- Direct links to music platforms (YouTube, Spotify, Apple Music, Amazon Music, Deezer)
- Embedded YouTube videos for instant playback
- AI-generated news summaries about the festival
- Secure admin authentication (JWT) for data management

## Repository Structure

This monorepo uses [Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules):

| Folder | Description | Tech Stack |
|---|---|---|
| [`web/`](web/) | Main web application | Vite, React, MUI |
| [`lite_app/`](lite_app/) | Lite mobile app (iOS & Android) | Vite, React, Capacitor |
| [`app/`](app/) | React Native mobile app | Expo, React Native |
| [`api/`](api/) | REST API | Node.js, Express, MySQL |

## Quick Start

Each part of the project runs independently. See the README in each subfolder for full details.

### API (Node.js)

```bash
cd api
npm install
node index.js
```

> **Note:** You need to set `JWT_SECRET` in your `.env` file and create an admin account with `node scripts/create-admin.js`. See [`api/README.md`](api/README.md) for full setup.

### Web (Vite + React)

```bash
cd web
npm install
npm run dev
```

Build for production:

```bash
npm run build
npm run preview
```

### Lite App (Capacitor)

```bash
cd lite_app
npm install
npm run dev
```

Build and sync for native platforms:

```bash
npm run build
npx cap sync
npx cap open ios    # or: npx cap open android
```

### Mobile App (Expo)

```bash
cd app
npm install
npx expo start
```

## Development Notes

- The `web/` and `lite_app/` apps both use Vite + React + MUI. The lite app adds Capacitor for native builds.
- The `app/` directory is an Expo project (React Native).
- The `api/` folder runs an Express server backed by MySQL.
- Each submodule has its own `package.json` and can be developed independently.

## Contact

**Maintainer:** Samuel Niang — [Portfolio](https://samuelniang.eu)
**Email:** [contact@sanremodatabase.eu](mailto:contact@sanremodatabase.eu)

## Support

If you enjoy this project, consider supporting the developer:

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T81A76CO)

## License

All rights reserved © 2025–2026 Samuel Niang

