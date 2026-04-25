# Foresight Grid MVP

A deploy-ready React/Vite prototype for a strategic foresight game inspired by GeoGrid, built for family offices, next-generation principals, and executive education cohorts.

## What is included

- Daily Signal Briefing
- False Signal Gauntlet
- Signal Clustering Challenge
- Scenario Builder
- Expert feedback panels
- Alignment, calibration, and timing scores
- Static sample signals for prototype testing
- Plain CSS; no Tailwind configuration required
- Ready for GitHub + Vercel deployment

## File structure

```text
foresight-grid/
  package.json
  index.html
  vite.config.js
  vercel.json
  src/
    main.jsx
    App.jsx
    styles.css
```

## Run locally

```bash
npm install
npm run dev
```

Open the local URL shown in the terminal, usually:

```text
http://localhost:5173
```

## Deploy to Vercel

1. Create a new GitHub repository.
2. Upload all files and folders from this project.
3. Go to Vercel.
4. Click **New Project**.
5. Import the GitHub repository.
6. Use these settings:
   - Framework: Vite
   - Build command: `npm run build`
   - Output directory: `dist`
   - Install command: `npm install`
7. Click **Deploy**.

## Important

Do not paste `src/App.jsx` into `index.html`.

The correct flow is:

```text
index.html loads src/main.jsx
src/main.jsx loads src/App.jsx
src/App.jsx contains the game code
```

## Next product step

Replace the static `SIGNALS` array in `src/App.jsx` with data from Supabase, Airtable, or a CMS. For the first paid pilot, static data is acceptable if you manually update and redeploy each round.
