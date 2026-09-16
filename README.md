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
