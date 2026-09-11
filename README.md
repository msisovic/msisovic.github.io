# Marko's Blog

A minimal Hugo blog using the [PaperMod theme](https://github.com/adityatelange/hugo-PaperMod).

## Preview locally

Hugo 0.166.0 is installed in `.tools/hugo` on this machine (not committed).

```sh
./.tools/hugo server -D
```

Open http://localhost:1313. `-D` includes draft posts.

On another machine, install Hugo 0.166.0 or newer and use `hugo` in place of `./.tools/hugo`. Clone this repository with `--recurse-submodules` to include PaperMod, or run `git submodule update --init --recursive` after cloning.

## Write a post

Edit `content/posts/my-first-post.md`, or create another post:

```sh
./.tools/hugo new content posts/another-post.md
```

Write in Markdown. Change `draft: true` to `draft: false` when the post is ready. Drafts are excluded from the public website, but their source files are visible in a public repository; keep private writing outside this repo.

To publish, commit your changes and push to `main`. GitHub Actions builds and deploys the website once the repository's Settings → Pages → Source is set to **GitHub Actions**.

## Customize

Edit `hugo.toml` to change the blog title, introduction, or author name. PaperMod is included as a Git submodule in `themes/PaperMod`, retaining its original MIT license.
