# Weihao Wu — Personal Portfolio

A modern, minimal personal portfolio website built as a single HTML file. No build tools, no frameworks, no dependencies to install — just open `index.html` in a browser or deploy it anywhere static files are served.

---

## Folder Structure

```
portfolio/
├── index.html      ← The entire site (HTML + CSS + JS inline)
└── README.md       ← This file
```

That's it. One file. Ready to deploy.

---

## Customization Checklist

Before deploying, swap out any remaining placeholder values:

| Location in `index.html`         | What to change                                              |
|----------------------------------|-------------------------------------------------------------|
| `<title>` tag                    | Your name and tagline                                       |
| `<meta name="description">`      | Your personal description                                   |
| Hero `[YOUR GITHUB URL]`         | Already set — verify links point to the right profiles      |
| Project GitHub links             | Replace `https://github.com/WeihaoWu30` with specific repos |
| "Live Demo" buttons              | Add live demo URLs if projects are deployed                 |
| Hero stats                       | Update numbers as you gain more experience                  |
| Footer copyright year            | Update to current year                                      |

---

## Deploy for Free on GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `your-username.github.io` (e.g. `WeihaoWu30.github.io`)  
   **This exact naming is required** for a user page at `https://your-username.github.io`
3. Set visibility to **Public**
4. Click **Create repository** — do NOT initialize with a README

### Step 2 — Push the portfolio files

Open a terminal in your `portfolio/` folder and run:

```bash
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### Step 3 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Branch: `main` / Folder: `/ (root)`
5. Click **Save**

### Step 4 — Wait ~60 seconds, then visit your live site

Your portfolio will be live at:
```
https://YOUR_USERNAME.github.io
```

GitHub Pages builds automatically on every push to `main`, so any future updates are live within ~30 seconds of `git push`.

---

## Updating Your Site

Make changes to `index.html`, then:

```bash
git add .
git commit -m "Update projects section"
git push
```

Done — GitHub Pages picks it up automatically.

---

## Deploying Elsewhere (Alternatives)

| Service         | How                                                                 | Cost    |
|-----------------|---------------------------------------------------------------------|---------|
| **Netlify**     | Drag the `portfolio/` folder to [app.netlify.com/drop](https://app.netlify.com/drop) | Free   |
| **Vercel**      | `npx vercel` in the folder, follow prompts                          | Free    |
| **Cloudflare**  | Connect GitHub repo in Pages dashboard, build command: none         | Free    |

---

## Tech Stack

- Pure HTML5 + CSS3 + Vanilla JS
- [Cabinet Grotesk](https://www.fontshare.com/fonts/cabinet-grotesk) + [Satoshi](https://www.fontshare.com/fonts/satoshi) via Fontshare CDN
- [Font Awesome 6](https://fontawesome.com) via CDN for icons
- CSS custom properties for theming (light/dark mode)
- `IntersectionObserver` for scroll animations
- Zero runtime dependencies — no npm, no bundler, no frameworks
