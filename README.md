# AI System Design — GitHub Wiki package

Ready-to-paste, multi-page Markdown documentation with **Mermaid diagrams**, a Home landing page and GitHub Wiki's special navigation pages (`_sidebar.md`, `_header.md`, `_footer.md`).

## Install

### Preferred: push into the repository Wiki Git remote

1. Enable **Wiki** in your GitHub repository settings and create its first page if needed.
2. Clone your Wiki, replacing `OWNER` and `REPO`:

   ```bash
   git clone https://github.com/OWNER/REPO.wiki.git
   ```

3. Copy the package's `*.md` files into the **root** of the cloned wiki. You may **omit this README.md** from the Wiki root if you do not want an extra page. `Home.md` is the Wiki front page.
4. Commit and push:

   ```bash
   git add .
   git commit -m "Document production AI system architecture"
   git push origin HEAD
   ```

### Manual copy/paste

In your GitHub repository, open **Wiki** → **New Page**. Make pages using the exact filenames **without `.md`** as their titles (example: `03-Identity-Gateway-and-Limits`), paste the matching Markdown, and save. Start with `Home`. For the custom `_sidebar`, `_header`, `_footer` pages, it is usually easiest to create them in the Wiki Git clone as files with those exact names.

## File map

- `Home.md` — overview and full site index
- `01-...md` through `15-...md` — architecture and implementation articles
- `_sidebar.md` — left navigation
- `_header.md` — top navigation
- `_footer.md` — bottom navigation
- `README.md` — this installation guide

## Link and diagram conventions

Pages use GitHub Wiki-compatible `[[Page-Name]]` and `[[Page-Name|Readable Label]]` links, with ordinary `(Home)` links also supported. **Keep filenames unchanged** so all links resolve. Mermaid fenced diagrams render in GitHub's supported Markdown/Wiki view; other Markdown viewers may show source code instead.

## Editorial scope

The content preserves the transcript's scenario and production-design ideas, while adding explicit implementation guidance. Sample settings, contracts, limits and readiness criteria are identified as recommendations. See [[15-Glossary-and-Source-Notes]] for corrections to transcript arithmetic and ambiguous terminology.
