# Webmentions

Vowel has experimental support for Webmentions, based on [webmention.io](https://webmention.io/).

If you set `webmentions: true` in your root `settings.md` file, then Vowel will add a `rel="webmention"` link to your website with an `href` pointing to a `webmention.io` endpoint for your website. (Your `domain` must also be property configured in `settings.md`.)

This will all happen automatically.

Vowel will also automatically send webmentions for links in your content. 

:::note

When will the webmention send? Only on subsequent builds; if you publish a link to a friend's website on Monday, and then update your website on Tuesday, your friend will receive the webmention on Tuesday.

This is a particular challenge of building a platform-agnostic static site generator. New webmentions are indexed when you build your site, but they can only be sent later, since the mention needs to be validated on your deployed site.

:::

Webmentions are still in development.

Want to display webmentions on your website? That feature will be available soon.