# Trustly Pharma Research Library — GitHub Pages

## Upload and publish

1. Create a **public** repository named `trustlypharma.github.io` under the GitHub account `trustlypharma`. If that name already exists, use a different repo and note that its Pages URL will be different.
2. Download the delivered ZIP and extract it. Upload **all its files directly to the repository root** (no folder nesting) using **Add file → Upload files**. Commit the changes.
3. Go to **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**, select **main** and **/(root)**, then Save.
4. Open `https://trustlypharma.github.io/` after GitHub reports a successful Pages deployment.
5. Test all menu links, search, category filtering, mobile navigation, and an article link.

## Add a new blog post (no new HTML file required)

1. Open `posts.json` in GitHub and click Edit.
2. Add one JSON object to the **beginning** of the array, with a unique `slug`, `title`, `category`, `date` (YYYY-MM-DD), `summary`, and `sections`.
3. A section has `heading` and `paragraphs` (an array of text strings). Copy an existing post object as your template, update its values and keep JSON commas and quotes valid.
4. Commit. The new post will appear automatically on the homepage and searchable blog library. Its URL follows `article.html?post=your-slug`.
5. Preview the live article. Text-only articles are safest with this approach; do not paste raw HTML into JSON.

## Notes

- Every file is placed in the ZIP root. The uploaded logo is `logo.jpg`.
- The site is a static GitHub Pages website. Its blog works by reading `posts.json` in the visitor's browser. It is not a WordPress CMS and does not support password-protected dashboard editing, image uploads per post, or automatically generated separate HTML files.
- For stronger individual article search indexing and per-post social previews, static HTML article files or a build system would be an upgrade.
- The three starting posts are editorial examples; check scientific sourcing before representing them as authoritative research.
- This ZIP is prepared for publication, not proof of live deployment or indexing.
