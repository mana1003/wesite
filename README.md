# Manali Jain: portfolio

Interactive 3D portfolio. Co-founder and CTO of Taravi; AI/ML and autonomous systems engineer.

Static site: one `index.html`, no build step. Libraries load from cdnjs: Three.js r128, GSAP 3.12.5 and ScrollTrigger.

## Files
| File | Purpose |
|---|---|
| `index.html` | The whole site |
| `404.html` | Page shown for unknown URLs |
| `robots.txt` | Lets search engines index the site |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |
| `DESIGN.md` | Colors, type, spacing and motion rules |

## Publish on GitHub Pages
1. Create a public repository named `<your-username>.github.io`.
2. Upload every file in this folder to the repository root, including `.nojekyll`.
3. Go to Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
4. Open `https://<your-username>.github.io` after a minute or two.

Using a different repository name (for example `portfolio`)? The site then lives at `https://<your-username>.github.io/portfolio/`, and the "Back to the portfolio" link in `404.html` should be changed to `/portfolio/`.

## Edit
- Demo video link: set `demoUrl` near the bottom of `index.html`. The "Watch the demo" button appears when it is not empty.
- Contact details are in the `#contact` section.
- Project tiles are the `T` array in the first `<script>`.

## Test locally
```
python3 -m http.server 8000
```
Then open http://localhost:8000.
