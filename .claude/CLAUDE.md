# Description

A documentation-only site for the **TSE Analytics** desktop application. There is no application code here — only Markdown source files, images, and configuration.
The site is built with **Zensical** (a MkDocs-based static site generator) and deployed to GitHub Pages.

## Commands

Dependencies are managed with **uv** (Python 3.14.3). The `zensical` CLI is the only dev dependency.

```bash
# Install dependencies
uv sync

# Serve locally with live reload
uv run zensical serve --open

# Build static site (output goes to site/)
uv run zensical build --clean
```

CI runs `zensical build --clean` and deploys `site/` to GitHub Pages on every push to `master`.

## Architecture

| Path | Purpose |
|---|---|
| `zensical.toml` | Main config: site metadata, navigation tree, theme, plugins, Markdown extensions |
| `docs/` | Markdown source files and assets |
| `docs/images/` | All screenshots and images referenced in docs |
| `docs/stylesheets/extra.css` | Custom CSS overrides |
| `site/` | Built output — gitignored, do not edit directly |

### Navigation

The navigation structure is **explicitly defined** in `zensical.toml` under the `nav` key. Adding a new page requires both creating the `.md` file under `docs/` and adding an entry to `nav` in `zensical.toml`. The order of entries in `nav` determines the sidebar order.

Top-level sections: Introduction → Installation → Get Started → Main Widgets → Toolbox Widgets → Predefined Variables → Disclaimer → Demo.

### Markdown Extensions in Use

The following non-standard Markdown extensions are enabled (configured in `zensical.toml`):

- `admonition` + `pymdownx.details` + `pymdownx.superfences` — admonition blocks (`!!! note`, `??? tip`, etc.)
- `attr_list` + `md_in_html` — HTML attributes on Markdown elements, Markdown inside HTML
- `pymdownx.blocks.caption` — figure captions
- `content.code.annotate` / `content.code.copy` / `content.code.select` — enhanced code blocks
