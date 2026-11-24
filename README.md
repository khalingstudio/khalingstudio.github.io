# khalingstudio.github.io

Public website for **Khaling Studio** — the home page and the legal pages (privacy policies) for each app.
Served by GitHub Pages at https://khalingstudio.github.io/

## Layout

One folder per app, so pages never clash:

| Path | Page |
|---|---|
| `index.html` | Khaling Studio home page, lists the apps |
| `family-khata/privacy-policy.html` | Family Khata privacy policy |
| `nepal-assistant/privacy-policy.html` | Nepal Assistant privacy policy |
| `privacy-policy.html` | Old Nepal Assistant address — only forwards to `nepal-assistant/privacy-policy.html`. Keep it until the Play Console link change for Nepal Assistant has been reviewed and is live, then it can be deleted. |

## Adding a new app

1. Create a folder named after the app (lowercase, words joined with `-`), e.g. `my-app/`.
2. Put its `privacy-policy.html` inside.
3. Add the app to `index.html`.
4. Use `https://khalingstudio.github.io/my-app/privacy-policy.html` in the Play Console and in the app.

## Where the text comes from

- **Family Khata:** generated from the app's own Privacy screen — run `node tools/make-policy-page.mjs` in the Family Khata project, then upload `site/family-khata/privacy-policy.html` here.
- **Nepal Assistant:** keep in step with `src/data/legalContent.ts` in the Nepal Assistant project.

Contact: khaling.studio@gmail.com
