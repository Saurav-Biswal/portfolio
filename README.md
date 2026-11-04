# Saurav Biswal — Portfolio

A responsive, editorial portfolio for Saurav Biswal, built with plain HTML, CSS, and JavaScript. The site presents selected work through interactive project doors, alongside a personal introduction, timeline, skills, and contact details.

## Features

- Interactive project doors with focused case studies, project visuals, and scoped previous/next navigation
- Responsive layouts for desktop and mobile, with reduced-motion support and keyboard-accessible controls
- Custom desktop cursor with native touch behavior on touchscreen devices
- Original cafe portrait used in the hero and interactive identity card
- Contact form validation that opens a prefilled email draft in the visitor’s default mail application
- GitHub and LinkedIn profile links

The contact form does not send data to a server. It uses a `mailto:` link to open an email draft.

## Technologies

- Semantic HTML
- CSS, including responsive layouts and motion preferences
- Vanilla JavaScript
- Google Fonts for DM Sans, DM Mono, and Playfair Display, with local system-font fallbacks

There is no framework, package manager, build step, backend, or runtime dependency.

## Project structure

```text
.
├── index.html
├── src/
│   ├── app.js
│   ├── styles.css
│   └── assets/
│       └── saurav-cafe.jpg
└── README.md
```

All site code and image references use paths relative to the project root. The portfolio does not call a local API or depend on files outside this repository. Google Fonts are an optional external font source; system fonts are used if they cannot load.

## Run locally

From the project directory, start any static file server. For example, with Python:

```bash
python -m http.server 4173
```

Then open <http://localhost:4173>.

## Deploy on Vercel

1. Push this repository to GitHub.
2. In Vercel, choose **Add New → Project** and import `Saurav-Biswal/portfolio`.
3. Use the repository root as the Root Directory and choose **Other** as the Framework Preset.
4. Leave the Build Command and Install Command blank. Serve the repository root (`.`) as the Output Directory.
5. Select **Deploy**.

No build or install command is required for this static site. Vercel can connect the production branch to automatic deployments: new commits pushed to `main` publish a production deployment, while preview branches and pull requests can receive preview deployments.

## Links

- GitHub: <https://github.com/Saurav-Biswal>
- LinkedIn: <https://www.linkedin.com/in/saurav-biswal/>
