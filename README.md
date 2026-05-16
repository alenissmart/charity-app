# Getting Started

This guide walks you through setting up and running this app from scratch on your computer.

---

## Step 1 — Install Node.js

1. Go to [https://nodejs.org](https://nodejs.org)
2. Download the **LTS** version (the left button)
3. Open the downloaded file and follow the installer — just keep clicking Next
4. Once done, open a terminal and verify it worked:
   ```
   node --version
   ```
   You should see a version number like `v22.0.0`

---

## Step 2 — Install Git

1. Go to [https://git-scm.com](https://git-scm.com)
2. Download and install it for your operating system
3. **Windows:** during installation, when asked about default editor, select **Use Visual Studio Code** — leave everything else as default
4. Once done, verify it worked:
   ```
   git --version
   ```
   You should see a version number like `git version 2.47.0`

---

## Step 3 — Install VS Code


1. Go to [https://code.visualstudio.com](https://code.visualstudio.com)
2. Download and install it for your operating system
3. Open VS Code and install these two extensions (click the Extensions icon on the left sidebar):
   - **ES7+ React/Redux/React-Native snippets**
   - **Prettier - Code formatter**

---

## Step 4 — Install Expo Go on your phone

1. Open the **App Store** (iPhone) or **Google Play Store** (Android)
2. Search for **Expo Go** and install it
3. Make sure your phone and computer are on the **same Wi-Fi network**

---

## Step 5 — Download this project

If you have Git installed:
```
git clone <repository-url>
cd <project-folder>
```

Or download the ZIP from the repository page and extract it, then open the folder in VS Code.

---

## Step 6 — Install project dependencies

1. In VS Code, open the terminal (Terminal → New Terminal from the top menu)
2. Run:
   ```
   npm install
   ```
3. Wait for it to finish — this installs everything the app needs to run

---

## Step 7 — Start the app

In the terminal, run:
```
npx expo start
```

A QR code will appear in the terminal.

---

## Step 8 — Open on your phone

- **iPhone:** Open the Camera app and point it at the QR code — tap the notification that appears
- **Android:** Open the Expo Go app, tap **Scan QR code**, and scan it

The app should launch on your phone within a few seconds.

---

## Adding a New Level

1. Copy `app/game/g1.tsx` and rename it to the next number (e.g. `g10.tsx`)
2. Inside the new file, change the function name and title text to match the new number
3. Open `app/levels.tsx` and add the new level ID to the `LEVELS` array at the top:
   ```
   const LEVELS = ['g1', 'g2', ..., 'g10'];
   ```
4. Save both files — the new level will appear in the level select screen automatically

---

## Troubleshooting

**`npm install` fails**
- Make sure Node.js is installed correctly by running `node --version` in the terminal

**QR code doesn't work**
- Make sure your phone and computer are on the same Wi-Fi network
- Try pressing `r` in the terminal to reload

**App shows a blank screen**
- Press `r` in the terminal to reload the app
- Check the terminal for any red error messages and copy them into your AI assistant

**Expo Go says SDK version mismatch**
- Make sure you have the latest version of Expo Go installed on your phone