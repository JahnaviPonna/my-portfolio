# Jahnavi Ponna — Portfolio

Modern dark portfolio with glassmorphism, gradient UI, smooth animations, and full resume content.

## Project Structure

```
jahnavi-portfolio/
├── index.html              ← Entire site (all CSS + JS inline)
├── Jahnavi_Resume.pdf      ← Your resume (linked in nav + contact)
├── my_img.jpg              ← Your profile photo (add this!)
├── vercel.json             ← Vercel deployment config
├── .gitignore
└── README.md
```

## Add Your Profile Photo

Place your photo as `my_img.jpg` in the root of this folder.
The site already points to it — no code changes needed.
(Currently falls back to your GitHub Pages photo if missing.)

## Deploy to Vercel

### Option A — GitHub + Vercel Dashboard (Recommended)

1. Create a new GitHub repo (e.g. `jahnavi-portfolio`)
2. Push this folder:
   ```bash
   git init
   git add .
   git commit -m "initial portfolio"
   git remote add origin https://github.com/YOUR_USERNAME/jahnavi-portfolio.git
   git push -u origin main
   ```
3. Go to https://vercel.com → New Project → Import your repo
4. Leave all settings default → Deploy
5. Live at `https://jahnavi-portfolio.vercel.app` ✅

### Option B — Vercel CLI

```bash
npm install -g vercel
cd jahnavi-portfolio
vercel
# Follow prompts → live URL in ~30 seconds
```

### Option C — GitHub Pages (existing)

Just replace your current `index.html`. Move `Jahnavi_Resume.pdf` into the repo root too.

## Custom Domain

Vercel Dashboard → your project → Settings → Domains → add your domain.

## Customizations

| What | Where |
|---|---|
| Accent colors | `:root` → `--a1` `--a2` `--a3` |
| Hero stats | `.hstat-num` values in `#hero` |
| Profile photo | Replace `my_img.jpg` |
| Resume file | Replace `Jahnavi_Resume.pdf` |
| Project links | Each `<a class="pc">` href |
