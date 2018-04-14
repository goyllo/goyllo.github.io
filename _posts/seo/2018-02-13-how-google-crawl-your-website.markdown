---
layout: post
title:  "How Google Actually Crawls your Website?"
permalink: /how-google-crawl-your-website/
category: SEO
description: This basic tutorial about Google crawling will help you to become a master in SEO.
---
Google has many <a href="https://support.google.com/webmasters/answer/1061943?hl=en" target="_blank"> types of crawlers</a> to index web content for example, Googlebot, Googlebot-image, Googlebot-news, Googlebot-Video etc., but first let's see

## What is web crawling?  ##

Crawling is nothing but a simple process which copy or you can say download our website content and save it on some computer/server.

It is simple like you save some web pages on your computer, and later you can find those pages with your computer search button. But saving billion of data’s is not our computer job, Google have a big data center, which saves thousand of gigabytes (GB) content daily on their data center. Here we are not talking about How Google works, we just want to know how [Google complete it's First phase which means crawling](/crawling-indexing-and-ranking/ "Google three phase: Crawling, Indexing and Ranking"). 

The Google main bot/spider/crawler is [Googlebot](https://support.google.com/webmasters/answer/182072?hl=en), which crawl any webpage first time, if they found particular website or webpage contain only images, then next time Googlebot-image will crawl that particular web pages, and similarly, if Google finds out those pages contain videos (like YouTube site contain) then Googlebot-Video will handle that in future crawling and for a news website, Googlebot-news will do its job. But most of the first time, Googlebot will crawl your website or blog, because we have mainly text content.

And there are [some old crawlers which Google was using in 1998](http://oak.cs.ucla.edu/~cho/papers/cho-order.pdf), and later added many of crawlers which don't depend on links.

## Old and Efficient Crawlers to crawl, important web pages first ##

**Crawler Based on Links:** Google main abstract about crawling is to - crawl important pages first, so how do they find out important pages, the simple answer is, via backlinks, it means if I link to some other web pages in my article then it is considered as important pages so which should be indexed faster. But links have different value, if I link to your article then it will going to crawl slower compare to if Google homepage link to you. Google also follows your internal links, it means if your home page is listed with new articles within your website then Google will crawl that URL from your homepage. In simple Google follow the links to crawl all of the web pages.

**Crawler based on PageRank:** PageRank is still used by Google internally, and it is still an important factor. When we links to some web pages, then few amount of PageRank will pass on that link, it means if you have a higher PageRank, the more Google will crawl that webpage. Wikipedia crawls often because their PR is high (You can’t check PR now, because it is dead on the toolbar, and if you try to check then you will get old/outdated value).

These both crawlers are still very important, so those websites who have Good backlinks and Higher PageRank are still **crawled first and automatically** compare to below crawlers.

## New and Sufficient crawler to crawl, more web content. ##

**Crawler based on sitemap:** There are many web pages will not be crawled by Google if they simply rely on links, so they have implemented sitemap crawler, so new webmaster can submit their sitemap into Google search console, so Google will crawl their site regularly, when new URL is published on the sitemap.

**Crawler based on webmaster request:** We know many times we change our content in website, and we want to invite Googlebot again to see that changes, so now webmaster can request, [fetch and render tools from search console](https://support.google.com/webmasters/answer/6066468?hl=en), to request re-crawl that pages again. You should note that it should take some time, it’s purely based on how many webmaster request same thing in one day to Google server. Google process only limited request on one day, other request will be processed on the next day and so on…. It means your URL will be on Google crawler queue, you just have to wait, it does not crawl in hours.

**Crawler based on old pages:** Once Google crawls any webpage, it will be stored on their data center, and they will continually check your old pages to see if any changes are made. Yes,  they will crawl the same web page again, even if you did not link/remove URL from anywhere also not included in your sitemap, but still it will be crawled by Google, because Google already have information about that URL and they want to check whether that page updated any information or not.

**Crawler based on popularity of webpage:** This type of crawler has also existed, but I don’t have more information on that. I just want to say, they may use other Google product information to index that kind of content, for example, User history who uses Google Chrome, User who uses Google public DNS, User who uses Google Cloud etc. It is just my assumption, I am not 100% sure, but if the content is getting viral or popular then Google will find out automatically, that’s what I want to say.

## Most important thing about Google Crawlers ##

Major search engine Crawlers don’t crawl your whole website in just one time because there are billion of web pages, Google need to crawl them on a regularly basis. They have distributed their works and add your URLs on the queue, so you have to wait for the next crawling, it is not like your whole website with 10k pages will crawl in one day, it can take up to a few weeks, and if it is very big website and have lower backlinks and PageRank, then it can take up to months

## How to Block Google Crawlers? ##

There is also some situation on which you need to block any webpage or whole directory, for example login pages, affiliate/ads directory or some kind of demo pages, so there are some technique to [block crawler to particular directories via robots.txt](/robots-txt/), or to the [particular webpage using meta tags and x Robots tags](https://developers.google.com/webmasters/control-crawl-index/docs/robots_meta_tag). 

But one thing you should note that, the password protected directory will not going to crawl, also the CGI directory will also not crawl by Google, because sometimes it generates an infinite number of pages, which can keep busy Googlebot for many times. So generally Google has set up some kind of algorithm to avoid such thing, it means they stop crawling such a thing who generates web pages automatically. 

## Few notes on Google Crawler. ## 

- Google always checks your robot.txt first before they start crawling your website.

- Crawling is not ranking factor, It’s just [one phase of Google to know about your content](/crawling-indexing-and-ranking/).

- Google doesn’t pass the PageRank to a blocked directory (via robots.txt).

- Google will not see your meta tags like noindex, nofollow if it is blocked by robots.txt


