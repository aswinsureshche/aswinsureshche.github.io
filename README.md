# aswinsuresh.us.com

Static portfolio, five pages. Each page repeats the same header, tabs and footer, so edit those in all five files. No build step, no JavaScript, no third-party requests.

| File | Purpose |
|---|---|
| `index.html` | Overview tab |
| `soc/`, `cloud/`, `asl/`, `experience/` | One page per tab (each an `index.html`) |
| `styles.css` | Shared styles for every page |
| `fonts/` | Self-hosted Newsreader, Public Sans, JetBrains Mono (OFL) |
| `og.png` | 1200×630 link preview for LinkedIn, Slack, iMessage |
| `.well-known/security.txt` | RFC 9116 security contact |
| `404.html`, `robots.txt`, `sitemap.xml`, `CNAME`, `.nojekyll` | Hosting and SEO |

## Run locally

    python3 -m http.server 4173

## Deploy (GitHub Pages)

1. Push this folder to a public repo, e.g. `aswinsureshche/aswinsuresh.us.com`.
2. Repo **Settings → Pages**: deploy from branch `main`, folder `/ (root)`.
3. At your domain registrar, add four `A` records for `aswinsuresh.us.com`:
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
4. Back in **Settings → Pages**, wait for the DNS check, then tick **Enforce HTTPS**.

## Keep it current

- Update the footer date (all five pages) and `sitemap.xml` `lastmod` when content changes.
- `security.txt` expires 2027-11-17; push the date forward before then.
- Replace `Aswin_Suresh_Resume.pdf` with each new résumé (same filename).
