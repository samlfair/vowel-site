---
title: Pages
description: Create content.
---

The `body` element on each page has a class representing the current page. The homepage has classes `"page home"`, while a blog post might have `"page blog-hello-world"`.

Vowel attempts to construct a logical semantic HTML structure based on the files and folders in your website.

To do this, Vowel distinguishes between evergreen pages and ephemeral pages. A page with a `date` property is considered ephemeral, so it is excluded from the navigation and sitemap.

Vowel will automatically create a multi-level nav, with one level for each parent folder for the current page.

Vowel will create a full side navigation that displays all evergreen pages.

# Frontmatter

Reserved properties

- `title`: Page title
- `image`: Page image
- `description`: Page description
- `date`: Date published
- `breadcrumb`: Short identifier for the page

Vowel will attempt to impute the type of each frontmatter property. Imputed types include:

- Links (Will generate a link preview)
- Images (will display the image)
- Date (will render a pretty date in a `time` element)

You can also use lists and objects in frontmatter.

# Markdown

Along with all standard markdown, Vowel also allows the following special elements:

## Rich link previews

Paste a URL on its own line (e.g. `https://example.com`).

## Internal link previews

Paste a relative path to a page (e.g. `/about`).

The link will be rendered as an `article` element with a class representing the linked path (e.g. `page-blog-hello-world`).

## Page lists

A relative path to a folder with a `count` parameter (e.g. `/blog?count=2`). This will exclude the `home.md` file for the folder. In this example, it would return the `/blog/hello-world.md` file but not `/blog/home.md`.

The page list will order pages first by date in reverse chronology (newest to oldest) and then alphabetically (a to z).

The list will be rendered as `article` elements (see above) in a `section` element. The `section` element will have a class representing the folder path (e.g. `folder-blog`).

## Headings

If your document starts with an `h1` (`#`) and has no `title` property, the `h1` will be used as the meta title.

If your document includes `h1`s after the title, all headings will be demoted one level (`#` to `h2`, `##` to `h3`).

## Description

If your document doesn't include a `description`, a meta description will be extracted from the text.
