Harry Potter TCG: Pocket Magic Awakened — Simulator V1.30

V1.30 — GitHub Pages preparation

This version is prepared to run as a static web application on GitHub Pages.

What was prepared:
- All card, Lesson, and deck-back image paths use relative paths.
- The simulator does not depend on a local server or backend to load the current game UI.
- Local deck data continues to use browser localStorage.
- Added .nojekyll so GitHub Pages can publish the project without Jekyll processing.
- Local Play Both Seats remains available and unchanged.
- The existing offline Invite Player lobby remains as a placeholder for the future online lobby.
- No multiplayer networking has been added yet.

Current gameplay features retained:
- 30-card Main Deck + 10 Lessons + 1 Starting Ally.
- Local two-seat play.
- Switch Side perspective.
- Drag cards into Play Area, Lesson Area, Hand, Main Discard, and Lesson Discard.
- Last discarded card image displayed in each discard pile.
- Spacebar ends the current turn.
- Deck Builder and Card Database.

GitHub Pages setup:
1. Create a GitHub repository.
2. Upload the CONTENTS of this project folder to the repository root.
3. Make sure index.html is in the repository root.
4. In GitHub, open Settings → Pages.
5. Under Build and deployment, choose "Deploy from a branch".
6. Select the main branch and the "/ (root)" folder, then save.
7. GitHub will provide the public Pages address after deployment.

Important:
- Do not open the project from a subfolder if you want the normal GitHub Pages structure; index.html should be at the published root.
- The cards/ and data/ folders must remain next to index.html.
- Browser localStorage is local to each player's browser/device. It is not shared between players.

Next multiplayer milestone:
- Replace the current offline Invite Player placeholder with a real online room system.
- Create Room → generate a short room code → friend enters the code → both select decks → Ready → Start Game.
