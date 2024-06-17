---
title: Deploy
description: Get going.
---

See the [quickstart](/docs/quickstart) for instructions on how to use npm.

# Building

Run `npm run build` (`vowel build`) to build your website.

Alternatively, with npx, run:

```
npx -p svelte@next -p vowel@latest npx vowel build
```

# Deploy

We recommend deploying on Vercel. Run `npx vercel` to deploy your project. Ignore all of the build settings (except project title), as your project will include a `vercel.json` file with build settings.
