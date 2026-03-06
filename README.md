# Solo Quiz Live Game (Firebase)

This is a **GitHub Pages hostable** live quiz app.

## Files
- `index.html` → the full quiz app
- `firestore.rules` → Firestore security rules for quick setup

## What this app does
- Host creates a game
- Shows **GAME PIN** and **QR code**
- Players join from phones/laptops
- **10-second timer** per question
- **Fastest correct answer scores highest**
- Live **scoreboard**

## Before publishing
Open `index.html` and paste your Firebase web config inside:

```js
const firebaseConfig = {
  apiKey: "",
  authDomain: "",
  projectId: "",
  storageBucket: "",
  messagingSenderId: "",
  appId: ""
};
```

## Firebase setup
1. Go to Firebase Console
2. Create a project
3. Add a **Web App**
4. Copy the config into `index.html`
5. Enable **Cloud Firestore**
6. In Firestore Rules, paste the contents of `firestore.rules`

## GitHub Pages steps
1. Create a new GitHub repository
2. Upload these files to the repository root
3. Commit the files
4. Go to **Settings → Pages**
5. Under **Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
6. Save

Your app will be live at:

```text
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

## Important note
This app is a static site, so GitHub Pages can host it directly.
Realtime multiplayer works because the game state is stored in **Firestore**.

## Firestore rules
The included rules are intentionally simple for event/demo use.
Tighten them later if needed.
