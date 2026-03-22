# Tortol Website

Static GitHub Pages site for the Tortol app — landing page, features, pricing, support, and privacy policy.

## Pages

| File | URL | Purpose |
|---|---|---|
| `index.html` | `/` | Landing page (hero, screenshots, features, pricing, FAQ) |
| `privacy-policy.html` | `/privacy-policy.html` | Privacy policy (required by App Store & Play Store) |

## How to Deploy on GitHub Pages

1. Create a new GitHub repository named **`tortol-website`**
2. Push this folder's contents to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial website"
   git remote add origin https://github.com/YOUR_USERNAME/tortol-website.git
   git push -u origin main
   ```
3. Go to the repo → **Settings → Pages → Source → Deploy from branch → main / (root)**
4. Click **Save** — site goes live at:
   - `https://YOUR_USERNAME.github.io/tortol-website/`
   - `https://YOUR_USERNAME.github.io/tortol-website/privacy-policy.html`

## Before Publishing

1. **Replace `your@email.com`** in `index.html` and `privacy-policy.html` with your real contact email
2. **Add the app icon** — copy `assets/icon.png` from the main project into the `images/` folder
3. **Add screenshots** — place real app screenshots in the `images/` folder and update `index.html`:
   - Replace each `<div class="screenshot-placeholder">` block with `<img src="images/screenshot-N.png" alt="..." />`
   - Recommended size: 1080×1920 px portrait
4. **Update Play Store / App Store links** — replace `href="#"` on the badge buttons with the real store URLs once the app is live
5. **Update the effective date** in `privacy-policy.html` if needed

## Folder Structure

```
tortol-website/
├── index.html            # Main landing page
├── privacy-policy.html   # Privacy policy
├── css/
│   └── style.css         # All styles (Tortol brand colors)
├── images/
│   ├── icon.png          # ← Copy from assets/icon.png in the app project
│   ├── screenshot-1.png  # ← Add your screenshots here
│   └── ...
└── README.md
```
