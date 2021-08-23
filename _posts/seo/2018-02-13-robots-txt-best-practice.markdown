---
layout: post
redirect_from: 
- /webmaster/robots-txt/
title:  "Robots.txt : Best Practice"
permalink: /robots-txt/
category: SEO
description: Learn how to implement correct robots.txt in your website with example.
---
Well, I am writing this post, just because you should aware all about the robots.txt, There are many of pro blogger, who does not know how to use proper robots.txt in own website, and posting wrong thing about the robots.txt. So here I am going to tell you how to implement the right Robots.txt in your website or WordPress blog.

Before we start, let’s talk about Robots.txt.

## What is Robots.txt? ##
Well, this is standard guidelines, which all bots should follow, let’s take the example of Googlebot, if your website contains some files, in one directory say example.com/files/, and you don’t like to crawl that directory by Google then you can simply add this robots.txt as an example.

    User-agent: Googlebot
    Disallow: /files/

So Google never goes for crawling those files in that directory.

Let’s say, you don’t want to block only one file from that folder, then you can use this robots.txt as an example.

    User-agent: Googlebot
    Disallow: /files/file-name.txt

So Google does not crawl that file only on your website, but it can crawl other files from same 'files' directory.

## Where to place robots.txt ##

It should be in your root directory, no matter, you have installed your WordPress or Joomla blog in a subdirectory, if you placed somewhere else, then all bots, never know about it. Keep in mind, search engine always first looks this http://example.com/robots.txt, then go for the crawling. If they did not find out robots.txt in the root directory, then they are simply assigned, you have allowed them for crawling anything.

Now, let’s talk about polite and impolite bots.

## Polite bots vs. Impolite bots ##

Mainly all the search engine bots like Googlebot, Bingbot, Baidu, Yandex, are considered as Polite bots, they strictly follow the standard robots.txt guidelines. For example, when you implement this in your robots.txt guidelines.

    User-agent: *
    Disallow :/

So All these polite boys, don’t crawl your site, because you have entered the * asterisk sign with your User-agent name.

Now, there are lots of Impolite bots (or say remaining bots), like HTTtack(For Website copy), dot-bot(Moz bot), ia_archiver(alexa bot), they don’t follow the standard guidelines strictly as like polite bots follow, that means they just ignore the * notation. To block those impolite bots, you should include their User-agent name in your robots.txt.

For example, if you don’t like Alexa bots, to crawl your website, then you can add this robots.txt as an example


    User-agent: 
    Disallow: 
    User-agent: ia_archiver
    Disallow: /

So above robots.txt say, we allowed all polite bots to crawl our website, but we don’t allow to crawl Alexa bot, in our website.

But here is note that, there are many of impolite bots, which can still access, your website, so you just need to enter all the User-agent name to prevent crawling from specific bots. In this article I blocked many of  [SEO bots](/block-seo-bots-in-robots-txt/ "Block SEO Bots using robots.txt"), to crawl my website.

## Let's see some FAQ on robots.txt ##

### What should I use Disallow or Allow? ###
    User-agent: *
    Disallow :
    or
	User-agent: *
    Allow : /

Both are same, but I recommended to use disallow, because this guideline followed by all the user agent name.

### What if I did not block anything in robots.txt? ##
Well, if you did not block anything, then many of bots crawl your website, and start consuming your server bandwidth once you are getting popular. So it is good practice to allow only specific bots to crawl your web pages, and block remaining bots.

### Can I use this robots.txt? ##
    User-agent: *
    Disallow :

Well, it is better to not use any robots.txt. Well, I have seen many of website owners using this robots.txt

    User-agent: Googlebot-Mobile
    Disallow: 
    User-agent: Googlebot-Image
    Disallow: 

If you note that, here is nothing you have blocked anything for those User-agent, so it is better to not include them in your website.

**I generally prefer to use robots.txt to stop crawling into the specific directory or file. Not for anything.**

Let’s take one example of Wikipedia.

    User-agent: Mediapartners-Google*
    Disallow: /

Here Wikipedia block the Mediapartners user agent, just because they are not using any ads on its website, so they can save some bandwidth, so it is good practice to block certain bots, that are not useful for your website.

