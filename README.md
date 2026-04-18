# Icy Tower My Way

`Icy Tower My Way` is a browser-based arcade platformer inspired by Icy Tower. The goal is to keep climbing, land on higher platforms, avoid hazards, and beat your best score.

The project is built as a lightweight static web game using:

- `HTML`
- `CSS`
- `JavaScript`
- `Canvas API`

## Features

- Endless vertical climbing gameplay
- Smooth screen scrolling as the player climbs
- Start menu and game over screen
- Score system with best-score leaderboard
- Keyboard controls
- Touch controls for mobile devices
- Camera mode with hand tracking
- Sound effects, background music, and mute toggle
- Animated background and themed visual assets
- Multiple hazards and collectible power-ups

## Controls

### Keyboard

- `Left Arrow`: move left
- `Right Arrow`: move right
- `Space`: jump

### Touch

On touch devices, on-screen buttons appear for:

- `Left`
- `Right`
- `Jump`

### Camera Mode

If you choose `Start with Camera`, the game uses hand tracking:

- Both hands up: jump
- Left hand up: move left
- Right hand up: move right

## Gameplay Mechanics

- You earn points by landing on new, higher platforms.
- Platforms can fall if you stand on them too long.
- Some platforms move.
- Some platforms crack and collapse shortly after you land on them.
- Enemies can block your climb, move across platforms, or shoot at you.
- A falling snow-storm hazard can instantly end the run.

### Power-Ups

- `Star`: temporary protection from enemy and bullet hits
- `Spring`: boosts your next jump
- `Diamond`: collect 5 to trigger a super jump

## How to Run

This is a static project, so no build step is required.

1. Clone or download the repository.
2. Open the project folder.
3. Run it in a browser.

You can usually do this in one of two ways:

- Open `index.html` directly in the browser
- Use a local development server such as VS Code Live Server

## Camera Mode Notes

- Camera mode requires webcam permission in the browser.
- It works best when the game is served from `localhost` or another secure context.
- The hand tracking model is loaded from external MediaPipe/CDN URLs, so an internet connection is needed for camera mode.

## Project Structure

.
|-- index.html
|-- style.css
`-- assets/

## Best Scores

Best scores are stored in `sessionStorage`, which means they are kept for the current browser session and may reset after the tab or browser is closed.

## Credits

- Inspired by the classic `Icy Tower`
- Uses themed custom art, audio, fonts, and browser-based canvas rendering

