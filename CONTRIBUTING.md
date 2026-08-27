# Contributing to HIMbook

Contributions from residents, students, and faculty are welcome.

## Suggest a resource or report a broken link

Open an issue: https://github.com/chasejwebber/himbook/issues

## Add or edit a page

1. Fork the repo and create a branch.
2. Edit Markdown in `content/`. For a new topic, copy `content/templates/topic.md` and set `draft: false` when ready.
3. Tag every external link with the legend: 🔓 open · 🔒 VUMC login · 🏥 VUMC internal network only.
4. For a VUMC-licensed resource, use the CKM resolver link (`https://myknowledgehub.vumc.org/ckmres?rid=...`) or the Eskind ResearchGuides redirect rather than a direct publisher URL, so off-campus login works.
5. Open a pull request. The editor reviews for accuracy and fit; expect light copyediting.

## Style

- One line per link: name, then an em dash, then *when to reach for it*.
- Curated, not comprehensive. If a section grows past ~10 links, that is a sign it wants a topic page instead.
- No patient information, ever.

## Attribution

Contributors are credited on the page they authored (frontmatter `contributors:`) and in `content/whats-new.md`.
