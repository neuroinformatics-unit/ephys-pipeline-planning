# ephys-pipeline-planning

This repository is for planning the development of an extracellular electrophysiology pipeline builder.

The planning document is published locally as a Quarto book in `book/`.

The site is configured to publish at <https://ephys-pipeline-planning.neuroinformatics.dev>.

## Preview locally

Install [Quarto](https://quarto.org/docs/get-started/), then run:

```bash
quarto preview book
```

For a one-off build:

```bash
quarto render book
```

The rendered site is written to `book/_site/`.

## Publish

The GitHub Actions workflow in `.github/workflows/publish-site.yml` renders the
Quarto book and deploys `book/_site/` to GitHub Pages when changes are pushed to
`main`. The custom domain is set by `book/CNAME`.

GitHub Pages must be configured to use **GitHub Actions** as the source, and DNS
for `ephys-pipeline-planning.neuroinformatics.dev` must point at GitHub Pages.
