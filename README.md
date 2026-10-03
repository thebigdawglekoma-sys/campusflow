# CampusFlow

Student productivity web app MVP for South African university students.

## Stack
- Next.js App Router
- Supabase Auth + Postgres + Row Level Security
- TypeScript
- CSS (no UI framework dependency)

## Run locally
1. Install Node.js.
2. `npm install`
3. Copy `.env.example` to `.env.local` and add your Supabase URL + publishable key.
4. Create a Supabase project and run `supabase/schema.sql` in the SQL Editor.
5. In Supabase Auth settings, set the Site URL to `http://localhost:3000`.
6. Configure the confirmation email redirect to `http://localhost:3000/auth/confirm`.
7. `npm run dev`
8. Open `http://localhost:3000`.

## Production
Deploy the repository to a Next.js-compatible host such as Vercel, set the same environment variables, and update Supabase Auth Site URL/redirect URLs to the production domain.

## Important
The app is wired for real authentication and database-backed student records, but payment processing is intentionally not connected yet. Add the chosen South African payment provider before accepting real money.
