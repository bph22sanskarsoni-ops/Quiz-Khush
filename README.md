# 🎮 Quiz Khush

Multiplayer AI Quiz game — up to 10 players!

## Setup

### 1. Add your Firebase Database URL
Open `index.html` and find this line:
```
Replace with your actual URL like:
```
databaseURL: "https//:Quiz-Khush.web.apo",
```

### 2. Firebase Realtime Database Rules
Go to Firebase Console → Realtime Database → Rules → paste this:
```json
{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null"
  }
}
```

### 3. GitHub Pages Deploy
1. Create GitHub repo named `quiz-khush`
2. Upload all files
3. Settings → Pages → Deploy from main branch

### 4. Firebase Hosting (Optional)
```
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

## Features
- 🔐 Email/Password Auth
- 👥 Friend system with UID
- 🔔 Free Fire style notifications
- 🎮 Room system (up to 10 players)
- 🤖 AI-generated questions (Claude)
- 🏆 Live leaderboard
- 📱 Mobile responsive
