# Koushik Chakraborty — Personal Portfolio

A lightweight, responsive personal portfolio built with plain HTML, CSS and JavaScript. It is designed to deploy directly to GitHub Pages with no backend, database, package manager or build step.

## Project structure

```text
koushik-portfolio/
├── index.html
├── style.css
├── script.js
├── README.md
├── robots.txt
├── favicon.svg
└── profile.png
```

`profile.png` was extracted from the profile photograph contained in the uploaded Europass resume. The public site intentionally omits sensitive resume details such as passport number, date of birth and full home address.

## Preview locally

You can open `index.html` directly in a modern browser. For the most accurate local preview, start a small local server from the project folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Commit and push the files.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your default branch (usually `main`) and the `/ (root)` folder.
7. Save. GitHub will publish the site after deployment finishes.

All CSS, JavaScript and image references use root-relative-to-the-repository file paths (simple relative paths), so the site works both at `username.github.io/` and at a project path such as `username.github.io/repository-name/`. The image files are intentionally kept in the repository root so they can be uploaded through GitHub’s web interface without creating a folder.

## Add or replace a downloadable resume later

The live portfolio does not currently publish a resume PDF because public resume files can expose personal details that are intentionally omitted from the website.

If you want to add a download button later:

1. Put a public-safe PDF in the repository root, for example `Koushik-Chakraborty-Resume.pdf`.
2. Add this link wherever you want the button to appear:

```html
<a class="button button-secondary" href="Koushik-Chakraborty-Resume.pdf" download>
  Download resume
</a>
```

## Replace the profile image

Replace `profile.png` with another image using the same filename, or update the image path in `index.html`. Keep a square or near-square crop for the best result.

## Small fields to review over time

As your background changes, the main items worth updating are:

- Education / graduation status and SGPA if needed
- Project descriptions, dates and technologies
- Current volunteering or activity dates
- Certifications and credential links
- GitHub and LinkedIn profile URLs if they change
- Contact email if you begin using a dedicated professional address

## Accessibility and compatibility

The site includes semantic HTML, a skip link, keyboard-visible focus states, accessible navigation controls, responsive layouts, reduced-motion support and a no-JavaScript navigation fallback. It has no external runtime dependencies.
