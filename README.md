# madinayedigeyeva.com

Personal site. Four static pages, one hand-written stylesheet, no build step, no JavaScript,
no external requests of any kind — no fonts, no analytics, no trackers. It renders offline and
it will render identically in five years.

## Editing

Open the `.html` file and change the text. There is nothing to compile and nothing to install.
Every page shares `style.css`; the nav lives in each page's `<header>` and is four lines.

## Deploying

GitHub Pages, from `main`. `CNAME` points at the apex domain; DNS for it must be:

```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  madinaedigeeva.github.io.
```

Then enable **Enforce HTTPS** in Settings → Pages once the certificate is issued.

## The rule this site is written under

Nothing here is stated that a reader cannot check. Where something is early, unproven or
absent, the page says so in those words — including the press page, which is currently empty
and says it is. This is not modesty. A page that pads itself is a page whose other claims a
careful reader will start discounting.
