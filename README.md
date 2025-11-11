# netbrain.github.com

Personal blog built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

## Development

To run the site locally:

```bash
hugo server
```

The site will be available at http://localhost:1313/

## Deployment

The site is automatically deployed to GitHub Pages using GitHub Actions on every push to the `master` branch.

The workflow:
1. Pushes to `master` trigger the GitHub Actions workflow
2. Hugo builds the static site
3. The built site is deployed to GitHub Pages (gh-pages branch is auto-managed)

## Project Structure

- `content/` - Blog posts and pages
- `static/` - Static assets (images, etc.)
- `themes/PaperMod/` - Hugo theme (git submodule)
- `config.toml` - Hugo configuration
- `.github/workflows/hugo.yml` - GitHub Actions deployment workflow

## Adding Content

Create a new post:

```bash
hugo new post/my-new-post.md
```

Edit the file in `content/post/` and set `draft = false` when ready to publish.
