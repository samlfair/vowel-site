---
title: Folder settings
breadcrumb: Folders
description: Configure your project.
---

Every folder should have a `settings.md` file with one property:

- `breadcrumb`: A navigation label

At the root of the project, there should be a global settings file with the `breadcrumb` property and any of the following properties:

- All folder settings, plus
- `title`: Website title
- `robots`
  - `google`: Allow Google Search indexing (`true`/`false`)
  - `google_images`: Allow Google Image indexing (`true`/`false`)
  - `ai`: Allow AI training (`true`/`false`)
- `domain`: Full root URL for the website domain (e.g. `https://example.com`)
- `author`: Website author credit for RSS and copyright
- `icon`: An emoji to use as the site favicon
- `slogan`: The website slogan
- `logo`: The website logo
