<!--
Create a repo named exactly like your GitHub username (e.g. jordanglass21/jordanglass21), public,
and put this in as README.md. Swap in your name/links below.
-->

### Jordan Glass

[LinkedIn](https://linkedin.com/in/jordan-glass-one) · [jordanglass421@gmail.com](mailto:jordanglass421@gmail.com) · [Resume](https://raw.githubusercontent.com/jordanglass21/jordanglass21/main/glass_resume.pdf)

Full Stack engineer with production experience shipping TypeScript/NestJS services and APIs. Before software, I ran operations for a business. I like building things people actually use and that make their life a little easier.

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

<img width="656" height="817" alt="Screenshot 2026-09-09 at 5 07 16 PM" src="https://github.com/user-attachments/assets/7356b9ef-eb6b-484f-a33a-5107cff99573" />

---

### ASL Drill

A typing test for ASL fingerspelling. Fingerspell a word to your webcam and it grades each letter in real time, then shows your letters per minute and accuracy. Everything runs in the browser, so video never leaves your device.

[asldrill.jordanglass.dev](https://asldrill.jordanglass.dev) · [Repo](https://github.com/jordanglass21/asl-drill)

- Hand tracking with MediaPipe, with letters read by a small neural net I trained in Python and run in plain TypeScript (no ML runtime)
- All 26 letters: 24 static handshapes from the classifier, plus J, Z, and double letters (the OO in BOOK) from a separate motion detector
- 96% accuracy on held-out recordings, cross-validated by take rather than by frame to avoid leakage
- Results page with per-letter timing, most-missed letters, and personal bests

**Stack:** Next.js · React · TypeScript · Tailwind · MediaPipe · Python (scikit-learn) · Vercel

Python and TypeScript test against shared JSON fixtures, so training and the app compute identical features and predictions. Hold, session, motion, and stats logic are pure reducers, tested without a camera using recorded hand-landmark data. 315 Jest and 39 pytest tests run in CI on every PR.

<img width="1109" height="815" alt="Screenshot 2026-10-29 at 8 28 38 PM" src="https://github.com/user-attachments/assets/cbcf6be9-6af5-450c-8ea0-aeeb4555e146" />
