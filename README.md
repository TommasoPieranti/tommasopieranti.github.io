# Homepage

## Template forked from
This repository contains the files needed to replicate my blog: [gregorygundersen.com/blog](http://gregorygundersen.com/blog/).  
For detailed background information, see [this post](http://gregorygundersen.com/blog/2020/06/21/blog-theme).

---

## Changes Made
### Core Updates
- **Gemfile**: Updated to use Jekyll 4.0 and its dependencies.
- **mainjax.html**: Edited to use KaTeX only to prevent conflicts with MathJax.
- **blog.css**: Added `figure-container` class for figures with multiple images.
- **_config.yml**: 
  - Updated `url`.
  - Integrated `ieee.csl` scholar style from Zotero.
- **_includes/bibliography.html**: Added Zotero support to handle double numbering.

### Layout Updates
- **nav.html**: Updated top-bar links.
- **index.html**: Modified homepage links.
- **_layouts/blog_main.html & _layouts/blog_post.html**: Created separate layouts for the blog's main page and individual posts.

### Other Additions
- **.gitignore**: Added `_site` to exclude build files.
- **assets/images**: Created directory to store images used in posts.

---

## Notes
- Jekyll automatically generates the `post.url` value based on the permalink structure defined in `_config.yml` or the front matter of each post.

---

## Useful Commands

### Test Locally
Run the site locally to preview changes:
```bash
bundle exec jekyll serve
```

### Clear Jekyll cache
```bash
rm -rf _site
bundle exec jekyll clean
```
