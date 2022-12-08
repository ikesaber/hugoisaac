---
title: "Installing Hugo"
tags: ['How-to']
draft: false
---

# How to install Hugo in Ubuntu: 

`sudo apt install npm && sudo apt install nodejs && sudo apt install hugo`

# Get a theme:

```sh
hugo new site new-site
cd new-site
git clone https://github.com/lukesmithxyz/lugo themes/lugo
echo "theme = 'lugo'" >> config.toml
cp themes/lugo/static/style.css static/
```

## stuff

- Makes one RSS feed for the entire site at `/index.xml`
- Stylesheet is in `/style.css` and includes some important stuff for partials.
- If a post is tagged, links to the tags are placed at the bottom of the post.
- `nextprev.html` adds links to the Next and Previous articles to the bottom of a page.
- `taglist.html` links all tags an article is tagged to for related content.

# Make a new page
- make a new page with `hugo new content/webpage.md`

# Change the templates for new pages
- change the file `archetypes/default.md`

# Use Hugo Server
- `hugo server --noHTTPCache` updates the website as it is being edited (viewable from a link presented by hugo, e.g. `http://localhost:1313/`)

# Change draft status / add category tag

- `tags: ['tag-goes-here']` will add a category tag to your page

- `draft: false` to publish 

- `draft: true` to unpublish

# Create a new home page
- make a new page with `hugo new content/_index.md`



---