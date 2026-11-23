# 📰 The Daily Pulse — Modern News & Magazine Website

> An independent digital news and magazine publication website built with pure semantic **HTML5** and **CSS3 Flexbox**. Designed for a First-Year B.Tech CSE Web Development Project.

---

## 🌐 Live Demo & Repository
- **Live Website**: `https://<your-username>.github.io/<your-repo-name>/` *(Replace with your GitHub Pages link)*
- **GitHub Repository**: `https://github.com/<your-username>/<your-repo-name>`

---

## 📌 Project Overview
**The Daily Pulse** is a responsive digital newspaper layout inspired by traditional broadsheet journalism (like *The New York Times* and *The Guardian*) combined with clean, modern web standards.

### Key Objectives Achieved:
1. **100% Pure HTML5 & CSS3**: No JavaScript, no Bootstrap, no external frameworks, and no CSS Grid.
2. **Mastery of Flexbox**: Every layout component (top bar, navbar, lead stories, category strip, featured cards, two-column 70/30 layout, sidebar widgets, author cards, and footer) is crafted using Flexbox.
3. **Editorial Newspaper Aesthetic**:
   - Classic serif masthead and headlines using Google Fonts (**Playfair Display**).
   - High-readability sans-serif body text using Google Fonts (**Inter**).
   - Crisp white paper background, dark charcoal text, and an editorial crimson accent (`#b30000`).
   - Defined cleanly via CSS Custom Properties (`:root` variables).
4. **Interactive Hover Effects**: Micro-interactions on article cards (subtle elevation lift), headlines (color transitions), and buttons using pure CSS transitions.
5. **Full Mobile Responsiveness**:
   - Desktop view (> 1024px): 70% main news column + 30% sidebar.
   - Tablet view (768px): Fluid adaptations.
   - Mobile view (360px - 768px): The two-column layout stacks vertically, moving the sidebar cleanly below the main news feed.
6. **Accessible & Semantic**: Uses `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>` with descriptive image `alt` tags and ARIA labels.

---

## 📁 Folder Structure

```text
magazine-website/
│
├── index.html       # Semantic HTML5 structure (commented for viva)
├── style.css        # Pure CSS3 Flexbox stylesheet with media queries
└── README.md        # Project documentation & deployment guide
```

---

## 🚀 How to Run Locally

### Option 1: Direct File Open (Simplest)
1. Navigate to the project directory on your computer:
   `c:\Users\HARSHA\OneDrive\Documents\web development projects\magazine website`
2. Double-click `index.html` to open it in your default web browser (Chrome, Edge, Firefox, Brave).

### Option 2: Using VS Code Live Server
1. Open the project folder in **Visual Studio Code**.
2. If installed, right-click `index.html` and select **"Open with Live Server"**.
3. The site will run at `http://127.0.0.1:5500/index.html`.

---

## 📤 Step-by-Step GitHub & GitHub Pages Deployment Guide

Follow these exact steps to upload your project to GitHub and deploy it on **GitHub Pages** before the 24 November deadline.

### Step 1: Create a New GitHub Repository
1. Log in to your account at [GitHub.com](https://github.com).
2. In the top-right corner, click the **`+`** icon and select **New repository**.
3. Name your repository (e.g. `daily-pulse-newspaper` or `magazine-website`).
4. Set visibility to **Public** (required for free GitHub Pages).
5. **Do NOT** check "Add a README file" (we already created one).
6. Click **Create repository**.

---

### Step 2: Upload Files via Git CLI or Web Browser

#### Method A: Using Git in Terminal (Recommended)
Open your terminal (PowerShell or Git Bash) inside this project folder:
```bash
# 1. Initialize a git repository
git init

# 2. Stage all files (index.html, style.css, README.md)
git add .

# 3. Create initial commit
git commit -m "Initial commit: Complete News & Magazine website with pure Flexbox"

# 4. Set default branch to main
git branch -M main

# 5. Connect to your GitHub repository (replace with your repo URL)
git remote add origin https://github.com/<your-username>/<your-repo-name>.git

# 6. Push code to GitHub
git push -u origin main
```

#### Method B: Uploading Directly Through GitHub Webpage
1. On your newly created GitHub repository page, click the link: **"uploading an existing file"**.
2. Drag and drop `index.html`, `style.css`, and `README.md` into the box.
3. Write a commit message like `Add project files`.
4. Click **Commit changes**.

---

### Step 3: Turn on GitHub Pages (Hosting)
1. In your GitHub repository, click on the **Settings** tab (gear icon at the top).
2. In the left sidebar, click on **Pages** (under the "Code and automation" section).
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Click the dropdown, select `main`, and keep folder as `/ (root)`.
   - Click **Save**.
4. Wait about 1 to 2 minutes. Refresh the page.
5. You will see a banner:
   > *"Your site is live at `https://<your-username>.github.io/<your-repo-name>/`"*
6. Click the link to test your live website!

---

## 🎓 College Viva & Interview Guide (First-Year CSE)

When presenting this project to your professor or viva examiner, here is how you can explain your technical decisions:

### Q1: Why did you use Flexbox instead of CSS Grid or Floats?
> **Answer**: *"Flexbox is an efficient 1D layout model designed to distribute space dynamically along an axis. Floats are an outdated technique that require clearfix hacks, whereas CSS Grid is best suited for complex 2D coordinate layouts. For this magazine website, Flexbox offered clean control over item alignment, row wrapping, equal-height cards (`align-items: stretch`), and responsive stacking on mobile screens."*

### Q2: How did you implement the 70/30 two-column layout?
> **Answer**: *"We wrapped the latest news and the sidebar in a flex container (`display: flex`). The main news section is assigned `flex: 7` (~70% width) and the sidebar is assigned `flex: 3` (~30% width). In our media query for screens below 768px, we set `flex-direction: column` and `flex: none; width: 100%`, causing the sidebar to cleanly stack beneath the main news."*

### Q3: Why are CSS Variables (`:root`) used?
> **Answer**: *"CSS Variables allow us to define our color palette, typography, and spacing scale in one single place. This prevents hardcoded hex values, guarantees design consistency across all components, and makes future theme changes effortless."*

### Q4: Why is semantic HTML important here?
> **Answer**: *"Semantic tags like `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>` give structural meaning to web content. This improves accessibility for screen readers, enhances SEO, and creates clean, self-documenting code."*

---

## 📜 License & Academic Integrity
Created for educational purposes by a First-Year B.Tech Computer Science student. All images sourced under the free Unsplash license.
