# Tampa Sprinkler Repair — Water Oak Irrigation

Marketing and lead-generation website for Water Oak Irrigation, serving the greater Tampa, FL area (sprinkler repair, irrigation install/design, drainage solutions, sod, and well-pump service across Westchase, Carrollwood, Lutz, Wesley Chapel, Hyde Park, Davis Island, and more).

## Tech stack

This is a static website built with plain HTML and image assets. There is no build step — every page is a self-contained `.html` file served directly.

## Hosting & deployment

The site is hosted on Netlify and deploys automatically from the `main` branch. Netlify configuration lives in `netlify.toml`:

- `publish = "."` — the site is served from the repository root, so file/asset paths are relative to root. Moving files into subfolders will break links unless references are updated.
- - Netlify Forms are enabled (`[forms] store = true`) to capture customer service requests.
 
  - Preview changes locally by opening any `.html` file in a browser, or use a simple static server (e.g. `npx serve .`).
 
  - ## Project layout
 
  - - `index.html` — homepage
    - - `*.html` — individual service and location landing pages
      - - Image assets (`.jpg`, `.jpeg`, `.png`, `.webp`) live in the repo root
        - - SEO / infra files: `sitemap.xml`, `robots.txt`, `_redirects`, `llms.txt`, `favicon.ico`, and search-engine verification files (`BingSiteAuth.xml`, `google*.html`)
         
          - ## Contributing
         
          - Changes are made via pull requests against `main`; merging to `main` triggers a Netlify deploy.
          - 
