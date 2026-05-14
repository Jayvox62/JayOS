# JayOS Portfolio Site

A retro terminal-themed personal portfolio homepage for Jamie Joyce.

## Current customisation

- Rebranded from `jamieOS` to **JayOS**.
- Removed old template/source-person references.
- Updated links:
  - GitHub: https://github.com/Jayvox62
  - LinkedIn: https://www.linkedin.com/in/jamie-joyce96/
- Projects now focus on:
  - **Lúgic** — safe, high-level browser tooling for formatting, parsing, diagnostics, and local-first workflow usability.
  - **CineClash** — a movie-chain game project.
- Education/certifications:
  - BSc in Computing
  - ITIL Foundation — pending certification, curriculum completed
- Public “Guestbook” wording has been renamed to **Open Channel**.

## Run locally

```bash
npm install
ADMIN_PASSWORD=your-password SESSION_SECRET=some-long-random-string npm start
```

Then open:

```text
http://localhost:3000
```

## Render settings

If this project is inside a folder in your GitHub repo, set Render’s **Root Directory** to that folder.

```text
Build Command: npm install
Start Command: npm start
```

Environment variables required on Render:

```text
ADMIN_PASSWORD=choose-a-password
SESSION_SECRET=choose-a-long-random-string
NODE_ENV=production
```

## Admin access

You are not admin automatically. Click **login** on the site and enter the value you set as `ADMIN_PASSWORD` in Render. Once logged in, the customize panel becomes available.

Do not commit `.env` or `node_modules/`.
