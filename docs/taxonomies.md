---
title: Taxonomies
description: Create tags, categories, and authors.
---

If the key for a frontmatter property matches a folder at the root of your project, Vowel will attempt to treat it as a taxonomy and link to the respective page.

For instance, in this folder structure:

```
.
├── home.md
├── design.md
├── recipes.md
└── category/
    ├── inspiration.md
    └── lifestyle.md
```

You can write the following frontmatter in `design.md`:

```
---
title: Design
category: inspiration
---
```

Vowel will render the property as a link to `/category/inspiration`.

Then, in `category/inspiration.md` (or anywhere) you can display all inspiration posts with a post list:

```
/?property=category.inspiration
```

This allows you to create author pages, category pages.
