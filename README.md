# Pablo J. Diego Simón — Personal Website

Personal website, published at **https://pjdisi.github.io/**.

## Files

- `index.html`: website content, styles, and carousel script.
- `assets/images/`: portrait and Music & Places photographs.
- `assets/cv.pdf`: CV linked from the website.
- `.nojekyll`: serves the site as plain static files.
- `robots.txt` and `sitemap.xml`: crawler access and the canonical homepage URL.

## Preview locally

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 in a browser.

## Publish updates

Edit `index.html` or replace files in `assets/`, then commit and push:

```sh
git add index.html assets/ robots.txt sitemap.xml README.md
git commit -m "Update website"
git push origin main
```

GitHub Pages publishes from the root of `main`. This is configured in
**Settings → Pages → Build and deployment → Deploy from a branch**.
No build step or package installation is required.

## Google Search

The homepage includes a canonical URL and structured profile data. The sitemap is
available at https://pjdisi.github.io/sitemap.xml.

To request indexing, add `https://pjdisi.github.io/` as a **URL-prefix property**
in [Google Search Console](https://search.google.com/search-console/). Choose
**HTML tag** verification, add Google's exact verification tag inside the
homepage's `<head>`, publish it, and click **Verify** in Search Console.
Keep the tag in place after verification.

Then inspect the homepage URL and choose **Request indexing**. You can also
submit `sitemap.xml` in the **Sitemaps** report. Crawling and indexing take time;
these steps do not guarantee inclusion or a particular search ranking.
