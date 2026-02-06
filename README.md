# Wild Lotus Management

A clean, professional website for Wild Lotus Management—an adult content creator management company run by women, open to male and female clients from all walks of life.

## Colors & Brand
- **White** – body text and clarity
- **Black** – background and contrast
- **Gold** – accents, headings, and CTAs (aligned with logo)

## Pages
- **Home** – Hero, platforms, services overview, 3 testimonials with case studies, CTA
- **About** – Company story, values, who we work with
- **Services** – Full-scale management, account management & chatting, brand development, consultations
- **Blog** – Blog listing (placeholder posts; you can add real posts later)

## How to View
Open `index.html` in a browser, or run a simple local server:

```bash
# Python 3
python -m http.server 8000

# Then visit http://localhost:8000
```

## Structure
```
wildlotus/
├── index.html      # Home
├── about.html      # About
├── services.html   # Services
├── blog.html       # Blog
├── css/
│   └── styles.css  # Shared styles
├── assets/
│   └── logo.png    # Logo
└── README.md
```

Replace blog post `#` links with real article URLs when you add individual blog posts.

---

## Deploy with Vercel & GitHub

The project is ready for Git. Follow these steps to publish and get previews.

### 1. Create a GitHub repository

1. Go to [github.com/new](https://github.com/new).
2. Name the repo (e.g. `wildlotus` or `wild-lotus-management`).
3. Choose **Public**.
4. **Do not** add a README, .gitignore, or license (the project already has them).
5. Click **Create repository**.

### 2. Push your code to GitHub

In a terminal, from the `c:\wildlotus` folder, run (replace `YOUR_USERNAME` and `YOUR_REPO` with your GitHub username and repo name):

```powershell
cd c:\wildlotus
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git branch -M main
git push -u origin main
```

Example: if your repo is `https://github.com/jane/wildlotus`, use:

```powershell
git remote add origin https://github.com/jane/wildlotus.git
git branch -M main
git push -u origin main
```

### 3. Deploy with Vercel

1. Go to [vercel.com](https://vercel.com) and sign in (use **Continue with GitHub** if you have a GitHub account).
2. Click **Add New…** → **Project**.
3. **Import** the GitHub repo you just created (e.g. `wildlotus`).
4. Vercel will detect it as a static site. Leave the defaults:
   - **Framework Preset:** Other
   - **Root Directory:** ./
   - **Build Command:** (leave empty)
   - **Output Directory:** ./
5. Click **Deploy**.

After the build finishes, you’ll get:

- **Production URL** – e.g. `https://wildlotus.vercel.app` (or your custom domain if you add one).
- **Preview URLs** – every push to a branch (e.g. a new branch or PR) gets its own preview link.

### 4. Optional: custom domain

In the Vercel project: **Settings → Domains** → add your domain and follow the DNS instructions.
