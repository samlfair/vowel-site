---
title: Quickstart
description: Get started with Vowel.
---

## npx

npx is the easiest way to use vowel:

```
npx -y -p svelte@next -p vowel@latest npx vowel
```

Vowel will attempt to generate a website based on the contents of your file.

## npm

Create a directory. Then, open that directory and run these commands in your terminal:

```bash
npm init --y && npm i vowel svelte@next
```

Edit your `package.json` to add these `scripts`:

```json
{
	"dev": "vowel",
	"build": "vowel build"
}
```

Now run `npm run dev`.

## Starter files

Create `home.md` and enter some basic information

```md
# Your website

Lorem ipsum...
```

Create `settings.md` and enter some basic information in the frontmatter:

```
---
breadcrumb: Home
domain: https://example.com
---
```
