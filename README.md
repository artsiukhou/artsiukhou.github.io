# Vova's Blog

Source for https://artsiukhou.github.io. Built with [Hugo](https://gohugo.io) and the [Bear Blog theme](https://github.com/janraasch/hugo-bearblog). Pushing to `main` deploys to GitHub Pages (`.github/workflows/hugo.yml`).

## Setup

```sh
brew install hugo
git submodule update --init   # fetches the theme
hugo server                   # http://localhost:1313, live reload
```

## Writing

- New post: `hugo new blog/<name>/index.md`, then edit the front matter (`title`, `date`, `tags`, `slug`) and remove `draft: true` to publish. Posts are served at `/<slug>/`.
- New page (e.g. a CV): create `content/cv.md` with a `title`, then add a `[[menu.main]]` entry in `hugo.toml`.
- Images and other files go next to the post's `index.md`, or into `static/` for site-wide files.
