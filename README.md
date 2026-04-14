# DWGX Blog

Add `.md` files to `posts/` folder. They auto-appear on [dwgx.github.io](https://dwgx.github.io).

## Frontmatter

```yaml
---
title: Post title
date: 2026-04-14
tags: [tag1, tag2]
author: DWGX
size: medium        # small | medium | large | full
color: "#4f8ff7"    # accent color for card border/glow
pin: false          # pinned to top
type: text          # text | image | link | log
image: url          # cover image (for image type)
link: url           # external link (for link type)
visibility: public  # public | unlisted
---
```

### Card Sizes
- `small` — 1 column, compact
- `medium` — 1 column, normal (default)
- `large` — 2 columns wide
- `full` — full width

### Types
- `text` — standard article card
- `image` — image-focused card with cover
- `link` — external link card with arrow
- `log` — dev log / changelog style (compact, monospace)
