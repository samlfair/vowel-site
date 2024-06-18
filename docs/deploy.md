---
title: Deploy
description: Get going.
---

See the [quickstart](/docs/quickstart) for instructions on how to use npm.

**Note on URLs:** This guide includes instructions for Vercel, which specify a deploy option called `cleanUrls`. This will trim the `.html` extension from your deployment URLs. If you configure your own deploy, ensure you use clean URLs or your links will not work.

# GitHub

If you have a GitHub repository of Markdown files, you can deploy them on Vercel automatically on changes.

Add a `vercel.json` file to the root of your project with the following contents:

```js
{
  "cleanUrls": true,
  "outputDirectory": ".output",
  "buildCommand": "npx -p svelte@next -p vowel@latest npx vowel build"
}
```

Then create a new Vercel project and connect your GitHub repository.

When you push changes to your repository, your Vercel project will automatically rebuild.

# npx

You can manually build your project with `npx`. Run this command:

```
npx -y -p svelte@next -p vowel@latest npx vowel build
```

The build command will create a `vercel.json` file at the root of your project with the necessary configuration for a Vercel deploy. Now deploy to Vercel:

```
npx vercel --prod
```

(The `--prod` flag will deploy to production.)

If you don't want to use the Vercel CLI, you can deploy the `.output` directory to any server that supports static HTML.

# npm

If you set up your project with npm, you can include a `build` command in your `package.json`:

```diff
    "scripts": {
      "dev": "vowel",
+     "build": "vowel build"
    },
```

Run `npm run build` (`vowel build`) to build your website.

Now you can deploy to Vercel:

```
npx vercel --prod
```

(The `--prod` flag will deploy to production.)

If you don't want to use the Vercel CLI, you can deploy the `.output` directory to any server that supports static HTML.