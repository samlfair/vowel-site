---
date: 2024-10-18
breadcrumb: Send Me
---

# Vowel Now Sends Webmentions

Vowel now has rudimntary support for [webmentions](https://indieweb.org/Webmention). This allows your website to communicate with the rest of the internet.

Webmentions are essentially messages between websites, turning the internet into a social network. Before webmentions, if you wanted to comment on a web page, you would post a comment there directly. Commenting systems require complicated back-end infrastructure and systems to identify users, which drove massive consolidation in web publishing around a few social networks. Large social networks let you interact with the content that other people share by keeping you trapped in their closed ecosystem.

So webmentions make it possible for very simple websites to host comments. How? By letting the commenter publish the comment _on their own website_. The commenter publishes a link to the content they want to comment on, along with their own comment, and then they send a "webmention" to alert the original website about their comment. This circumvents the need for logins and comment boxes. Everyone who uses webmentions can display "comments" below their posts.

With the latest version, Vowel will scan your content for any links to other websites; check if those websites have webmentions; and send a webmention to the ones that do. (This is actually a two-step process. First, Vowel will scan for links. Later, the next time the website is published, Vowel will send the webmention.)

I'm also working on displaying webmentions at the bottom of pages. Right now, Vowel will just display a URL. In the coming days I'll flesh that out with titles, descriptions, and images. One part of that work is [implementing](https://github.com/samlfair/vowel/commit/875b5092e5cf050149114ba31e1972a9c0f1dfa7) proper [microformat markup](https://indieweb.org/microformats). This creates structured data from your content.

For now, let's give it a test. Here's a link to a blog post I wrote recently about choosing 35mm film:

https://www.littlefair.ca/photography/film

If the system is working properly, a webmention should appear at the bottom of that page after I publish both sites.

_Edit: I can see that the website has updated properly, and it's earmarked the new link. Now, I'll redploy the website. This time, it should send the webmention._

_Edit 2: The webhook didn't send properly. Upon investigation, I see that it's because I had hardcoded the webmention URLs. Hopefully I've resolved that problem! I will now try redploying to see if it works for this blog post of photos from Paris:

https://littlefair.ca/photography/adieu
