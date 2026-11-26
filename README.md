# Money Tracker

Personal money tracker for Android and PC. Installable app (PWA), works offline. Your data stays on your device; optional sync to a private file in your own Google Drive.

**Features:** income and expenses, wallets (add / rename / archive), budgets, recurring expenses, savings goals, cicilan, money lent to friends, business trips (dinas), CSV/JSON export and import, PIN lock, English / Bahasa Indonesia / 中文.

## Install
1. Turn on GitHub Pages: repo **Settings → Pages → Deploy from a branch → `main` / root**.
2. Open the Pages link in Chrome.
3. Android: menu ⋮ → **Install app**. PC: install icon in the address bar.

## Google Drive sync (one time)
1. console.cloud.google.com → create a project "Money Tracker".
2. APIs & Services → Library → enable **Google Drive API**.
3. OAuth consent screen → External → fill app name + your email → add every Google account you will use under **Test users**.
4. Credentials → Create credentials → OAuth client ID → **Web application**.
5. Authorized JavaScript origins: `https://<your-github-username>.github.io`
6. Copy the Client ID → app → More → Backup & import → Google Drive sync → paste → **Connect & sync**.

Use **Switch account** to pick another Google account, **Disconnect** to revoke access.
While the consent screen is in "Testing", Google asks you to sign in again about every 7 days.

## Security notes
- Only the hidden app folder is used (`drive.appdata` scope). The app cannot see your other Drive files.
- The sign-in token is kept in memory only, never stored.
- PIN lock (More → Security) is a screen lock, not encryption. Keep your device lock and Google 2-step verification on.
- Exported CSV/JSON files are plain text. Store them somewhere safe.
- Never record card numbers or PINs in notes.
