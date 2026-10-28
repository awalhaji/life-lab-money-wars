# LIFE LAB MONEY WARS — competition package

## Play immediately (no setup)
Open `offline-game.html` in Chrome. This is pass-and-play on one computer, not remote multiplayer.

## Play on different computers (requires setup)
1. Create a Firebase project at https://console.firebase.google.com/.
2. Enable Realtime Database. In Project settings > Your apps, register a Web app.
3. Open `firebase-config.js` in a text editor and replace each PASTE_* value with your Firebase web app config; include `databaseURL`.
4. Set Realtime Database rules. `database.rules.json` is a demonstration-only rules file, NOT safe for public deployment. Use only for a controlled test. Secure production requires authentication and server-side authorization.
5. Upload `index.html`, `firebase-config.js`, `offline-game.html` to a public GitHub repository root. GitHub Settings > Pages > Deploy from branch > main > root.
6. Visit the Pages website (not a local file). Create a room on computer A and join using the code on computer B.

## Troubleshooting
Opening `index.html` directly from Finder cannot connect to Firebase; the page now shows an explanation instead of a blank modal. If online is not configured, use `offline-game.html`.

## Competition description
LIFE LAB: Money Wars is a financial strategy game for 2–4 players. Players manage $1,500 starting cash, acquire properties, collect rent, build houses and hotels, and respond to life events. The game makes financial risk, budgeting, and investment tradeoffs tangible through play. The offline version is playable without internet. Online room-based multiplayer requires Firebase configuration and hosted deployment.
