# Deploying Starter Bank

## GitHub Pages

1. Push this folder to a repo (e.g. `Demo-Banking-Application` or `Starter-Bank`).
2. **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main** → Save.
3. Open `https://<username>.github.io/<repo-name>/` (use the **trailing slash** or `index.html`).

The app uses a dynamic base URL so login, dashboard, CSS, and JS work correctly on the repo subpath.

## Vercel / Netlify

- Drag-and-drop this folder or connect the same GitHub repo.
- Always use the **HTTPS** URL they give you (e.g. `https://your-app.vercel.app`).

## Chrome "Dangerous" or "Not safe" warning

- **Cause:** New or low-traffic domains are sometimes flagged by Chrome’s Safe Browsing until they build reputation.
- **What to do:**
  - Use the **HTTPS** link (not `http://`). The project uses relative paths and works over HTTPS.
  - In Chrome you can use “Visit this unsafe site” / “Details” → “Visit site” (only if you know and trust the deployment).
  - Edge and other browsers often don’t show the same warning for the same URL.
- **Optional:** Connect a custom domain (e.g. your own domain) on Vercel/Netlify; established domains are less likely to be flagged.
