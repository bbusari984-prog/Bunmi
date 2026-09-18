# Barakat Busari — Book Editing & Ghostwriting Website

A single-page, SEO/AEO/GEO-optimized portfolio website for **Barakat Busari**, a professional book editor and fiction ghostwriter, built to be hosted for free with **GitHub Pages** and linked from an Upwork profile.

## 🎨 Design

- **Brand palette:** Bordeaux (`#5c0f1e`, `#3d0a14`) mixed with warm cream (`#f7f0e3`, `#fbf6ea`) and a gold accent (`#c8a15c`) — a literary, editorial, high-end feel.
- **Typography:** Playfair Display (serif, headings) paired with Jost (sans-serif, body) via Google Fonts.
- Fully responsive layout with a mobile slide-out navigation drawer, animated hover states, accordion FAQ, and a dedicated contact block.
- Single self-contained `index.html` file — all CSS and JavaScript are inlined, so there is nothing else to configure.

## 📄 Files in this repository

| File | Purpose |
|---|---|
| `index.html` | The full website (structure, styling, and interactivity in one file). |
| `sitemap.xml` | XML sitemap listing the page's sections for search engine crawlers. |
| `robots.txt` | Crawler rules pointing search engines and AI crawlers to the sitemap. |
| `README.md` | This file. |

## 🔍 SEO / AEO / GEO Features

This site is built with **three layers of discoverability** in mind:

- **SEO (Search Engine Optimization):** semantic HTML5, descriptive `<title>` and `<meta name="description">`, keyword-relevant headings, canonical URL tag, Open Graph and Twitter Card meta tags, and a submitted `sitemap.xml` + `robots.txt`.
- **AEO (Answer Engine Optimization):** an on-page, visually accordion-based **FAQ section** is mirrored in machine-readable `FAQPage` JSON-LD structured data, so voice assistants and AI answer engines (Google AI Overviews, Bing Copilot, ChatGPT browsing, Perplexity, etc.) can extract direct question-and-answer pairs.
- **GEO (Generative Engine Optimization):** `ProfessionalService` and `Person` JSON-LD schema describe the service type, service area, and contact details in a structured format that generative AI systems can cite directly when recommending an editor or ghostwriter, plus `geo.region` / `geo.placename` meta tags for locale signals.

## 🚀 How to publish with GitHub Pages

1. Create a new **public** GitHub repository (e.g. `barakat-editing` or `<your-username>.github.io` for a root domain).
2. Upload all four files in this folder to the root of that repository (drag-and-drop works fine on github.com, or use `git add . && git commit -m "Launch website" && git push`).
3. In the repository, go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and `/ (root)` folder, then click **Save**.
5. GitHub will publish your site at either:
   - `https://<your-username>.github.io/<repository-name>/` (project repo), or
   - `https://<your-username>.github.io/` (if the repo is named exactly `<your-username>.github.io`).
6. Wait 1–2 minutes, then visit the URL to confirm it's live.

### Before you publish — update these placeholders

Open `index.html`, `sitemap.xml`, and `robots.txt` and replace every instance of:

```
https://bbusari984-prog.github.io/Oluwabunmi-/
```

with your actual GitHub Pages URL once you know it (repository name included, if applicable).

Optional but recommended: add a real `assets/og-cover.jpg` image (1200×630px) to the repository and update the `og:image` / `twitter:image` tags in `index.html` so link previews on WhatsApp, LinkedIn, and social media show a proper cover image instead of a broken link.

## ✏️ Customizing content

Everything is in `index.html`. Useful anchors to search for and edit directly:

- **Hero headline & subtext** — inside `<section class="hero">`
- **Services & pricing** — inside `<section id="services">` (`.service-card` blocks)
- **About / bio / stats** — inside `<section id="about">`
- **Process steps** — inside `<section id="process">`
- **Testimonials** — inside `<section id="testimonials">` (replace placeholder quotes with real client feedback once you have permission to publish it)
- **FAQ** — inside `<section id="faq">`; each `<details>` block is one question. Keep the matching `FAQPage` JSON-LD block near the top of the file in sync with any wording changes.
- **Contact details** — WhatsApp and email appear in the `<section id="contact">` block and in the footer.

## 📞 Contact details used on this site

- **WhatsApp:** +234 813 164 2111
- **Email:** busaribaraka1@gmail.com

## 🛠 Tech stack

Pure HTML5, CSS3, and vanilla JavaScript — no build step, no dependencies, no frameworks. Works on any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages) with zero configuration.

## 📈 Recommended next steps

- Submit the sitemap URL to [Google Search Console](https://search.google.com/search-console) and [Bing Webmaster Tools](https://www.bing.com/webmasters) after publishing.
- Replace placeholder testimonials with real, permissioned client reviews as they come in.
- Add a custom domain (optional) via **Settings → Pages → Custom domain** in your GitHub repository, and update the `canonical`, `og:url`, and sitemap URLs to match.
