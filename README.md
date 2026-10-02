# BioMem

A responsive company website for BioMem, an early-stage project developing biologically derived memory hardware in Helsinki, Finland. The site explains material, electrical-interface, and memory-architecture research through a conceptual device illustration and a write, hold, read sequence.

## Website files

- `index.html`: website copy, accessible inline SVG device illustration, and search/social metadata.
- `styles.css`: responsive layout, keyboard focus styles, and reduced-motion support.
- `favicon.svg`: BioMem memory-cell icon.
- `.nojekyll`: serves the static website without Jekyll processing.

The site uses plain HTML and CSS. No build step, JavaScript, external fonts, analytics, or runtime dependencies are required. `.preview/` contains local review output and must not be uploaded.

## Local preview

Serve this directory with a static HTTP server. For example:

```sh
python -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080/`. Review desktop and phone layouts, section links, and the device diagram.

## GitHub Pages

Repository: [Athena5-28/Bio-mem-website](https://github.com/Athena5-28/Bio-mem-website).

Live website: [athena5-28.github.io/Bio-mem-website/](https://athena5-28.github.io/Bio-mem-website/).

1. Keep the website files at the root of `main`, preserving unrelated files and repository history.
2. In [Settings → Pages](https://github.com/Athena5-28/Bio-mem-website/settings/pages), select **Deploy from a branch**, **main**, and **/(root)**.
3. After changing website files, check the [Actions deployment](https://github.com/Athena5-28/Bio-mem-website/actions) for success.
4. Verify the live website, styling, favicon, and section links.

Assets use relative URLs so they work under the repository's Pages path. The canonical and social URL metadata point to the current live address.

## Content maintenance

All technology descriptions concern research and development. The device illustration is conceptual; performance and system integration remain under experimental validation. Update technical claims only when supported by evidence.

The Connect section links to the actual GitHub repository. Direct contact details can be added when available.

The `linkedin/` directory contains separate, earlier marketing drafts and is not linked from the website.

## A custom domain later

Configure a verified domain in GitHub Pages settings and follow [GitHub's custom-domain guidance](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site). Preserve any `CNAME` file GitHub creates. Once the new domain works over HTTPS, update the two absolute URLs next to the `DOMAIN` comment in `index.html` and verify the deployed website again.

