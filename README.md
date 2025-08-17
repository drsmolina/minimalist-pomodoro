# Minimalist Pomodoro (GitHub Pages)

A clean, single-file Pomodoro timer built with React (UMD) + Tailwind via CDN. No build tools.

**Live locally:** open `index.html` in your browser.

## Features
- Focus / Short / Long sessions, with auto-advance
- Rounds tracker (e.g., long break every 4 focus sessions)
- Progress ring, keyboard shortcuts, and subtle beep
- LocalStorage persistence for settings/state
- Optional desktop notifications when sessions end

## Keyboard Shortcuts
- **Space**: Start/Pause
- **R**: Reset current session
- **N**: Skip to next session
- **1 / 2 / 3**: Focus / Short Break / Long Break

## Deploy on GitHub Pages
1. Create a new GitHub repository (e.g., `minimalist-pomodoro`).
2. Upload `index.html` and `README.md` to the **root** of the repo (drag-and-drop on GitHub works).
3. Go to **Settings → Pages**.
4. In **Build and deployment**, select **Deploy from a branch**.
5. Choose branch **main** and folder **/** (root). Click **Save**.
6. Wait for the green check. Your site will be available at:
   - `https://<your-username>.github.io/<your-repo>/`

## Customization
- All durations and behavior are adjustable from the in-app **Settings**. Values persist via `localStorage`.
- To hardcode defaults, edit the `useLocalStorage` initial values inside `index.html`.

## Notes
- Uses Babel in-browser for JSX to keep deployment zero-build. For heavier use, consider a Vite build later.
