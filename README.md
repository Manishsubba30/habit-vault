# Habit Vault

**Build better habits. Keep them to yourself.**

Habit Vault is a free, private habit tracker that runs entirely in your browser. Everything you enter is encrypted on your device with a passcode only you know. There's no account, no server and no ads.

## What it does

- **Month and week views**: tick off habits on a calendar grid, with daily progress, perfect days and a goal-vs-actual analysis.
- **Flexible goals**: every day, N days a week (e.g. gym 5 days a week) or N days a month. Rest days are free and only skips beyond them count as missed. Weeks run Monday to Sunday even across months.
- **Playbooks**: a motivational page for each habit (why it matters, what you gain, the cost of skipping, return on investment, quotes) that you can edit.
- **Money tracker**: income, a needs/wants/savings split, daily expenses and spending charts.
- **Gym log**: sets, weights and reps, personal records, strength charts, body weight and encrypted progress photos with a before/after view.
- **Share progress**: make an image of the habits you choose to send to a friend.
- **Several people, one device**: each person logs in with their own name and passcode. Nobody's name is shown on the lock screen.
- **Works on phones**: open it in your phone's browser and choose "Add to Home Screen".

## Privacy and security

| | |
|---|---|
| Encryption | AES-256-GCM with a fresh random IV on every save; photos encrypted one by one |
| Key | PBKDF2-SHA256, 600,000 iterations, random 128-bit salt, from your passcode |
| Storage | Your browser only (localStorage, photos in IndexedDB). Only encrypted data is written |
| Network | None. A Content-Security-Policy blocks all network requests |
| Login | Vaults are found by a SHA-256 hash of your name, so the lock screen lists nobody |

Your passcode can't be recovered. Make an encrypted backup from Settings now and then; it's safe to keep in cloud storage. Each device keeps its own vault, so use backup and restore to move between phone and computer.

## Run it yourself

It's a single file with no build step. Download `index.html` and open it in any modern browser, or host it anywhere static.

## Licence

MIT © 2026 Manish Subba. See [LICENSE](LICENSE).
