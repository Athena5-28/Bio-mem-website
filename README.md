# Matter Fold

A responsive website for Matter Fold, an early-stage project exploring how biology can shape matter and make useful materials more widely available. The first research focus is biologically derived memory chips. Broader material and manufacturing systems are future directions; therapeutics is a long-term ambition.

## Website files

- `index.html`: website structure, copy, concept illustrations, and search/social metadata.
- `styles.css`: responsive layout, keyboard focus styles, and reduced-motion support.
- `favicon.svg`: Matter Fold browser icon.
- `matter-fold.svg`: standalone Matter Fold brand mark.
- `.nojekyll`: serves the static website without Jekyll processing.

The site uses plain HTML and CSS. No build step, JavaScript, external fonts, analytics, or runtime dependencies are required. `.preview/` contains local review output and must not be uploaded.

## Local preview

Serve this directory with a static HTTP server. For example:

```sh
python -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080/`. Review desktop and phone layouts, section links, the brand mark, and concept illustrations.

## GitHub Pages

Repository: [Athena5-28/Bio-mem-website](https://github.com/Athena5-28/Bio-mem-website).

Live website: [athena5-28.github.io/Bio-mem-website/](https://athena5-28.github.io/Bio-mem-website/).

The public brand is Matter Fold. Keep the existing repository and Pages URL when updating the website.

1. Keep the website files at the root of `main`, preserving unrelated files and repository history.
2. In [Settings → Pages](https://github.com/Athena5-28/Bio-mem-website/settings/pages), select **Deploy from a branch**, **main**, and **/(root)**.
3. After changing website files, check the [Actions deployment](https://github.com/Athena5-28/Bio-mem-website/actions) for success.
4. Verify the live website, styling, brand mark, favicon, and section links.

Assets use relative URLs so they work under the repository's Pages path. The canonical and social URL metadata point to the current live address.

## Content maintenance

Explain the mission in plain language: use biology to shape matter for broader material abundance. Keep the first focus on memory chips distinct from future material and manufacturing systems and the long-term ambition in therapeutics.

Technology descriptions concern research and development. Illustrations are conceptual; device performance and system integration remain under experimental validation. Do not present future applications as existing products or imply demonstrated clinical capabilities. Update technical and therapeutic claims only when supported by evidence.

The Connect section links to the actual GitHub repository. Direct contact details can be added when available.

The `linkedin/` directory contains separate, archived marketing drafts from the earlier brand and is not linked from the website. Preserve those files as historical materials.

## A custom domain later

Configure a verified domain in GitHub Pages settings and follow [GitHub's custom-domain guidance](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site). Preserve any `CNAME` file GitHub creates. Once the new domain works over HTTPS, update the two absolute URLs next to the `DOMAIN` comment in `index.html` and verify the deployed website again.

