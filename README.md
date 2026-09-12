# kevin.babu

Static site. Plain HTML + one shared `style.css`. No JS, no build step, no templating — pages are hand-edited and self-contained.

## Adding a blog post

1. Create `blog/YYYY/MM/slug.html` (copy `blog/2026/08/hello-world.html` as a starting point).
2. Fix the relative paths to `style.css`, home, and blog index (three `../../../` levels deep from a post).
3. Add a line for it in `blog/index.html`, under the right year (`h2`) and month (`h3`), newest first.

## Structure

```
index.html          homepage
style.css            shared styles for every page
blog/index.html      archive, grouped by year > month
blog/YYYY/MM/*.html  individual posts
```
