# CSU Library Journal Finder redesign

This folder is a complete static website. Keep these items together when deploying:

- `index.html` — redesigned interface and search logic
- `journals.json` — journal dataset
- `for-codes.json` — ANZSRC 2020 FOR division and group labels
- `assets/` — CSU logo and approved graphic asset extracted from the supplied CSU DLS template

## Preview locally

The data is loaded with `fetch()`, so opening `index.html` directly may be blocked by browser security. Preview it through a local web server or upload the entire folder to GitHub Pages.

## Deploy to the existing GitHub Pages site

Replace the existing `index.html` and `journals.json`, then add `for-codes.json` and the `assets` folder at the repository root. Commit all files together.

The existing LibGuides iframe URL can stay unchanged.

## Search behaviour

- **Check a journal** searches journal titles and offers autocomplete.
- **Explore by topic** searches journal titles plus official ANZSRC 2020 FOR descriptions.
- **Free to publish** means `Eligible = Yes` or `Diamond OA = Yes`.
- The interface notes that publisher conditions may apply.
- **Scimago Q1** uses the Scimago rank field.

No backend, framework, package installation, or build step is required.
