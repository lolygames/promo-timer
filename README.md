# Pomodoro Timer 🍅

A cute single-file Pomodoro timer with a soft Muse-like chime. Focus 25 / Short Break 5 / Long Break 15, session dots, adjustable durations, keyboard shortcuts (Space / R / 1-2-3), and light & dark mode.

**Quick Tasks (added 2026-10-10):** a small task list under the timer — type a task, pick a priority tag (Urgent / High / Medium / Low / Delegate), press Enter. Tap a tag to change priority, tap the task text to focus the timer on it, tick done or × to delete. Tasks are saved in your browser (localStorage), so they survive reloads on the same device — no account needed.

**Spark buddy (added 2026-10-10):** a little original amber star buddy on the timer ring (pure SVG/CSS, still one file) that bobs/blinks when idle, cheers while you focus, gets sleepy with Zzz on breaks, and bounces when a session finishes. Respects reduced-motion settings.

## Put it on GitHub Pages (3 steps)

1. Create a new GitHub repo (e.g. `pomodoro-timer`) and upload `index.html` to the root (or run: `git init && git add index.html README.md && git commit -m "Pomodoro timer" && git branch -M main && git remote add origin https://github.com/<your-username>/pomodoro-timer.git && git push -u origin main`).
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` / `(root)`, Save.
3. After a minute your timer is live at `https://<your-username>.github.io/pomodoro-timer/` — bookmark it for day-to-day use.

## Notes

- Everything lives in the one `index.html` file — no build step, no dependencies to install.
- Fonts load from Google Fonts, so the timer needs internet the first time it loads; after that the browser caches them.
- If a session ends while the tab is in the background, the chime/vibration fires when the browser allows it — keeping the tab open (even unfocused) works best.
