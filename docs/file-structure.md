---
title: File structure
breadcrumb: Files
description: Organize your files.
---

Your website is made of folders and markdown files. Every folder should have a `home.md` file. Every folder can also have a `settings.md` file to apply folder-level settings, such as the `breadcrumb`.

Almost every file and folder represents a page on your website:

- `home.md` is your homepage, `/`
- `about.md` would be your about page, `/about`
- `blog/home.md` would be your blog homepage, `/blog`
- `blog/hello-world.md` would be a blog post, `/blog/hello-world`

(File names like `Hello World.md` also seem to work fine so far.))

Even if a folder doesn't have a `home.md` file, it will still generate a page, so long as it contains any markdown files. So, if you have a `blog` folder with posts inside it, Vowel will generate a `/blog` homepage even if you don't have a `/blog/home.md` file.

There are a few special files and folders:

- `assets/` contains some static files
  - `assets/styles.css` contains your stylesheet, which will be automatically applied if present
  - `assets/favicon.png` is your favicon
- `templates/` is a commonly-used directory in Obsidian projects, so it will be ignored
- A `settings.md` file will not generate a page. If you want a page called `settings`, you can create a `/settings/home.md` file.
- `.cache.json`
- `.output/`
- `vercel.json`

Any files prefixed with a period will be ignored, as will any files that are not markdown.
