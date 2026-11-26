# wobble-blog

Static site built with [Parcel v3](https://v3.parceljs.org/) (alpha), deployed to GitHub Pages.

## Develop

```sh
npm install
npm start        # dev server on http://localhost:1234
npm run build    # production build into dist/
```

Entry point is `src/index.html` (the `source` field in `package.json`).

## Deploy

`.github/workflows/deploy.yml` builds and deploys to GitHub Pages on every push to `main`. One-time setup: in the repo settings, set **Pages → Source** to **GitHub Actions**.

The build uses `--public-url ./` so asset URLs are relative and work under the `/wobble-blog/` project-site path.
