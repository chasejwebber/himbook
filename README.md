# HIMbook — himbook.org

A curated, public hospital internal medicine handbook for learners and teachers, built with [Quartz 5](https://quartz.jzhao.xyz) and published to GitHub Pages at **himbook.org**.

## Editing

All content lives in `content/` and is plain Markdown. Open `content/` as an Obsidian vault and edit there; wikilinks, callouts, and frontmatter all work.

- `content/index.md` — the front page (resource shelf)
- `content/about.md` — editor, license, disclaimer
- `content/reasoning/` — schema library and FSPD
- `content/ai.md` — AI at the bedside
- `content/whats-new.md` — changelog
- `content/templates/topic.md` — template for new topic pages (not published)

Legend for links: 🔓 open · 🔒 VUMC login · 🏥 VUMC internal network only

## Local preview

```bash
npm ci
npx quartz plugin install
npx quartz build --serve   # http://localhost:8080
```

## Publishing

Push to `main`. The workflow in `.github/workflows/deploy.yml` builds and deploys to GitHub Pages. The custom domain is set by `baseUrl` in `quartz.config.yaml`, which the CNAME plugin writes into the build output.

## Link checking

`.github/workflows/link-check.yml` runs [lychee](https://github.com/lycheeverse/lychee) every Monday and opens an issue labelled `link-rot` if anything is broken. Login-gated VUMC links are excluded via `.lycheeignore`.

## Upgrading Quartz

```bash
npx quartz upgrade
```

## License

Site text: CC BY-NC-SA 4.0. Quartz: MIT (see `LICENSE.txt`).
