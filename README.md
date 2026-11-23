# Privora website

The public web pages for the Privora Android app, served at **https://privora.codefotech.com/**
by GitHub Pages. The app's source code and the Google Play release material live in the private
repository `codefotech/privora`.

| Path | What it is | Address |
|---|---|---|
| `index.html` | Landing page | https://privora.codefotech.com/ |
| `privacy-policy/index.html` | Privacy policy; Google Play links to it | https://privora.codefotech.com/privacy-policy/ |
| `support/index.html` | Support: common questions and contact | https://privora.codefotech.com/support/ |
| `assets/site.css` | Shared styles: system fonts, light and dark | |

The site has no scripts, no trackers and no third-party requests.

## Hosting

- **GitHub Pages:** branch `main`, root folder.
- **Custom domain:** `CNAME` holds `privora.codefotech.com`.
- **Plain HTML:** `.nojekyll` makes Pages serve the HTML files as they are.

### DNS (one record, at the DNS provider for codefotech.com)

| Type | Name | Value |
|---|---|---|
| CNAME | `privora` | `codefotech.github.io` |

Once the record resolves, turn on **Enforce HTTPS** in the repository's Settings → Pages. To
stop anyone else from claiming the subdomain on GitHub, also verify `codefotech.com` under GitHub
**Settings → Pages → Verified domains**. That adds one TXT record.

## Details shown on the pages

These must match the Google Play listing (`docs/release/play-store/listing-en-US.md` in the app
repository).

| Detail | Value |
|---|---|
| Developer | Seam Uddin |
| Support email | privora@codefotech.com |
| Privacy policy effective date | 23 November 2026 |

## Keeping it accurate

The privacy policy describes the app as built: no `INTERNET` permission, and no data collected
or shared. Any app change that touches permissions, SDKs or data must update the policy and the
Play Console Data safety answers in the same release.
