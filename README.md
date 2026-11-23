# Harmony Waves Pro — Brony & Furry Radio

Modern responsive website, installable PWA and Capacitor-ready Android/iOS source.

## Run locally
`npm install && npm run start`

## Build
`npm run build` (output: `dist`)

## Render Static Site
Connect the GitHub repository; build command `npm install && npm run build`; publish directory `dist`. `render.yaml` is provided.

## Features
25 built-in community station entries, categories, station search, favorites, recently played, custom stations, surprise selection, persistent bottom player, volume, media-session controls, listening history of station tune-ins, and device-local diagnostics. Data is stored in localStorage.

## Important
Radio streams are third-party and may be offline, block browser playback, or require HTTPS. Station listings are not live-verified. Song title/artist artwork and true server-side uptime monitoring are **not implemented** because they require reliable station-specific metadata endpoints or a backend. The design uses category artwork instead of falsely claiming song cover art. See MOBILE_SETUP.md for native build instructions.
