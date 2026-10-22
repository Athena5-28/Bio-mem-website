# Matter Fold

A responsive website for Matter Fold, an early-stage project exploring how biology can shape matter and make useful materials more widely available. The first research focus is biologically derived memory chips. Broader material and manufacturing systems are future directions; therapeutics is a long-term ambition.

## Website files

- `index.html`: website structure, copy, a memory-cell concept illustration, and search/social metadata.
- `styles.css`: responsive layout, keyboard focus styles, and reduced-motion support.
- `favicon.svg`: compact Matter Fold emblem of interwoven strands for the browser icon.
- `matter-fold.svg`: standalone Matter Fold emblem of interwoven strands, based on the supplied brand reference.
- `.nojekyll`: serves the static website without Jekyll processing.
- `CNAME`: GitHub Pages custom hostname, `matterfold.bio`. Preserve this file when publishing.

The site uses plain HTML and CSS. No build step, JavaScript, external fonts, analytics, or runtime dependencies are required. `.preview/` contains local review output and must not be uploaded.

## Local preview

Serve this directory with a static HTTP server. For example:

```sh
python -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080/`. Review desktop and phone layouts, section links, the interwoven strand emblem, and the memory-cell concept illustration.

## GitHub Pages

Repository: [Athena5-28/Bio-mem-website](https://github.com/Athena5-28/Bio-mem-website).

Website domain: [matterfold.bio](https://matterfold.bio/).

The public brand is Matter Fold. Keep the existing repository and use `matterfold.bio` as the public website address.

1. Keep the website files at the root of `main`, preserving unrelated files and repository history.
2. In [Settings → Pages](https://github.com/Athena5-28/Bio-mem-website/settings/pages), select **Deploy from a branch**, **main**, and **/(root)**.
3. After changing website files, check the [Actions deployment](https://github.com/Athena5-28/Bio-mem-website/actions) for success.
4. Verify the live website, styling, brand mark, favicon, and section links.

Assets use relative URLs so they work under the repository's Pages path. The canonical and social URL metadata point to the current live address.

## Content maintenance

Explain the mission in plain language: use biology to shape matter for broader material abundance. Keep the first focus on memory chips distinct from future material and manufacturing systems and the long-term ambition in therapeutics.

Technology descriptions concern research and development. The memory-cell illustration is conceptual; device performance and system integration remain under experimental validation. Do not present future applications as existing products or imply demonstrated clinical capabilities. Update technical and therapeutic claims only when supported by evidence.

The Connect section links to the actual GitHub repository. Direct contact details can be added when available.

The `linkedin/` directory contains separate, archived marketing drafts from the earlier brand and is not linked from the website. Preserve those files as historical materials.

## Custom domain

Set the repository's GitHub Pages custom domain to `matterfold.bio` and retain the root `CNAME` file. The canonical and social URL metadata in `index.html` use `https://matterfold.bio/`; the local generator in `.preview/` uses the same address.

Cloudflare website DNS records should use DNS only and TTL Auto:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | athena5-28.github.io |

Keep domain-verification TXT records and unrelated email records. Once DNS validation and certificate provisioning complete, enable Enforce HTTPS in GitHub Pages. Verify `https://matterfold.bio/`, the redirect from `www.matterfold.bio`, styling, the emblem, and section links. Follow [GitHub's custom-domain guidance](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) when troubleshooting.

