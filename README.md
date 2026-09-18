# eXp Culture Center Louisville

Public website for the eXp Culture Center in Louisville, KY. Single static page (`index.html`), no build step, English/Spanish toggle built in.

## Publish with GitHub Pages
1. Push this folder to the repo's `main` branch.
2. Repo → Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / `/ (root)` → Save.
3. The site goes live at `https://<user>.github.io/<repo>/` within a minute or two.

## Custom domain: expculturecenterlouisville.com
The `CNAME` file in this repo tells GitHub Pages which domain to serve.

At the registrar, add these DNS records:

| Type  | Name | Value                    |
|-------|------|--------------------------|
| A     | @    | 185.199.108.153          |
| A     | @    | 185.199.109.153          |
| A     | @    | 185.199.110.153          |
| A     | @    | 185.199.111.153          |
| CNAME | www  | fjmerlet-cell.github.io  |

Then: repo → Settings → Pages → Custom domain → `expculturecenterlouisville.com` → Save → tick "Enforce HTTPS" once the DNS check passes.

Later, the agent app goes on `app.expculturecenterlouisville.com` (one more CNAME).

## Editing
All copy lives in `index.html`. English text is in the HTML; Spanish translations are in the `ES` dictionary near the bottom of the file, keyed by `data-i18n` attributes.
