# Deploy SystemLab

## Deploy to Vercel

1. Open https://vercel.com/new and sign in with GitHub.
2. Import `riddhiroy/systemlab`.
3. Keep the detected framework as **Vite**.
4. Build command: `npm run build`.
5. Output directory: `dist`.
6. No environment variables are required for the current local-first MVP.
7. Click **Deploy**. Vercel will provide the public URL and deploy future pushes to `main` automatically.

## Local development

```bash
npm install
npm run dev
```

## Current MVP boundaries

- Architecture diagrams and edits run in the browser.
- Save/load uses this browser's local storage; it is not synced across devices.
- Simulation is a transparent educational approximation using configured component capacity, replica count, and latency.
- Supabase schema is provided in `supabase/schema.sql`, but authentication and cloud persistence are not connected yet.
- No payment processing or premium entitlements are enabled.
