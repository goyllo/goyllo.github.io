---
layout: post
title:  "What is Nofollow Link? - A Complete SEO Guide about nofollow/dofollow"
permalink: /nofollow-link/
category: SEO
description: In this SEO article, we will talk about what is nofollow and dofollow links, and how it impacts in SEO.
---
As an SEO webmaster you may hear lot’s of about nofollow link, so what is that? How it impacts in your SEO? And what is the difference between dofollow and nofollow links? So in this article, we will cover all of your questions about nofollow and dofollow links. So first let’s take your question.

## What is a nofollow link? ##
*Nofollow link is a type of link, on which Google don't pass Pagerank and keyword anchor text to the destination link.*

Still, confused about nofollow? So let me tell you one main point about backlinks. When you add any hyperlinks in your blog post or website, then Google pass some link juicy or Pagerank to that links. The link juicy or PageRank algorithm is a top secret of Google, and you will never know how exactly Google compute it. But one thing is true that, If the particular web page/URL get a large number of quality backlinks, then it will rank higher in the search result because quality links improve PageRank. And PageRank is Google core algorithm to decide which web page rank, in which position. Google don’t rely only on PageRank, they use more than 200 + signals, but still, Pagerank is important ranking factors among them.

It means if I mention any links in my blog post, then that link owner will get some PageRank from my website to his/her website, so the ranking of that website will go high, but what if I want to point some scam or fake website? What about comment links? If those links pass PageRank, then all of that website will get higher ranking in search results, because I point them. And hence Google introduce nofollow attribute, which you can add very easily in your hyperlink (If you’re using any CMS or blogging platforms then look out their official documentation, you may easily find some plugins or option to add nofollow link easily with one click).

    <a href="https://some-unknown-site.com" rel="nofollow">The commenter</a>

So as you can see in our above hyperlink we just add rel attribute with a nofollow value, it means Google don’t pass the link juicy or PageRank to that hyperlink. Here *the commenter* is keyword anchor text, which also collects by Googlebot when they crawl your website. A good keyword anchor text surely helps in SEO, but when there is nofollow attribute, then Google don’t collect that keyword anchor text.

## When to use nofollow links? ##
- If you have a blog, then you should use nofollow link in your comment links; otherwise, lot’s of comment links will drain your main website PageRank. And such a blogs always attract to blackhat webmaster to build backlinks.

- If you have forum website, then you should use nofollow link in external/signature links; otherwise, lot’s of product or marketing webmaster will promote their products to gain ranking benefits.

- If you have a normal website, and you want to point some scam or fake website then use the nofollow attribute.

- If you are doing any paid post(for example sponsor post) in your website/blog then use nofollow attribute otherwise Google may penalize your site for selling links.

## What if you don't use nofollow links in bad links? ##

1. Lot’s of spammer will attract to your site because they have opportunities to build links without nofollow attribute.

2. Too many low-quality links, make your web page quality lower and hence you will get less or zero amount of traffic from search engine result.

3. Too many bad links make your website as a link farm, and Google may penalize your site for having too many spammy links. And such a penalty can kick out your website completely from Google search result pages.

OK, now let's see,
## What is the difference between dofollow and nofollow links? ## 

When there is no nofollow attribute, then the link is considered as dofollow links or follow links. Yes, there is no any `rel` attribute for that, but in case if you use `rel="dofollow"` then it will be simply ignored by Googlebot, just like they ignore your div/span class tag. So When links have no nofollow attribute then by default, it is considered as dofollow links.

## OK, so how nofollow/dofollow link impact in SEO? ##

- So if there is nofollow attribute then no PageRank and keyword anchor text will transfer to that page, it means there is no any SEO value for that link.

- And if there is follow/dofollow links Or in other words if there is an absence of nofollow attribute then by default PageRank and keyword anchor text will pass to that page, and it will impact well in SEO.


## FAQ on nofollow links. ##

**Q. Does backlinks from Wikipedia article help in SEO?**

No it’s not because the link is nofollow, lot’s of people will say it impacts in SEO and will increase your domain authority and blah blah blah, but that’s not true. Nofollow link is purely made to prevent link manipulation score. So if there is nofollow attribute then no matter what the site is, it will not be going to add any direct value to SEO/ranking. But links are links and useful links always drive traffic to your site, so indirectly it helps to your business, but if you concerning about ranking, then again there is no any benefits. So if you’re doing comment backlinks just for ranking/SEO, then you should change your strategy, have you ever seen any PRO webmaster do comments for SEO? No, mostly not.  So do comments on other blogs only to establish a relationship with them.

**Q. Should I use nofollow attribute in good external links as well?**

It purely depends on you. But linking to useful resource actually help you to gain some expertise score. But adding nofollow attribute on good out bounding links won’t hurt you as well.

**Q. Should I use nofollow attribute in internal links as well?**

No don’t do that ever, it will don’t pass Pagerank, but it will [sculpt your PageRank](https://www.mattcutts.com/blog/pagerank-sculpting/) it means your Pagerank will be lost. [Use nofollow](https://support.google.com/webmasters/answer/96569?hl=en) internally only for some specific pages as a sign in and signup pages. Personally, I think Google consider nofollow differently for internal and external links. Nofollow in External links may save PageRank, but same is not true for internal links.

**Q. How to check nofollow links on any website?**

Personally, I use <a href="https://chrome.google.com/webstore/detail/nofollow/dfogidghaigoomjdeacndafapdijmiid?hl=en" rel="nofollow" target="_blank">nofollow Chrome extension</a>, which highlights nofollow link with a red border. But if you're tech savvy then you can also view page source code as well.

**Q. Do Googlebot crawl nofollow links?**

Yes, Googlebot crawl nofollow links, don’t you see the list of all links in your webmaster search console under who links to me option?. It displays nofollow links because Googlebot already crawls those links.