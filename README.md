# UPSC Prelims 2027 Tracker

Static site (no build step). Data syncs to Supabase per user; localStorage is the offline cache.

## Deploy
1. **Supabase**: create a project. SQL Editor: paste `schema.sql`, Run.
2. Supabase > Project Settings > API: copy the Project URL and the publishable (anon) key.
   Never use the service_role key in this file.
3. Open `index.html`, replace `YOUR_SUPABASE_URL` and `YOUR_SUPABASE_PUBLISHABLE_KEY`.
4. Supabase > Authentication: for personal use you can turn off "Confirm email" so sign-up works instantly.
   Otherwise set Site URL to your Vercel URL.
5. **GitHub**: push this folder as a repo.
6. **Vercel**: Add New > Project > import the repo. Framework preset: Other. No build command, output directory blank. Deploy.
7. Open the Vercel URL, Sign up once, then Sign in on every device.

Your existing browser data uploads on first sign-in; after that the newest copy wins.
