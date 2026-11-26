# Money Tracker

Personal money tracker (income, expenses, budgets, goals, cicilan, lent money, business trips). Installable app (PWA) for Android and PC. Data stays on your device; optional sync to a private file in your own Google Drive.

## Install
1. Open the GitHub Pages link in Chrome (Android or PC).
2. Android: menu ⋮ → Install app. PC: install icon in the address bar.

## Google Drive sync setup (one time)
1. Go to console.cloud.google.com → create a project "Money Tracker".
2. APIs & Services → Library → enable **Google Drive API**.
3. OAuth consent screen → External → fill app name + your email → add yourself under **Test users**.
4. Credentials → Create credentials → OAuth client ID → **Web application**.
5. Authorized JavaScript origins: `https://lamejelly.github.io`
6. Copy the Client ID → app → Backup tab → Google Drive sync → paste → Connect & sync.

Only the hidden app folder (`drive.appdata` scope) is used; the app cannot see your other Drive files.
