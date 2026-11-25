# lisabielik.com

Personal resume site for Lisa Bielik, built with [Hugo](https://gohugo.io/) using a customized copy of the [Anatole](https://github.com/lxndrblz/anatole) theme (MIT licensed, see `LICENSE`).

## Layout

- `exampleSite/` – the site itself: content, config, images
  - `content/english/` – pages
  - `config/_default/` – site settings, sidebar/social links, menu
  - `static/images/` – images
- Everything else at the top level is the theme (layouts, styles, scripts).

## Run locally

Requires Hugo **extended** and Dart Sass (`brew install hugo sass/sass/sass`).

```bash
cd exampleSite
hugo server --themesDir ../.. --theme lisa-bielik-resume-master
```

Then open http://localhost:1313. (Use the name of this folder after `--theme`; if you cloned it as `hugo-resume`, use that.)

## Deploy

Netlify builds from `netlify.toml` on every push to `main`.
