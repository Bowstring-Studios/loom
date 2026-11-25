# Loom

A Bowstring-built recreation of Kantata (formerly Mavenlink): project dashboard, time tracking, resourcing, and a per-project Gantt/task tracker.

Live demo: https://loom-five-gamma.vercel.app (pushes to `main` auto-deploy here)

## Running locally

```bash
python3 -m http.server 4173 --directory webapp
```

Then open http://localhost:4173.

## Data

When opened as a Claude Artifact, Loom reads and writes real shared data (projects, team, resourcing, per-user timesheets) through the artifact's built-in database.

Outside that environment (e.g. this Vercel deployment), there's no backend: Loom falls back to read-only sample data held in the page itself, so the UI can still be demoed but nothing is saved.
