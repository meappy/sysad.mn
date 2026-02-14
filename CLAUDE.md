# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio website for Gerald Sim (sysad.mn). Jekyll-based static site deployed automatically via GitHub Pages with a custom domain through Cloudflare.

## Development Commands

```bash
# Install dependencies
gem install bundler jekyll
bundle install

# Run local dev server (serves at http://localhost:4000)
bundle exec jekyll serve

# Build site (output to _site/)
bundle exec jekyll build
```

There is also a private companion repo (`sysad.mn-ops`) expected to live alongside this one for automation/deployment scripts.

## Architecture

- **Framework**: Jekyll 3.10 via the `github-pages` gem (v232)
- **Templating**: Markdown + Liquid, rendered by kramdown
- **Styling**: All CSS is written inline within the Markdown content files (no external stylesheets)
- **JavaScript**: Vanilla JS, also embedded directly in Markdown files
- **Layout**: Single `_layouts/default.html` template wraps all pages

### Key Content Files

- `index.md` — Homepage with hero section, rotating taglines, expertise cards, lava lamp background animation, and contact links. All HTML/CSS/JS is self-contained in this file.
- `tetris.md` — Full Tetris game implementation using canvas rendering. Desktop controls (arrow keys, space) and mobile touch controls. All game logic is inline.
- `favicon.svg` — Animated SVG favicon with terminal prompt styling.

### Design Patterns

- Dark theme with blue/purple/cyan gradient palette throughout
- Responsive design via media queries at 768px and 480px breakpoints
- No build pipeline beyond Jekyll — no npm, no bundler for JS/CSS, no preprocessors
- Content and presentation are co-located: each page's styles and scripts live in its own Markdown file
