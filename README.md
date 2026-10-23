# Full-Stack Gym

A hands-on full-stack course: lessons, try-its, questions and auto-checked coding drills.
Plain HTML, CSS and JavaScript in one file (`index.html`), with Supabase for accounts and saved progress.

## Files
- `index.html` — the whole app
- `config.js` — Supabase URL and anon key (public by design; security comes from the policies)
- `supabase.sql` — creates the `progress` table and its row-level security policies

## Run locally
Open `index.html` in a browser, or run `npx serve .` and open the printed address.
Without values in `config.js` it runs without accounts and saves progress in the browser.

## Set up accounts (Supabase)
1. Create a free project at supabase.com.
2. SQL Editor → paste `supabase.sql` → Run.
3. Project Settings → API: copy the Project URL and the `anon` public key into `config.js`.
4. Authentication → URL Configuration: set Site URL to your Vercel address.

## Deploy (Vercel)
Push this folder to GitHub, then on vercel.com: Add New → Project → import the repo → Deploy.
No build step; Vercel serves the files as they are.
