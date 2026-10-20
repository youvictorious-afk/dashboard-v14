# Dashboard V14 — Standalone personal workspace

A mobile-first, installable static dashboard inspired by a premium white-and-orange SaaS interface. This is a new, separate project; it does not modify or depend on any existing Life Dashboard repository.

## Included modules
- Overview with finance metrics, charts, tasks, recent activity and quick links
- Tasks and reminders with completion, due dates and priority
- Manual income/expense tracker with CSV export
- Account hub for website shortcuts
- Spanish study-time log and Spanish/English/Hindi vocabulary list
- Searchable notes vault and quick note
- Activity log, dark/compact modes, currency display
- JSON backup, restore/import, and reset controls
- PWA manifest and service worker for installability/offline shell

## Run locally
Open `index.html` in a browser. Most features work directly from local storage. For PWA installation and service worker support, serve the folder over HTTPS or localhost.

## Deploy to Cloudflare Pages
1. Create a **new** GitHub repository (for example `dashboard-v14`). Do not select or reuse the Life Dashboard repository.
2. Upload all files from this folder to the new repository root.
3. In Cloudflare Pages, create a new project and connect only this new repository.
4. Framework preset: `None`; build command: leave blank; build output directory: `/` (the repository root).
5. Deploy. Open the generated HTTPS URL on iPhone. In Safari, tap Share → Add to Home Screen.

## Data and security
- User-entered data is stored in this browser's local storage. It is not automatically synced to other devices.
- Download a JSON backup before clearing browser storage or changing devices.
- Finance records are manual; this app does not connect to banks or payment apps.
- Website shortcuts open external sites; passwords and authentication tokens are never requested or stored.
- Live currency rates, bank integrations, WhatsApp reminders, Gmail data and social account APIs require separate official integrations and are not represented as active connections.
- Google Fonts are optional styling; if offline, fallback fonts are used.
