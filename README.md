# Abu Bakar Siddik — Academic Research Homepage

A minimal, static, research-focused website for PhD applications. No build system, dependencies, paid services, backend, or external fonts are required; the printable CV uses a single built-in browser print action. Hosted for free with GitHub Pages.

## Files

```text
siddik-abu-bakar.github.io/
├── index.html             # Research homepage: EDIT THIS to update content
├── styles.css             # Homepage colors, typography, layout, responsive styles
├── cv.html                # Printable academic CV: keep aligned with index.html
├── cv.css                 # CV screen/print styles
├── assets/
│   ├── headshot.jpg       # Your supplied, unedited professional portrait
│   ├── favicon.svg       # Browser tab icon
│   ├── apple-touch-icon.png
│   └── og-card.png        # Social sharing preview
├── robots.txt
├── sitemap.xml
├── .nojekyll              # Tell GitHub Pages to serve static files directly
└── README.md
```

## Publish with GitHub Pages (browser, no terminal required)

1. Sign in to the GitHub account **siddik-abu-bakar**.
2. Create a **public** repository named **`siddik-abu-bakar.github.io`** (exact spelling).
3. Use **Add file → Upload files** to upload the **contents of this folder**, not the folder itself. Keep `index.html`, `styles.css`, `cv.html`, and `cv.css` at the repository root. Upload the entire `assets` folder as well.
4. Commit the files on the `main` branch. GitHub's browser upload normally preserves folders when dragged in as a complete directory, but confirm the final repository file tree matches the list above.
5. Go to **Settings → Pages → Build and deployment**, select **Deploy from a branch**, branch **main**, and folder **/(root)**, then click **Save**.
6. Visit **https://siddik-abu-bakar.github.io/** after GitHub completes its Pages deployment. Check the **Actions** tab or **Settings → Pages** for status. Changes can take several minutes to appear.

This specific user-site URL depends on repository ownership and name matching the actual GitHub username.

## Local preview

Open `index.html` directly in a browser. All styles and assets use relative URLs. To preview from a local HTTP server (optional):

```bash
python3 -m http.server 8000
```

Visit `http://localhost:8000/`.

## Update information

- **Introduction/research interests:** In `index.html`, edit the `hero` and `interests` sections.
- **Current research:** Edit `section id="research"`; update study scope and claims only when accurately supported. Do not present future plans as completed work.
- **Add publication:** Duplicate one `<li class="publication">...</li>` in `section id="publications"` and update number, authors, title, venue, year, and verified link (if available). Preserve actual author order.
- **Add research project or PhD affiliation:** Edit `section id="projects"` and the top profile information; distinguish individual contributions from team work.
- **CV:** Independently update `cv.html` with the same factual changes. Open `cv.html` and choose **Print / Save as PDF** to produce an actual PDF for application uploads.
- **Research introduction video:** Update or remove the link in `section id="contact"`.
- **Last updated:** Change the footer in `index.html`, the end note in `cv.html`, and `<lastmod>` in `sitemap.xml` as appropriate.
- **Design:** Edit the CSS variables at the top of `styles.css`.

### Your current profile photo

Your uploaded portrait has already been added **without changing your face** as `assets/headshot.jpg`. It is displayed in its original square aspect ratio inside a subtle frame. To update the photo later, replace `assets/headshot.jpg` with another image of the same name (or update the `src` in `index.html`).

### Change colors, text sizes and icons

- Edit the `:root` color variables in `styles.css` to modify the navy, teal, and gold palette.
- The homepage has larger reading text than the original version, with a smaller hero name.
- Academic icons are defined in an inline SVG sprite in `index.html`; no icon library or CDN is required.
- Your ORCID profile is linked in the hero, contact section, CV, and structured metadata. Its public URL is `https://orcid.org/0009-0007-3658-9194`.

### Replace the CV with your own PDF later (optional)

The provided `cv.html` already works and is printable. If you prefer to link directly to a PDF, place your verified PDF in `assets/Abu_Bakar_Siddik_CV.pdf` and change all `href="cv.html"` to `href="assets/Abu_Bakar_Siddik_CV.pdf"` in `index.html`. Do not change this until the PDF exists.

## Before sending to professors

- Check accuracy of affiliations, dates, titles, and publications (especially venue and publication status).
- Check every academic link and the research-introduction video.
- Confirm the monogram is acceptable or replace it with a real photo.
- Open the site on a phone and desktop.
- Open `cv.html` and print to PDF, checking page breaks.
- Check that your GitHub profile, Google Scholar and ORCID links match the URLs included in applications.

## Design notes

Academic editorial layout: off-white background, deep navy typography, teal with sparing warm-gold highlights, subtle academic outline icons, Georgia headings, readable system sans-serif body text, a real headshot, no JavaScript framework or unnecessary animations, and explicit distinction between ongoing research and future interests.

## GitHub documentation

- https://docs.github.com/en/pages/quickstart
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
