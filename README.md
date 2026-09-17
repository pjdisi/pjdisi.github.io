# Pablo J. Diego Simón — Personal Website

Personal website, published at **https://pjdisi.github.io/**.

## Files

- `index.html`: website content, styles, and carousel script.
- `assets/images/`: portrait and Music & Places photographs.
- `assets/cv.pdf`: CV linked from the website.
- `.nojekyll`: serves the site as plain static files.

## Preview locally

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 in a browser.

## Publish updates

Edit `index.html` or replace files in `assets/`, then commit and push:

```sh
git add index.html assets/
git commit -m "Update website"
git push origin main
```

GitHub Pages publishes from the root of `main`. This is configured in
**Settings → Pages → Build and deployment → Deploy from a branch**.
No build step or package installation is required.
