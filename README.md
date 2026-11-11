# Pegasus Training Flow – UI prototype

Clickable prototype of the three training-ticket flows in Pegasus (incident, commissioning, client request), the trainer workspace and the pilot SMS confirmation. It is a single static page with no build step and no backend; data resets on every refresh.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `pegasus-training-prototype`).
2. Upload `index.html`, `.nojekyll` and this `README.md` to the repository root (Add file → Upload files → Commit).
3. Open **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

Note: GitHub Pages sites from a free account are public. For a private site you need GitHub Enterprise Cloud, or host it internally instead.

## Run locally

Open `index.html` in any browser. Nothing to install.

## How to use

Use the bar at the top to switch views:

- **Pegasus user** – Flow 1: Parent Tickets → Ticket-17157 → Timeline → Initiate Training. Flow 2: Delivery Tracker → edit a drone → Pilot & Field → Initiate Training. "Logged in as" changes who raises the ticket.
- **Ticket creator** – Flow 3: Initiate Training next to Need Any Support?.
- **Trainer** – update tickets, set Training Completed, send the confirmation SMS.
- **Pilot (SMS link)** – stand-in for the existing SMS page: rate 1–5 and confirm to auto-close.

**Reset demo** clears everything. The page loads the Inter font from Google Fonts and falls back to the system font when offline.
