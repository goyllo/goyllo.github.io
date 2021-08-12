---
layout: post
title:  "How To Show Post Title First Before Blogger Blog Title In Search Results?"
permalink: /show-post-title-first-before-blogger-title/
category: BlogSpot
description: Step by step guide to display your blog post name first then your blogger blog name into search results.
---
By default, blogger shows the blog title name first, then your post title name i.e. Blog name: post title. But if your blog name is too long, then Google surfers, don’t see your full post title name, because Google only shows the first 66 characters in search snippets, other characters will automatically ignore. So you have only two options, first one is, make your blog name or title shot, or use the below blogger technique to show your post title name first, then your blog name.

## Changing blog post title first before blog name. ##

First off go to template option then click on edit html option.<img class="img-responsive" alt="Blogger Template - Edit HTML" src="https://cdn.arjunsinh.com/blogspot/blogger-template-edit-html.png" title="Blogger Template - Edit HTML" />

Then Find out below code.

    <title><data:blog.pageTitle/></title>

Then Replace the above codes with below codes.

    <b:if cond='data:blog.pageType == &quot;item&quot;'>
    <title><data:blog.pageName/> | <data:blog.title/></title> <b:else/>
    <title><data:blog.pageTitle/></title>
    </b:if>

Click on save changes and visit your any post from browser, you will see your blog post title first, then your blog name. Don’t worry, you will see the same search result when Google index it.

### Useful guidelines for your old blog post. ###
Well, by following above steps, your new post will show something like this blog title: blog name, but what about your old blog post? It already index with blog name: blog title, so we should fix it. If your blog post link is internally linked to your other post, just like Wikipedia does in articles, then Google will update your blogger results in a few days, otherwise it will take some times to update automatically. But if you want quick result, then follow the simple steps.

#### Steps to update your old blog posts. ####

**Useful for many blog posts: It will take some time, may be a few days or months.**

I hope you already [submitted your blog/website to Google Search Console](/add-website-to-google-search-console/), Now just fetch your blog URL to <a href="https://www.google.com/webmasters/tools/googlebot-fetch" rel="nofollow" target="_blank">Google webmaster fetch Tools</a> and submit it to index. In a few days your all old blog post will updated in search result.

**Useful for few blog posts: Instant result in fewer hours.**

You can submit your old specific blog post URL to <a href="https://www.google.com/webmasters/tools/submit-url" rel="nofollow" target="_blank">Google Webmaster tool</a> (GWT), this will update your old post in few hours. But you need to submit every URL to GWT, and it will take some times, hence do this only if you have only a few posts in your blogger dashboard, and want quick results in Google search.

## Does changing orders help in SEO? ##

Yes it does slightly because Google score any document based on when keywords is  appear, if it appear first then it gives better score. So by using this trick your main keyword i.e. your title will appear first, and that's how it helps in SEO, but as I said it's not help heavily. 
