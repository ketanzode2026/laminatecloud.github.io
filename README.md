# Laminate Cloud - Landing Page Showcase

This repository contains the landing page codebase for **[Laminate Cloud](https://laminatecloud.com)**.

## 🛡️ SEO & Canonical Protection

Because this repository is hosted under `*.github.io`, duplicate content protections are actively configured to protect the primary domain (`https://laminatecloud.com`) from search engine indexing conflicts:

1. **`robots.txt`**: Configured with `Disallow: /` to block web crawlers from indexing this mirror.
2. **Meta Robots**: Set to `noindex, nofollow, noarchive, nosnippet` in `index.html`.
3. **Canonical Link**: Always points directly to `https://laminatecloud.com/`.
4. **Auto-Redirect**: An embedded script redirects any traffic landing on `*.github.io` directly to `https://laminatecloud.com/`.

---

### Deploying to Production Domain (Custom Domain)
If this landing page is ever migrated or served directly from the official custom domain (`https://laminatecloud.com`):
1. In `index.html`, update the robots meta tag to:
   ```html
   <meta name="robots" content="index, follow, max-image-preview:large, max-snippet:-1, max-video-preview:-1">
   ```
2. Update `robots.txt` on the server to allow indexing:
   ```txt
   User-agent: *
   Allow: /
   Sitemap: https://laminatecloud.com/sitemap.xml
   ```
