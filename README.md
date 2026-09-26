# Meridian — Allocation Arena

A browser strategy game where players allocate resources across assets, compete on a shared scoreboard, and earn top-three rewards.

## Run locally

Requires Node.js 18 or newer. From this directory:

```sh
npm start
```

Open `http://localhost:4173`. To let other devices join on the same Wi-Fi, use this computer's LAN address and port 4173.

## Deploy

This repository is configured for Render as a single Node web service. Create a new Web Service from this GitHub repository and use the included `render.yaml` settings. The service serves the game and multiplayer API from the same public URL.

## Playtest storage note

Rooms, player presence, and scores are currently held in memory. They are lost when the service restarts, redeploys, or sleeps. Use persistent storage before relying on long-lived game rooms.

