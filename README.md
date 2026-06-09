# Miri's Kitchen

A small, public collection of recipes worth sharing, rendered as a static site
by GitHub Pages.

**This repo is generated.** The recipes live in an Obsidian vault on the laptop.
To publish a recipe, add `publish: true` to its YAML front matter, then run the
generator (in the `~/remarkable` repo):

```bash
./publish-recipes          # regenerate recipes/ + index.md, commit, push
./publish-recipes --dry-run  # show what would publish, write nothing
```

The generator strips the `## My Notes` section (personal scratch space) before
publishing.

Layout, styling, and config (`_config.yml`, `_layouts/`, `assets/`) are hand-authored
and safe to edit; `recipes/*.md` and `index.md` are overwritten on every run.
