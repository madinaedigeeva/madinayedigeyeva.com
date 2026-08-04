# madinayedigeyeva.com

Personal site. Four static pages, one hand-written stylesheet, no build step, no JavaScript,
no external requests of any kind — no fonts, no analytics, no trackers. It renders offline and
it will render identically in five years.

## Editing

Open the `.html` file and change the text. There is nothing to compile and nothing to install.
Every page shares `style.css`; the nav lives in each page's `<header>` and is four lines.

## Deploying

GitHub Pages, from `main`. `CNAME` points at the apex domain. DNS records, from GitHub's own
[custom-domain documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site):

```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
AAAA  @    2606:50c0:8000::153
AAAA  @    2606:50c0:8001::153
AAAA  @    2606:50c0:8002::153
AAAA  @    2606:50c0:8003::153
CNAME www  madinaedigeeva.github.io.
```

**On Cloudflare, set every one of these to "DNS only" (grey cloud), not proxied.** GitHub's
documentation describes these records as resolving directly to Pages, and says HTTPS may take
up to 24 hours to become available — it does not document proxying, and a proxy in front of the
apex is an undocumented extra hop while the certificate is being issued. Proxying can be turned
on later, once HTTPS is confirmed working, if there is a reason to.

Then enable **Enforce HTTPS** in Settings → Pages once the certificate is issued.

## The rule this site is written under

Nothing here is stated that a reader cannot check. Where something is early, unproven or
absent, the page says so in those words — including the press page, which is currently empty
and says it is. This is not modesty. A page that pads itself is a page whose other claims a
careful reader will start discounting.
