---
title: Styling
description: Add styles to your website.
---

Vowel allows styling through themes and vanilla CSS.

## Themes

Vowel includes a default theme, but you can disable this in your root `settings.md` file:
```
theme: none
```
You also have two other themes available:
- `reset`: A classic CSS reset
- `typography`: A classic CSS reset, plus some basic text styling

## CSS

Create an `assets/styles.css` file for your styling. We recommend using a style framework like Pico or Open Props. You can simply download their stylesheet and either copy-paste it into your own or include it in `assets/` and `import` it into `assets/styles.css`.

For some inspiration on how to style semantic HTML, check out Swyx's [Spark Joy repository](https://github.com/swyxio/spark-joy).

:::tip

You can combine a theme with your own CSS. Feel free to use the `reset` or `typography` theme as a starting point and build from there.

:::

:::warning

This project is still in development, so the generated markup is likely to change quickly and without warning, which will likely affect your styles.

:::
