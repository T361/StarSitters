# Star Sitters — Admin Dashboard

Admin web dashboard for **Star Sitters**, a childcare/babysitting booking platform.
Built with Next.js (App Router) and Supabase as the backend-as-a-service layer
(Postgres, auth, row-level security).

## Stack

- **Next.js** (TypeScript, App Router)
- **Supabase** — Postgres database, authentication, and role-based access control
- Role provisioning uses Postgres RLS with an explicit immutability-bypass flag for
  controlled admin-role grants, rather than trusting client-supplied role claims

## Contents

- `starsitters-admin/` — the Next.js admin application

## Run

```bash
cd starsitters-admin
cp .env.local.example .env.local   # set Supabase URL + anon key + service role key
npm install
npm run dev
```

See `starsitters-admin/README.md` for first-admin-user provisioning details.
