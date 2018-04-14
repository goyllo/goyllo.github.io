---
layout: post
title:  "How to Use Blogger Default XML Sitemap?"
permalink: /blogger-sitemap/
category: BlogSpot
description: Learn how to find your inbuilt blogger XML sitemap. You don't need to use any third party tools for that.
---
A blogger creates a sitemap automatically whenever you published any content on your blog post or page. You don’t need to use any third party tools. But you cannot customize your sitemap manually because it is generated automatically by blogger. Blogger sitemap is necessary when you [add your site into Google search console](/add-website-to-google-search-console/) or Bing Webmaster Tools. So they can easily find your new blog post and index into the search result ASAP. 

This one is your post sitemap 

    www.example.blogspot.com/sitemap.xml

This one is your page sitemap

    www.example.blogspot.com/sitemap-pages.xml

Similarly, you can also find your sitemap for post and pages, just by changing example.blogspot.com name to your blog URL address. If you’re using a custom domain, then your sitemap will be on www.example.com/sitemap.xml location.

Another thing you should note that the blogger sitemap is changed automatically according to your number of blog posts. Look out this guy <a href="http://blogging.nitecruzr.net/sitemap.xml" rel="nofollow" target="_blank"> sitemap</a>. There are multiple sitemaps into the main sitemap.

    /sitemap.xml?page=1
    /sitemap.xml?page=2
    /sitemap.xml?page=3


So initially when your total number of posts is less than 500, then your all post link goes to the main sitemap i.e. `www.example.blogspot.com/sitemap.xml`. But when you post your 501 posts, then, your main sitemap will change i.e. your first 1-500 post will be listed out in `www.example.blogspot.com/sitemap.xml?page=1`, and another 500-1000 listed out in `www.example.blogspot.com/sitemap.xml?page=2` and so on. And all these sub sitemap pages will point to your main sitemap(`www.example.blogspot.com/sitemap.xml`).

So whenever you need to add a sitemap somewhere like Google webmaster tool, then you just need to submit your main sitemap (i.e. `www.example.blogspot.com/sitemap.xml`). You can also submit your page sitemap(`www.example.blogspot.com/sitemap-pages.xml`) if you've many important pages as well. 