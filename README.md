# LIS351_M1_Huarte.github.io
Fulfilling the requirements of LIS351 Major Project 1

This repository contains a scaffold of a 5-page website for the LIS351 Module 1 assignment.

Pages included:
- `index.html` — Home page (intro)
- `travel.html` — Travel page (unique two-column layout)
- `family.html` — Family page
- `work.html` — Work page
- `friends.html` — Friends page

## Accessibility & validation

What I implemented:
- A visible "Skip to main content" link on every page to help keyboard users.
- Navigation with `aria-current="page"` on each page so assistive tech can identify the active page.
- `alt` attributes and `<figure>/<figcaption>` for non-decorative images.
- Focus styles for keyboard navigation and clear contrast in the header.
- An embedded resume at `media/resume.pdf` with a downloadable fallback.

What to validate with WAVE (and why):
- Run WAVE at https://wave.webaim.org/ against each page (open the page in the browser and paste the URL into WAVE).
- Check for missing `alt` attributes, unlabeled form controls (none in this scaffold), ARIA issues, and color contrast warnings.

Current known items to check/notes:
- A description list was required by the assignment; it has now been added to `work.html` (the Internships section is a `<dl>` with `<dt>`/`<dd>` pairs).
- Manual review: ensure the embedded PDF loads in your browser; some browsers may block cross-origin PDF embedding or block local file renderers — use the download link if the preview fails.

How to preview locally:

```bash
# macOS / zsh
cd /Users/emmahuarte/Documents/LAS351/LAS351_M1_Huarte.github.io
python3 -m http.server 8000
```

Open `http://localhost:8000` and run WAVE from https://wave.webaim.org/ for each page you want to validate. Fix any issues WAVE flags and re-check.

Assets:
- `css/style.css` — External stylesheet linked from all pages
- `images/photo1.svg`, `images/photo2.svg`, `images/photo3.svg` — SVG placeholders

What you need to do:
- Replace placeholder text and images with your own content.
- Validate pages with WAVE (https://wave.webaim.org/) and fix any alerts as needed. There should be no validation errors.

Preview locally:

If you have Python installed, run a simple HTTP server from the repository root and open http://localhost:8000 in your browser:

```bash
# macOS / zsh
cd /Users/emmahuarte/Documents/LIS351/LIS351_M1_Huarte.github.io
python3 -m http.server 8000
```

Then open the pages and check navigation and styles.

Notes:
- The travel page (`travel.html`) uses a grid layout to satisfy the "unique layout" requirement.
- Headings, lists, description lists, images with alt text, nav on each page, and an external link are included as placeholders.
# LIS351_M1_Huarte.github.io
Fulfilling the requirements of LIS351 Major Project 1
