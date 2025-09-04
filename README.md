# Idle Hands Tinkering — Site (GitHub → Netlify)

This repo contains your static website. When connected to Netlify, **every push to `main` auto-deploys** your site.

## One-Time Setup (GitHub → Netlify)
1. Create a **new GitHub repo** named `idle-hands-tinkering` (public or private).
2. Upload this folder's contents to that repo (drag/drop on GitHub or use GitHub Desktop).
3. In **Netlify → Add new site → Import from Git**, choose **GitHub** and pick your repo.
4. Build settings:
   - **Build command:** _none_ (leave blank)
   - **Publish directory:** `/` (root)
5. Click **Deploy**. Netlify will build and publish automatically.
6. In your site **Settings → Domain management**, add your custom domain later if you want.

## Making Changes
- Edit files locally or ask Knox (me) to prepare updates.
- Commit and push to `main`:
  - GitHub Desktop: *Commit to main* → *Push origin*.
  - Command line:
    ```bash
    git add -A
    git commit -m "Update gallery/copy"
    git push origin main
    ```
- Netlify will auto-deploy the new version.

## Where things live
- `index.html` — homepage (has Hero, About, Bladesmithing links, **Knife Gallery**, Videos, Contact).
- `assets/` — logos, images, gallery, favicon.
- `styles.css` — site styles.
- `script.js` — slider + lightbox code.
- `netlify.toml` — security headers.
- `README.md` — this file.

## Forms
This site uses **Netlify Forms**. After the first deploy:
- Netlify → **Forms** → select *contact* → **Notifications → Add notification → Email** → set to `Thomknitter@msn.com`.

## Tips
- Image sizes: gallery images are optimized to ~1600px wide for performance. Replace with similar sizes for best speed.
- If you forget to optimize, Netlify still works—page may load slower on mobile.
- To add more photos: drop them in `assets/gallery/` and create matching thumbnails in `assets/gallery/thumbs/` (400px wide).

— Prepared 2025-09-04 by Knox
