<!--
Create a repo named exactly like your GitHub username (e.g. jordanglass21/jordanglass21), public,
and put this in as README.md. Swap in your name/links below.
-->

### Jordan Glass

[LinkedIn](https://linkedin.com/in/jordan-glass-one) · [jordanglass421@gmail.com](mailto:jordanglass421@gmail.com)

Backend engineer with production experience shipping TypeScript/NestJS services and APIs. Before software, I ran operations for a business — I like building things people actually use and that make their life a little easier.

More projects coming soon.

---

### Shopping List

A grocery list web app that turns recipes into shopping lists, sorts items by supermarket aisle, and syncs across devices.

[list.jordanglass.dev](https://list.jordanglass.dev/) · [Repo](https://github.com/jordanglass21/shopping-list)

- Paste a recipe, get parsed shopping items with a review step before anything's added
- Auto-categorizes items by supermarket aisle
- Saves lists for reuse, tracks checked-off items with a running count
- Google sign-in with magic-link fallback

**Stack:** Next.js · TypeScript · Tailwind · Supabase (Postgres, RLS) · Vercel

Data access is enforced with row-level security at the database, not just in app code. Data logic lives in custom hooks, keeping components presentational. Schema is version-controlled through Supabase migrations.
