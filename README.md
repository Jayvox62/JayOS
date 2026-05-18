# JayOS Portfolio Site

A retro terminal-themed personal portfolio homepage for Jamie Joyce, with an admin customize panel, Signal/contact area, projects, links, certifications, live theme editing, and an editable "currently" section.

## Included updates

- Rebranded the app to **JayOS**.
- Updated links to Jamie's GitHub and LinkedIn.
- Removed pronouns from the public profile and customize form.
- Removed unrelated TSOYP/template wording from the public-facing defaults.
- Cleaned projects down to **Lúgic**, **CineClash**, and **Scraggle**.
- Updated education/certifications to **BSc in Computing** and **ITIL Foundation — pending certification**.
- Added **Scraggle** as a portfolio project.
- Added an editable **currently** block for small human details like building, watching, playing, or thinking about.

## Run locally

```bash
npm install
cp .env.example .env
# edit .env and set ADMIN_PASSWORD
npm start
```

Visit `http://localhost:3000`. Click **login** and use the password from `.env`.

## Render setup

Use these commands:

```bash
Build Command: npm install
Start Command: npm start
```

Add these environment variables in Render:

```text
ADMIN_PASSWORD=your-admin-password
SESSION_SECRET=any-long-random-string
COOKIE_SECURE=true
NODE_ENV=production
```

## Config

| Variable | Required | Notes |
|---|---:|---|
| `ADMIN_PASSWORD` | yes | Password for the single admin user. |
| `PORT` | no | Defaults to `3000`. |
| `COOKIE_SECURE` | no | Set to `true` behind HTTPS, including Render. |
| `SESSION_SECRET` | no | Auto-generated into `data/session.secret` if omitted. |
| `DATA_DIR` | no | Defaults to `./data`. |

## Notes

All editable site state is stored in `./data/`. Back that folder up if you deploy it with persistent storage.

Original project is MIT licensed. Keep `LICENSE` when publishing your fork.
