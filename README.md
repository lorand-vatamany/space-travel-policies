# space-travel-policies

Public pages (privacy policies and the like) for all my Android apps, published
with GitHub Pages at https://lorand-vatamany.github.io/space-travel-policies/.
The apps' source repos stay private; only these pages are public.

| App | Privacy policy URL (as entered in Play Console) |
|---|---|
| Space Travel | https://lorand-vatamany.github.io/space-travel-policies/privacy-policy.html |
| First Cut | https://lorand-vatamany.github.io/space-travel-policies/first-cut/privacy-policy.html |

## Layout

```
index.html                     home page listing every app
privacy-policy.html            Space Travel (kept at the root: its URL is already in Play Console)
first-cut/privacy-policy.html  First Cut
<app-name>/...                 one folder per new app
```

## Adding a new app

1. Copy `first-cut/` to a new folder named after the app, lowercase with
   dashes (e.g. `plane-war/`).
2. In the copied `privacy-policy.html`, change the app name, the "Last updated"
   date, and the sections that differ (what the app saves, ads, analytics,
   purchases, permissions). The policy has to describe that specific app.
3. Add a section for it to `index.html`.
4. Commit and push to `main`. The page is live a minute later at
   `https://lorand-vatamany.github.io/space-travel-policies/<app-name>/privacy-policy.html`.
   Paste that URL in Play Console.

Other pages for an app (terms, support, account deletion) go in the same
folder.

Don't rename this repo or move the existing pages: the GitHub Pages URLs would
change and the links in Play Console would break.
