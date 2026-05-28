# Contributing to Patio Coffee Club

## Adding a New Event

Open `events.html` and copy an existing event card block inside `.events-list`. Update the date, title, time, description, and tag:

```html
<div class="event-card">
  <div class="event-date">
    <div class="day">6</div>
    <div class="month">Jul</div>
  </div>
  <div class="event-info">
    <h3>Event Title</h3>
    <div class="event-meta">
      <span>&#x1F554; 9:00 – 11:00 AM</span>
      <span>&#x1F4CD; Back Patio</span>
    </div>
    <p class="event-description">A short description of what's happening.</p>
    <span class="event-tag">Open to All</span>
  </div>
</div>
```

Keep events in chronological order.

## Adding Photos to the Gallery

1. Drop your image file into the `images/` folder (JPEG or WebP recommended, keep files under 2MB)
2. Open `gallery.html` and replace a placeholder block with a real image tag:

```html
<!-- Replace this: -->
<div class="gallery-item">
  <div class="gallery-placeholder">...</div>
</div>

<!-- With this: -->
<div class="gallery-item">
  <img src="images/your-photo.jpg" alt="Brief description of the photo">
</div>
```

3. Add a descriptive `alt` attribute for accessibility.

## Code Style

- 2-space indentation
- Use semantic HTML elements (`<section>`, `<nav>`, `<footer>`, etc.)
- Keep all styles in `style.css` — no inline styles except when unavoidable
- Test in a browser before pushing

## Pushing Changes

```bash
git add events.html          # or gallery.html, images/, etc.
git commit -m "Add June 6 event"
git push
```

GitHub Actions will automatically deploy the updated site to GitHub Pages within a minute or two.
