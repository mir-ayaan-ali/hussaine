# Ayaan — GitHub Pages (Jekyll) Starter

Clean & minimal blog with 4 categories (Nohas, Bravo, Charlie, Delta), search, dark mode, SEO, RSS, and featured posts.

## Quick Deploy (Project Pages)
1. Create a repo named **`hussaine`** under your GitHub account `mir-ayaan-ali`.
2. Upload all files from this folder to the repo root and commit to the **main** branch.
3. In **Settings → Pages**, set:
   - **Source**: Deploy from branch
   - **Branch**: `main` / `/ (root)`
4. Your site will publish at **https://mir-ayaan-ali.github.io/hussaine/**.

> If your account uses a different name or repo, update `_config.yml` `url` and `baseurl` accordingly.

## How to add a new post
Create a file in `_posts/` named `YYYY-MM-DD-your-title.md` with front matter like:

```yaml
---
title: "Your Post Title"
date: 2025-08-27
categories: [nohas]   # or bravo/charlie/delta
author: taylor_swift  # or ed_sheeran / michael_jackson / adele
featured: true        # set to true to appear on homepage Featured grid
summary: "Short one-line summary for cards and social."
---
Your content in **Markdown**. You can include code, lists, images, etc.
```

## Customize
- **Colors/Theme**: edit `assets/css/styles.css` (CSS variables at top).
- **Tagline/Meta**: edit `_config.yml` and homepage hero in `_layouts/home.html` (subtext).
- **Navigation**: update links in `_layouts/default.html` if needed.
- **Authors**: edit `_data/authors.yml`.
- **Favicon**: replace `assets/favicon.svg`.

## Features
- 4 category pages: `/nohas/`, `/bravo/`, `/charlie/`, `/delta/`
- Featured posts section (8 slots by default)
- Search (client-side, no backend)
- Dark mode toggle (remembers preference)
- SEO (`jekyll-seo-tag`), RSS (`/feed.xml`), Sitemap (`/sitemap.xml`)
- Accessible, responsive, fast by default
