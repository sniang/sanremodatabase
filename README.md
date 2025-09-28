# Sanremo Satabase

A small collection of projects for the Sanremo song database: a static web frontend, a React web app (Vite), a React Native mobile app, and a tiny API used by the apps.

This repository collects the data and multiple frontends used to browse Sanremo Festival songs by year, singer, and other filters.

Table of contents
- About
- Repository structure
- Quick start
	- Web (Vite React)
	- Mobile app (Expo / React Native)
	- API (Node.js)
- Data
- Development notes
- Contributing
- License

About
-----
The goal of this project is to provide an accessible, searchable database of songs and artists who have participated in the Sanremo Music Festival across years. The repository contains multiple interfaces:

- `web` - a Vite/React web app and static HTML pages used as the main public website.
- `app` - a React Native (Expo) mobile application.
- `api` - a small Node.js API used to serve data to the apps or for development.
- `admin` - static admin pages and supporting files.

Repository structure
--------------------
Top-level folders and their purpose:

- `web/` - front-end web app (Vite + React) and static site files. Contains `src/` React components and the data used by the site in `web/data_analyst/json/`.
- `app/` - React Native (Expo) application used on mobile. Contains components, screens and assets.
- `api/` - Node.js microservice that exposes endpoints used by the frontends (simple local server).
- `admin/` - static admin pages.

Quick start
-----------
The repository includes three independent parts. Pick the one you want to run.

Web (Vite React)

1. cd into the `web` folder
2. Install dependencies (npm or yarn)

```bash
cd web
npm install
# or: yarn
```

3. Start the dev server

```bash
npm run dev
```

4. Build for production

```bash
npm run build
npm run preview
```

Mobile app (Expo)

1. cd into the `app` folder
2. Install dependencies

```bash
cd app
npm install
# or: yarn
```

3. Start Expo

```bash
npm start
# then open on a device using Expo Go or run on simulator
```

API (Node.js)

1. cd into the `api` folder
2. Install dependencies and start the server

```bash
cd api
npm install
node index.js
```

By default the API is tiny and intended for development. See `api/README.md` for details.


Development notes
-----------------
- The `web` app is built with Vite and React. Look at `web/package.json` for available scripts.
- The `app` directory is an Expo project (React Native). Look at `app/package.json` for scripts and dependencies.
- The `api` folder contains a minimal Node.js server used during development.
- Static site folders for multiple languages are present: `en/`, `fr/`, `it/` containing pre-rendered HTML pages.

Contributing
------------
Contributions are welcome. Please open issues or pull requests with clear descriptions. Typical contribution types:

- Frontend improvements: make UI/UX changes in `web/src` or `app/components` and include screenshots when relevant.
- Bug fixes: include a short test or reproduction steps.

If you're updating data, please include the provenance/source for the data and any script used to transform it.

License
-------
This repository does not include a license file. Add a LICENSE to indicate how you'd like the project to be used. If you want, use MIT or Creative Commons for data.

Contact
-------
If you are the maintainer and want your contact or project site added here, update this README accordingly.

Acknowledgements
----------------
Thanks to the maintainers and contributors who collected and cleaned the Sanremo dataset.
