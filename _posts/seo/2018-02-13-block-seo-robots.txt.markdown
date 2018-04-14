---
layout: post
title:  "How to Block SEO bots Using Robots.txt? "
permalink: /block-seo-bots-in-robots-txt/
category: SEO
description: Learn how to block seo bots using robots txt and say bye bye to your competitors for spaying in your website.
---
Hello guys, I know many of Expert Marketers using many of SEO tools like SEMrush, Market Samurai and Majestic SEO to rank higher over its competitors. But did you ever note, how these tools are working? How they get information from most of site? But surely you will get the hint from the title of this page.

Actually, this type of SEO tools, used bots, to crawl your web pages, just like <a href="https://support.google.com/webmasters/answer/182072?hl=en" rel="nofollow" target="_blank">Googlebot</a> does. Please refer this article to know more about [Robots.txt](/robots-txt/ "Robots.txt")

Many of people just uses this robots.txt in his/her site.

     User-agent: Googlebot
     Disallow:      
     User-agent: Bingbot
     Disallow:
	 User-agent: *
     Disallow: /     
 
In the last * indicates all the **polite bots**, i.e. only Googlebot and Bingbot, can crawl your webpages, other Polite bots like Yandex, Baidu, Ask, Yahoo and AOL will not crawl your site. And it is surely helpful to save your bandwidth by blocking other non-useful bots. But **Impolite bots** like HTTrack,Semrushbot,MJ12bot and rest of all bots ignore the * notation, but you can disallow it, by specifying its user-agent name. Just look out below robots.txt

     User-agent: Googlebot
     Disallow:      
     User-agent: Bingbot
     Disallow:
	 User-agent: HTTrack
     Disallow: /
	 User-agent: *
     Disallow: / 

In reality, there are many of sites, are not included Robots.txt in the root of the directory, so for this reason any of bots, can crawl your all web pages. And almost all SEO bots, crawl your web pages, if you’re not disallowing them with its User-Agent Name, And this SEO bots, collect all the web page information like keywords and links, and sell to the third parties. For example **Market Samurai Tools using the <a href="http://www.noblesamurai.com/blog/uncategorized/new-market-samurai-update-allows-you-to-choose-between-majestic-seo-yahoo-for-backlink-data-2288/" rel="nofollow" target="_blank">Majestic API</a> to display the competitors keywords and Link information**. And Majestic API collects all the information using the <a href="http://www.majestic12.co.uk/projects/dsearch/" rel="nofollow" target="_blank">Mj12bot</a>. So if any of site owner block the Mj12bot, then Market Samurai does not give the accurate information about that site. And hence sometimes user of market samurai said, "This tool sometimes displays zero backlinks for some competitors, but in reality the competitors are in the top position". So the reason behind it, your competitors block this type of Bots, in the robots.txt. And you can also do the same.

So, here is some guidelines, which will help to block the SEO bots, so your competitors do not get any information about your site. And your position will be safe in the search result. Also note that When you registered yourself in Majestic SEO, Site Explorer site,SEMrush Audit Tool, then they will forced to allow to crawl your web page, hence your site information will be a help to others, and others registered member information will help to you. So it is the Game of SEO. So for this reason I never registered on any site to Increase my SEO, or to check my competitors rank. Anyway, look out the below Robots.txt

## Block Semrush Bot in Robots.txt ##
	 User-agent: SemrushBot
	 Disallow: /

## Block Majestic Bot in Robots.txt ##

     User-agent: MJ12bot
     Disallow: / 

## Final Robots.txt for SEO ##

     User-agent: MJ12bot
     Disallow: /     
	 User-agent: SemrushBot
	 Disallow: /
	 User-agent: SemrushBot-SA
	 Disallow: /
     User-agent: rogerbot
     Disallow:/ 
     User-agent: dotbot
     Disallow:/ 
     User-agent: AhrefsBot
     Disallow: /
     User-agent: Alexibot
     Disallow: /
     User-agent: SurveyBot
     Disallow: /
     User-agent: Xenu’s
     Disallow: /
     User-agent: Xenu’s Link Sleuth 1.1c
     Disallow: /

Here is note that, there are many of <a href="http://www.robotstxt.org/faq/blockjustbad.html" rel="nofollow" target="_blank">bad bots</a>, which does not follow the any robots.txt guidelines even when you specify its User-agent name. So Here I did not mention the bad bots because it is worth to mention.

But I think bad bots, does not sell the information to the right third parties. They use it for the own purpose and that is illegal. Also the popular marketing companies never buy the information from the bad bots. So I think above Robots.txt will surely help to you if your competitors using Market Samurai, SEMrush or any other tools, which are used above bots, to crawl your web page. If you find any other marketing tools, then you can surely find out it's bot name from the resource documents, and you can block it :)
