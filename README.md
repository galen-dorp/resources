# AI & Mathematics — resource site

A small Jekyll site for GitHub Pages.

## Publish it

1. Create a new GitHub repository and upload all of these files (keep the folder structure).
2. In the repo, go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
3. If the repo is *not* named `USERNAME.github.io`, open `_config.yml` and set `baseurl: "/REPO-NAME"`.
4. After a minute or two the site appears at `https://USERNAME.github.io/REPO-NAME/`.

## Edit it

| To change…                 | Edit                     |
|----------------------------|--------------------------|
| Mission statement / intro  | `index.md`               |
| Quotes on the front page   | `_data/quotes.yml`       |
| Resource list              | `resources.md`           |
| Site title / nav tabs      | `_config.yml`            |
| Colors and fonts           | `assets/css/style.css`   |

### Adding a quote

Append a block to `_data/quotes.yml`:

```yaml
- who: Jane Mathematician
  source: Quanta
  url: https://example.com/article
  text: |
    The quote goes here. Keep it indented under "text: |".
```

### Adding a tab

Create a new file such as `events.md`:

```markdown
---
layout: default
title: Events
permalink: /events/
---

# Events
...
```

Then add it to the `nav` list in `_config.yml`.

## Preview locally (optional)

```
gem install jekyll
jekyll serve
```

Then open http://localhost:4000.
