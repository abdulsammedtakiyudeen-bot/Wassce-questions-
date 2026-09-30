# WASSCEPASSCO

Mobile-first WASSCE preparation PWA for GitHub Pages.

## Included now
- All 11 PDFs from the supplied WASSCE-Study1 source ZIP.
- Real PDF Open + Download buttons.
- Search and filters.
- Per-account local demo sign-up/sign-in with fresh 0% progress.
- Google login button ready for Supabase OAuth.
- PWA manifest + service worker.
- Study-resource upload spaces for future Chief Examiners’ Reports, guides, Do’s & Don’ts and Super Mocks.
- Supabase-ready cloud authentication, resource database and admin upload interface.
- Privacy/Terms pages and AdSense-ready reserved space can be added without changing auth logic.

## GitHub Pages
Upload the contents of this folder to the `main` branch and enable GitHub Pages from `main` / root. No GitHub Actions workflow is required.

## Supabase backend
1. Create a Supabase project.
2. Run `sql/schema.sql`.
3. Create the `wassce-resources` Storage bucket and suitable public-read/admin-write policies.
4. Put your Supabase project URL and anon/publishable key in `config.js`.
5. Put authorized admin emails in `ADMIN_EMAILS`.
6. Enable Google OAuth in Supabase if you want Google sign-in.

Do not place a Supabase service-role key in this repository.