Similarly, if you think your website is not targeting internationally, then you can block Yandex bots, from crawling, it will also help to save more bandwidth.

### Why Google index my some of pages, which I blocked in robots.txt? ##
Normally, when internal or external web page, pointing to your blocked resources through hyperlinks, then Google go for crawling, but you have blocked it by using robots.txt, So they just provide a simple snippet like this.

<img class="img-responsive" alt="Google Analytics block crawling" src="https://cdn.goyllo.com/seo/Google-analytics-block-crawling.png" title="Google Analytics block crawling" />

So, if you did not want to index at all, then just use a  <a href="https://support.google.com/webmasters/answer/93710?hl=en" rel="nofollow" target="_blank">noindex</a> tag in your specific page. This is the most preferred solution for any webpage.

### I want to block only pdf files, not all the things, How to do? ###

    User-agent: * 
    Disallow: *.pdf

You can use asterisk sign before the file extension name to block only specific file type like .jpg or .png etc. But why you want to do that? Leave your comment, maybe I have another option for you.

### Can I add sitemaps in my robots.txt? ##
Yes, go ahead, there are many of rip search engine like ASK, they don’t have the option to submit a sitemap, but once they land on your website, and check your robots.txt, and found out sitemap link, then they regularly visit your website. It is good practice to add a sitemap into robots.txt. You just need to add this line at last.

Sitemap: http://www.domain.com/sitemap.xml


### How to block multiple robots.txt ###

Well, if you are not targeting your website internationally, and useful for only local search engine say only in Google and Bing, not in Baidu (Chinese Search Engine) or Yandex(Russian Search Engine), then you can use this robots.txt, it will help to save some bandwidth.

    User-agent: *
    Disallow: 

    User-agent: Baiduspider   
    User-agent: YandexBot
    User-agent: Baiduspider
    User-agent: Baiduspider-image
    User-agent: Baiduspider-video
    User-agent: YandexBot
    User-agent: YandexMedia
    User-agent: YandexImages
    User-agent: YandexBlogs
    Disallow: /



## Robots.txt Security ##

I want to say never ever block sensitive or secret folder by using robots.txt, because you have blocked those files and folder in the eyes of the search engine not in human eyes. Many smart people, just open your robots.txt and easily can find out what you have blocked, and read out all the secret documents. So always password protect your specific directory or use .htaccess functionality to prevent access to files/folder. Also, Google said we can’t crawl password protected directory.

## Robots.txt for WordPress ##
After researching a lot, I can say you just need to add this lines in your WordPress robots.txt. Also you can [block some of SEO bots using robots.txt](/block-seo-bots-in-robots-txt/ "Block SEO Bots") .

    User-agent: *
    Disallow: /?s=*

Yoast has updated its article on this  <a href="https://yoast.com/wordpress-robots-txt-example/" rel="nofollow" target="_blank" >page</a>, and he says, we only need to block /wp-admin/ directory and use noindex tag or X-Robots tag to stop displaying results on Google search. If you block other WordPress directory, then Googlebot cannot access your CSS and JS files and you will see different rendering result in Google Search Console.

But Google has recently updated its  <a href="https://support.google.com/webmasters/answer/93710?hl=en" rel="nofollow" target="_blank">article</a>, and say if you block certain directory or files by using robots.txt, then we can’t see the noindex meta tag under those blocked directory, so I did not think, you should block /wp-admin/ directory **with meta tags together**. 

Also, there are many of the WordPress directory like  `/cgi-bin, /wp-content/plugins/`, these types of directory if you did not block, then don’t worry, it will not be indexed by Google until, some links are not pointing to those directories. But if you want to block, then go ahead, and test out your robots.txt in Google search console.

## Check your robots.txt in Google search console ##
I hope you have created your own robots.txt, check out  <a href="https://www.goyllo.com/robots.txt" target="_blank">mine</a>, for some reference. Now it’s time to  <a href="https://www.google.com/webmasters/tools/robots-testing-tool" rel="nofollow" target="_blank">check out our robots.txt in Google Webmaster Tools</a>.

I hope you get my all points, Thanks for reading. Feel free to ask your question in the comments.
