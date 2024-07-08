---
date: 2024-07-08
breadcrumb: Breadcrumb Trail
link: https://www.nngroup.com/articles/breadcrumb-navigation-useful/
---

# A Trail of Breadcrumbs

The breadcrumb is a wonderful, humble UI element. As Jakob Nielsen explains in this article from 2007, breadcrumbs show users their current location relative to higher-level concepts. They're great because all users understand what they are and they take up almost no screen real estate.

A breadcrumb helps situate a user within a certain context and understand how to exit that context. This is important because the context adds meaning to the content. 

The breadcrumbs on this page tell your that this is content is in the blog, which means that it should be light, ephemeral, and personal. If instead of *Blog*, the breadcrumb said *Docs*, that would tell you that this content is dense and authoritative.

Vowel also includes breadcrumbs in page meta titles. This is useful for SEO, as a page with the title *SEO - Features - Vowel* should obviously have different content from a page called *SEO - Docs - Vowel*. I use this feature on my personal blog with my reviews. For a book review, I don't want to write a contrived title, so I use the book's title as the post title. That's a little confusing though, since it makes it look like Malcolm Gladwell wrote a post for my blog. The breadcrumb solves this: *Outliers, by Malcolm Gladwell - Reviews - Sam Littlefair*. The breadcrumb adds context that explains the content. I don't need to spent any time explaining that I'm reviewing a book, since the title and breadcrumb already explain as much. 

Information architecture is the secret superpower of HTML. Content has infinitely more meaning within a larger context. That's why fortune cookies feel cheap while biblical proverbs feel profound. Breadcrumbs are perhaps the most important signifier of information architecture; they announce the relationship between a piece of content and the whole website.

As Nielsen explains, this practically serves as a navigation aid and gives users one-click access to parent pages. But this also forces site authors to consider the context.

In his post on [URLs](/blog/url-ui), Nielsen explains that URLs should be "hackable" — so that if you delete a segment, you arrive at the parent page. If you remove the last segment of this URL, `the-breadcrumb`, you will arrive at the blog homepage. 

Often, site designers ignore this criteria and create meaningless URL segments, like `/how-to/create`, where there is no `/how-to` page. The breadcrumb forces the site designer to consider this architecture. What is `/how-to` and why does it exist on the website? What content does it contain, and how is that content unique from other sections of the website, like `/guide`. As Nielsen explains,

> Breadcrumbs are useful only if you can find a way to show the current page's relation to more abstract or general concepts.

So the breadcrumb forces us to consider those abstract concepts. This is a difficult exercise, as it involves creating an information architecture for the website. Some website architectures are obvious: `/blog`, `/docs`, `/authors`. But in a growing website will create questions: _Where do we put legal? Should we separate announcement from blog posts?_ This requires some serious thinking. If you're at that point, I would recommend the book _Everyday Information Architecture_. Then, once you've mastered IA, you can return to the breadcrumb.