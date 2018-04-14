---
layout: post
title:  "Understand Basic of Crawling, Indexing and Ranking"
permalink: /crawling-indexing-and-ranking/
category: SEO
description: Beginner tutorial to understand how search engine like Google, Bing and Yahoo work.
---
Google Search Engine work with these three phases.

1)	Crawling

2)	Indexing

3)	Ranking

## What is crawling? ##

Crawling is nothing but a downloading website content via Google crawler/spider/bot. Googlebot renders web pages just like our browser does, so it can understand your CSS layouts and execute Javascript pretty well. I already wrote a detailed article about  [How Google actually crawl your website](/how-google-crawl-your-website/), it will really helpful for any level of the webmaster.

In some situation, you need to block specific directory/folder from crawling that time you can [use Robots.txt to prevent crawling into a specific directory](/robots-txt/). 


## What is Indexing? ##

The next phase is indexing, and Google has so many big data center which saves all crawled content. Google gives query result so fast because they have the whole internet data on their index data server, so it can search and rank specific things very quickly. Google use <a href="https://googleblog.blogspot.in/2010/06/our-new-search-index-caffeine.html" rel="nofollow" target="_blank">caffeine</a> system to index all crawled data, and they continued to crawl important web pages, again and again, to make their index data fresh. If you click on cached results, then you will know, Google have fresh data about your site or not.

If you don’t like to display particular webpage into Google search results, then you can use <a href="https://support.google.com/webmasters/answer/93710?hl=en" rel="nofollow" target="_blank">noindex header tag</a>. Most Webmasters use noindex tag on low quality or duplicate pages, so Google doesn't penalize their website.

## What is ranking? ##

Ranking is done in real time(When you search any query), Google uses 200+ algorithms to rank any particular webpage. Few algorithms use ON Page ranking factor, and few algorithms use Offline Page ranking factor. And few algorithms are specially designed to give rich experience to users for example company/scientist information on the right side (Knowledge Graph), movies related query or sports score related query.

Those 200+ algorithms give some output separately(We called it document score) and finally it combines the full weight, and then Google shorts out the search results based on highest value to lowest. And then display it on search result page, pro webmaster often called it SERP(Search Engine Result Page) in 
 Short and these all processes Google do it very super fast(Mostly under 1 second), and it is because they have indexed the whole internet world and have an intelligent algorithm to short out the results. If you want more inner details about server side, then please refer this [Wikipedia article](https://en.wikipedia.org/wiki/Google_Data_Centers#Search_infrastructure).
