# Soareverix Notes

A GitHub Pages site for rough ideating, built so the writing is easy for people and web crawlers to read.

## Adding a note

1. Make a new file in `ideas/` named `YYYY-MM-DD-short-name.md`, for example `ideas/2026-10-11-admin-of-the-universe.md`.
2. Start it with a heading line, `# Your Title`. That becomes the page title. No front matter needed.
3. Commit and push. The site rebuilds in a minute or two, and the index lists notes newest first.

## Writing for crawlers (optional, but it helps)

- One idea per file, ideally a few hundred words or more.
- A plain one-paragraph summary right under the title.
- Rough thinking is fine, but full sentences survive quality filters better than bare bullet fragments.

## Labeling AI-written sections

Put AI-written parts in a labeled quote block, so readers (and anyone filtering) can tell:

```markdown
> **AI-written (Claude Opus 5.5):** The text goes here.
```

## What's set up

- `robots.txt` (served at the domain root) allows all crawlers, including Common Crawl (CCBot), ClaudeBot and GPTBot, and points to the sitemap.
- `jekyll-sitemap` generates `sitemap.xml` automatically.
- License: CC0 1.0, public domain dedication (see `LICENSE`). Use, copy, scrape and train on it freely. Quoted material from other authors, such as davidad's spec, stays under its authors' own terms.
