# Eureka Blueberry Dash

A Crossy Road–style endless hopper starring the farmers of Eureka. Hop across roads,
rivers, and bike paths, fill your bucket with blueberries to unlock new farmers
(Andrew up to Ridley), and climb the global leaderboard. Every 100 jumps you dive
into the sewer and the next level runs 10% faster.

**Play it:** https://joshmcguiness.github.io/eureka-blueberry-dash/

## Controls

- **Desktop:** arrow keys / WASD
- **Touch (iPad/phone):** on-screen D-pad or swipe

## How it's built

- `index.html` — the entire game: canvas renderer (45° isometric), game logic, sounds, UI. No dependencies.
- Leaderboard: shared Cloudflare Worker (`rat-road-leaderboard`, board `berry`) — source lives in the
  [tommys-rat-road](https://github.com/joshmcguiness/tommys-rat-road) repo under `worker/`.

## Deploying

GitHub Pages deploys `index.html` from `main` via the Actions workflow on every push.
