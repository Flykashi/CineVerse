# Cineverse

A beginner-friendly full stack movie catalog project with React and Express.

## Project structure

- `server/` - backend API using Express
- `client/` - frontend React app built with Vite
- `vercel.json` - Vercel build configuration for the frontend

## Local setup

1. From the repo root, install dependencies:
   - `npm install`
2. Run both services in development:
   - `npm run dev`
3. Open the frontend URL shown by Vite in your browser.

### Start services separately

- Frontend only: `npm run client`
- Backend only: `npm run server`

## Backend API

The server provides a simple movie API:

- `GET /api/health`
- `GET /api/movies`
- `GET /api/movies/:id`
- `POST /api/movies`
- `PUT /api/movies/:id`
- `DELETE /api/movies/:id`

## Vercel deployment

Use Vercel to deploy only the frontend from the repo root.

Settings to use in Vercel:

- Application Preset: `Other`
- Root Directory: `.`
- Build Command: `npm run vercel-build`
- Output Directory: `client/dist`

> The backend is not deployed by Vercel in this setup. If you want a full-stack deployment, host the backend separately and update `VITE_API_URL`.
