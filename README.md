# www.xperilab.com

The Xperilab, LLC landing page. One static file, no build step, no dependencies.

Served by GitHub Pages from `main` at the repo root. `CNAME` pins the custom
domain; changing it in the Pages settings UI rewrites this file, so edit it here
and let Pages follow.

Deliberately unbranded for now — it exists so the company domain resolves to
something real. Branding comes later.

## DNS

    CNAME  www   →  com-xperilab.github.io.
    A      @     →  185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

The apex A records let GitHub redirect `xperilab.com` → `www.xperilab.com`.

## Planned: split the per-app policies out

These pages currently carry per-app detail for Elite Workouts and Budge. When
each app gets its own subdomain, that detail moves and this site slims down:

- `www.xperilab.com/privacy/` keeps only the company-level posture (no servers,
  no collection) and links out.
- `<app>.xperilab.com/privacy/` and `/support/` carry the real per-app document,
  **authored in that app repo's own `web/` directory** — so a change to how the
  app handles data and the change to its policy land in the same diff, and the
  policy travels with the repo if the project spins out.

Leaving the detail in two places is how a privacy policy quietly stops being
true, so do the split when the subdomains go up rather than after.

App records can point here in the meantime; Apple allows those URLs to be
edited per version.
