# Patio Coffee Club

A simple website for a recurring Sunday morning coffee gathering on the back patio.

**Live site:** https://szellers.github.io/sunday-coffee/

---

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero, about the event, quick details |
| Events | `events.html` | Upcoming Sunday events list |
| Gallery | `gallery.html` | Photo grid |

## Running Locally

No build tools or server required. Just open any HTML file directly in your browser:

```
open index.html
```

Or double-click `index.html` in Finder.

## Deploying

The site auto-deploys to GitHub Pages on every push to `main` via the GitHub Actions workflow at `.github/workflows/deploy.yml`.

To deploy manually:
1. Push your changes to `main`
2. GitHub Actions picks it up automatically
3. Check the Actions tab in the GitHub repo for deploy status

To enable GitHub Pages for the first time:
1. Go to repo Settings → Pages
2. Set Source to **GitHub Actions**

## Adding Content

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add events and photos.

## Project Structure

```
sunday-coffee/
├── index.html              # Home page
├── events.html             # Events list
├── gallery.html            # Photo gallery
├── style.css               # All shared styles
├── script.js               # Mobile nav toggle
├── images/                 # Drop photo files here
├── README.md
├── CONTRIBUTING.md
└── .github/
    └── workflows/
        └── deploy.yml      # Auto-deploy to GitHub Pages
```

## Future Ideas

- RSVP / headcount form (Formspree)
- Custom domain
- Dark mode
- Instagram photo embed
- Auto-generate event cards from a JSON file
- Coffee brew guide page
