# Personal Academic Website (GitHub Pages)

A modern, fast, and responsive academic personal homepage inspired by [adamwang0224.github.io](https://adamwang0224.github.io).

Built with **pure semantic HTML5, modern CSS, and lightweight vanilla JavaScript** — zero build tools, zero Ruby/Jekyll dependencies, and 100% ready to deploy to GitHub Pages with instant local previewing.

---

## 🌟 Key Features

- **Academic Profile Sidebar (Sticky)**:
  - Avatar, full name, research title, affiliation, and location.
  - Social & academic links: Email, Google Scholar, GitHub, X (Twitter), LinkedIn, ORCID.
  - One-click Curriculum Vitae (CV) anchor/download button.
- **Top Navigation Bar**:
  - Smooth scroll to sections: `About`, `News`, `Publications`, `Projects`, `Experience`, `Service`.
  - Responsive mobile drawer menu.
  - Integrated **Dark / Light mode toggle** with auto-detection of system color scheme and localStorage persistence.
- **Rich Publications Section**:
  - Category filters: `All`, `Conferences`, `Preprints`.
  - Paper cards with teaser diagram/thumbnail, title, bolded author highlight, conference venue badges, and abstract.
  - Action pills: `PDF`, `arXiv`, `Code`, `Project Page`.
  - **Collapsible BibTeX snippet** with a **one-click copy button** and toast feedback.
- **Projects Showcase**:
  - Grid cards featuring open-source codebases, PyTorch packages, and tech tags.
- **Timeline for Experience & Education**:
  - Clean vertical timeline displaying degrees, research fellowships, and internships.
- **Academic Service & Honors**:
  - Organized lists for reviewer roles (CVPR, ICCV, NeurIPS, MICCAI) and academic awards.

---

## 🚀 Quick Start (Local Preview)

Because this template uses standard web standards without heavy build dependencies, you can preview it immediately:

### Option 1: Python Built-in Server (Recommended)
Run the following in your terminal:
```bash
# Navigate to this directory
cd /Users/alinr/Desktop/web

# Start a local HTTP server
python3 -m http.server 8000
```
Then open your browser to [http://localhost:8000](http://localhost:8000).

### Option 2: Direct File Open
You can simply double-click `index.html` in Finder or open it in any modern web browser.

---

## 🌐 Deploying to GitHub Pages (3 Simple Steps)

### Step 1: Create your GitHub Pages Repository
1. Log in to [GitHub](https://github.com).
2. Create a **new public repository** named:
   ```
   <your-username>.github.io
   ```
   *(Replace `<your-username>` with your exact GitHub username).*

### Step 2: Push your Files
In your terminal, initialize and push your repository:
```bash
cd /Users/alinr/Desktop/web
git init
git add .
git commit -m "Initial commit: academic personal homepage"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

### Step 3: Verify GitHub Pages
1. Go to your repository on GitHub: `https://github.com/<your-username>/<your-username>.github.io`
2. Navigate to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, ensure it is set to **Deploy from a branch** with branch: `main` and folder: `/ (root)`.
4. Within 1–2 minutes, your website will be live at:
   ```
   https://<your-username>.github.io
   ```

---

## 🛠️ Customization Guide

All personal data and content are organized cleanly in [`index.html`](file:///Users/alinr/Desktop/web/index.html):

### 1. Update Profile & Sidebar Information
Look inside `<aside class="sidebar">` in `index.html`:
- **Avatar Photo**: Replace `assets/images/avatar.svg` with your personal photo (e.g., `assets/images/avatar.jpg`), then update the `<img src="...">` tag.
- **Name & Titles**: Change `Alex Morgan` to your name, and adjust your title/institution.
- **Social Links**: Update the `href` URLs for Google Scholar, GitHub, LinkedIn, Twitter/X, and Email.

### 2. Add or Edit Publications
Look inside `<section id="publications">` in `index.html`:
- Each paper is an `<article class="pub-card" data-category="conference">` (or `data-category="preprint"`).
- Update the title, authors (wrap your name in `<strong>Your Name</strong>` to highlight it), venue, and links.
- Set your paper's BibTeX citation inside the `data-bibtex="..."` attribute of the copy button and inside the `<pre class="bibtex-code"><code>` block.
- Add your paper's teaser image to `assets/images/` and update `<img src="assets/images/your-paper.png">`.

### 3. Update News and Projects
- **News**: Add new entries inside `<div class="news-list">` using `<div class="news-item">`.
- **Projects**: Edit cards inside `<div class="projects-grid">` with your repository names, descriptions, and tags.

### 4. Styles & Customization
- Colors, fonts, and dark mode themes are centralized in [`assets/css/style.css`](file:///Users/alinr/Desktop/web/assets/css/style.css) under CSS variables (`:root` and `[data-theme="dark"]`).
- You can tweak `--accent` (default academic blue `#2563eb`) to match your preferred personal theme color.
# ali1556.gtihub.io
