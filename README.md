# HoopIQ — public website package

This folder is ready for GitHub Pages, Netlify, Cloudflare Pages, or Vercel.

## What is included
- 8 NBA trivia mini-games
- Accounts and persistent scores through Supabase
- Daily / weekly / all-time leaderboards
- Achievement badges
- Weekly featured-game rotation
- Weekly challenge/progress card
- Owner command center
- Mobile-friendly design
- 404 page, robots.txt, and web manifest

## Make it live

### Option A — GitHub Pages
1. Create a GitHub account.
2. Create a new public repository, for example `hoopiq`.
3. Upload every file in this folder to the repository root.
4. In GitHub: **Settings → Pages → Deploy from a branch → main → / (root)**.
5. GitHub will give you a public `github.io` address.

### Option B — Netlify
1. Create a Netlify account.
2. Choose **Add new site → Deploy manually**.
3. Upload this folder.
4. Netlify immediately gives you a public `netlify.app` address.

## Turn on accounts and leaderboards
1. Create a Supabase project.
2. Run `supabase.sql` in Supabase SQL Editor.
3. Open `index.html`.
4. Replace `YOUR_SUPABASE_URL` and `YOUR_SUPABASE_ANON_KEY`.
5. Upload the changed file again.
6. Create your first HoopIQ account.
7. In Supabase, set that account's `profiles.is_owner` to true using its UUID.

Only use the public Supabase anon key in the browser. Never expose the Supabase service_role key.

## Custom domain
After the site is live, buy a domain from a registrar and connect its DNS to your hosting provider. Your final URL can then be something like `hoopiq.example`.

## Important
I cannot publish into your GitHub/Netlify/Supabase accounts from this chat because those accounts require your own login and authorization. The package is prepared so the remaining publishing steps are account-side.
