# Creator Hub Website Template

A modern, mobile-first personal hub template for creators, influencers, and digital professionals.

## Project Structure

```text
/
├── index.html
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   └── img/
│       ├── profile.svg
│       └── about.svg
└── README.md
```

## How to Change Profile Data

Edit `index.html`:

- Creator name: update text in the header brand and hero `<h1>`.
- Bio: update the paragraph with class `.hero-bio`.
- Expertise and about text: update the content in the **About** section.
- Email and contact links: update values inside the **Contact** section (`mailto:` and WhatsApp URL).

## How to Update Links

In `index.html`, update `href` values for:

- Header social links
- Hero CTA buttons
- Main link cards
- Featured content links
- Product buttons
- Footer links

Tip: Use full URLs (`https://...`) for external links and IDs (`#contact`) for same-page navigation.

## How to Add New Cards

### Main Links cards
1. Locate the `Main Links` section.
2. Copy one `<a class="card card-link">...</a>` block.
3. Paste it inside the same `.link-grid` container.
4. Update title, description, icon, and link.

### Featured / Products / Contact cards
1. Locate the target section.
2. Copy one `<article class="card">...</article>` block.
3. Paste it in the section's `.card-grid`.
4. Update content and CTA link.

## How to Change Colors

Open `assets/css/style.css` and edit CSS variables in `:root`:

- `--color-primary`
- `--color-secondary`
- `--color-accent`
- `--color-bg`
- `--color-text`
- `--color-muted`

These are used globally for buttons, text, cards, and backgrounds.

## JavaScript Behavior

`assets/js/main.js` handles:

- Dynamic footer year (`© current year`)
- Lightweight fade-in on scroll using `IntersectionObserver`
- Respect for `prefers-reduced-motion`

## Deploy to GitHub Pages

1. Push this project to a GitHub repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or your default branch)
   - **Folder:** `/ (root)`
4. Save and wait for deployment.
5. GitHub Pages will provide your public URL.

## Performance & Accessibility Notes

- No framework dependencies.
- System font stack for fast rendering.
- Semantic sectioning and a single `<h1>`.
- Focus-visible styles and keyboard-friendly interactive elements.
- Alt text included for images.
