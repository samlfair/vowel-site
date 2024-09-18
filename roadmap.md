---
description: What's planned.
---

# Roadmap

## MVP

- [x] Add all element types supported in Obsidian to markdown
- [x] Add rich link previews
- [x] Add RSS
- [x] Add robots.txt
  - [x] AI
  - [x] Search
  - [x] Image
- [x] Typing
- [x] Add sitemap
- [x] Make taxonomies linkable in frontmatter (if a corresponding folder exists)
- [x] Add header metadata (meta tags)
- [x] CSS handling
- [x] Favicon handling
- [x] Docs
- [x] Build action

## V2

- [x] Images as `<figure>`s
- [x] Frontmatter interpolation (title and description)
- [x] CSS default
- [x] Better favicon and styles handling
- [x] Ignore README files
- [x] Include breadcrumbs in page titles
- [x] Add hidden routes (`$`)
- [x] Image alt text
- [x] Deploy action (Vercel)
- [x] Add anchor links for headings
- [x] Figure out how to stop components from remounting on every change
- [x] Demote headings global option (headings are now demoted intelligently)
- [x] Taxonomy lists
- [x] ~~Strikethrough~~
- [x] Checklists
- [x] GitHub-style notes
- [x] Footnotes
- [x] Better create/delete handling in HMR
- [x] Disable default styles option
- [x] Better theme CSS handling
- [x] Create style reset theme
- [x] Debug settings page HMR (temporary fix with full-page refresh)
- [x] Fix checklist boxes
- [x] Handle SVGs properly
- [x] Slogan in homepage `<title>`
- [x] Prioritize `title` and `h1` for meta title
- [x] Prioritize `title` over `h1` for thumbnails
- [x] Tables of contents
- [x] Frontmatter interpolation (image)
- [ ] Add a default 404 page
- [ ] [WebMentions](https://indieweb.org/webmentions)
- [ ] [Microformats2](https://indieweb.org/microformats2) markup
- [ ] Define get-all queries with `*` and `**`
- [ ] Add a meta `generator` tag
- [ ] Basic caching with [fs.stat](https://nodejs.org/docs/v0.4.12/api/fs.html#fs.stat)
- [ ] Support Obsidian callouts and GitHub alerts

## V3

- [ ] Fallback homepages
- [ ] Date format customizing
- [ ] Init CLI
  - Option for destructive actions
  - Create homepage
  - Create CSS file
- [ ] ::Mark::
- [ ] Add more header metadata?
- [ ] Define folder settings
  - [ ] Title
  - [ ] Breadrumb
- [x] Define special page properties
  - [x] Title
  - [x] Description
  - [x] Meta image
  - [x] Date
  - [ ] Modified date
  - [ ] Tags
  - [ ] Author/Authors
- [ ] Make file names kebab-cased for URLs and links
- [ ] Code highlighter
- [ ] Add in-browser search
- [ ] Make RSS optional
- [ ] Pagination

## Wish list

- [ ] Automatic file creation
- [ ] Image serving and optimization
- [ ] GUI
- [ ] More deploy actions
- [ ] Optional JSON interactivity (ratings, comments, SubPubHub)
- [ ] Redirects
- [ ] Advanced markdown
  - [ ] Highlight
  - [ ] Sanitize
  - [ ] Mermaid
  - [ ] Math
  - [ ] Wikilinks
