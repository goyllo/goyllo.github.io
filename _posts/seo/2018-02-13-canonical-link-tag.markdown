---
redirect_from: 
- /webmaster/seo/canonical-link-tag/
- /seo/beginner/canonical-link-tag/
- /webmaster/seo/beginner/canonical-link-tag/
- /webmaster/seo/beginner/canonical-url/
- /webmaster/canonical-link-tag/
- /seo/technical/canonical-link-tag/
layout: post
title:  "Basic of canonical link tag - SEO guide"
permalink: /canonical-link-tag/
category: SEO
description: Understand How Search Engine treat canonical link tag, and How you can implement in your website.
---
The canonical link tag is strong hint for search engine (<a href="https://support.google.com/webmasters/answer/139066?hl=en&rd=1" rel="nofollow" target="_blank">Google</a>,<a href="http://www.ysearchblog.com/2009/02/12/fighting-duplication-adding-more-arrows-to-your-quiver/" rel="nofollow" target="_blank">Yahoo</a>) to which page link or which preferred URL we want to index in search result among all other duplicate URLs.

Actually, many of website have same content with a different URL, for example


    www.exmple.com/page-1.html
    www.example.com/page-2.html

Page-1 and page-2 both have the same content, so we should tell the search engine to don’t index both the pages, if you don’t do that, then you will get punishment from a search engine, because you are displaying same content, with different URL’s. Now,

## Let's implement canonical link tags in our website ##
No matter, if your site having single webpage or many web pages, you're all the web pages should contain canonical link tags properly.

Canonical URL must be implemented **only once** between `<head>` and `</head>` tag, if you put the canonical tag on `<body>` section, or using two times canonical tags, then it will not work.


    <link rel="canonical" href="www.exmple.com/page-1.html" /> //page-1.html
    <link rel="canonical" href="www.exmple.com/page-1.html" /> //page-2.html

So here I implemented same canonical URL in page-1.html and page-2.html, and so whenever the search engine spider comes to page-1 html then, they will notice the canonical tag and it is same as page-1 URL, So Google will index that page URL in search result. And when, search engine spider goes to the page-2.html then it is noticed, the canonical tags, that is linked to another page (i.e. page-1.html), so they will assign page-2.html is duplicate URL, and follow the canonical(i.e. page-1.html)URL, so search engines will only index the page-1.html and ignore your all other duplicate content to index. I hope now you get the idea of canonicalization.

Many of people assume, they have no duplicate URLs for the same content, but technically these URLs are different,

    www.example.com/mypage
    www.exmple.com/mypage.html
    www.example.com/mypage/
    example.com
    https://www.example.com


So if you did not setup redirection between them, and mention some of the links with www, https, and trailing slash, and others without www, https and trailing slash, then Google can index both version in search result. So for a best practice you should include canonical URL tags in every webpage. So search engine can understand which preferred URL, you want to index in search result. So first off search your site on Google, and check out your all webpage’s URL, Are you satisfied with it or not?. If not, then you should do canonicaliation in your website into head tags. If you did not setup canonical URL tag, then Google can automatically pick up best URL as per how many times your links are referred from other webpage’s, so many times, people link to `goyllo.com/canonical-link-tag/` URL, thank god it is redirects to my proper URL `https://www.goyllo.com/canonical-link-tag/` automatically, otherwise Google index both the pages in search result, and it is very bad sign in SEO. So canonical tags, many times helpful in many ways, so you should include it in your website, or in your blog by using third party plugins or widget. Google uses, your canonical tags many times, when people point your website and forgot to add slashes at the end of URL, also forgot to mention www subdomain and https in URL. So **your juicy link (PageRank) will only go to your preferred version (canonical URL), it will not distribute to other version**. Yes, you can also do 301 redirection to save your PageRank, but you need to setup manually, for all the situation, but once you setup canonical tags, you did not worry about all the redirection option across www, non-www, https, trialing slash etc. Also, you did not worry about how your page is linked from another source, Google does its job very carefully to save your important pages.

Note:- Don’t set a canonical tag in such URLs, which redirect to another URL, for example, If people forgot to mention slash at the end in this URL<br/>
`https://www.goyllo.com/canonical-link-tag` <br/>
then it will automatically redirect(301 redirection) to this URL
`https://www.goyllo.com/canonical-link-tag/`<br/>
So it is good practice to use second one URL for canonicalization.


> ProTip: - Stick with your canonical URL everywhere, for example in internal linking and in your website sitemap (XML).

More Resource: - <a href="http://googlewebmastercentral.blogspot.in/2013/04/5-common-mistakes-with-relcanonical.html" rel="nofollow" target="_blank">Official Google Webmaster Central Blog</a>
