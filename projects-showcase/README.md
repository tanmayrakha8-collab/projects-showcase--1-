# Projects showcase

A small site that lists my deployed projects, with links to each live site and its code.

**Live page:** `https://YOUR-USERNAME.github.io/YOUR-REPO/`

## Add or edit a project

Everything comes from `projects.json`. Each entry looks like this:

```json
{
  "name": "Project name",
  "summary": "One or two sentences on what it does.",
  "stack": ["HTML", "JavaScript"],
  "live": "https://example.com",
  "repo": "https://github.com/you/repo",
  "status": "live"
}
```

`status` can be `live` (a website you can open), `app` (Android) or `desktop`. Leave `live` empty if there is nothing to open.

## Run locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000. (Opening `index.html` directly will not load `projects.json`.)

## Deploy

Pushing to `main` publishes the site through the included GitHub Actions workflow.
In the repo, go to Settings → Pages and set Source to **GitHub Actions** (one time only).
