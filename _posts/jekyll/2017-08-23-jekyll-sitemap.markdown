---
layout: post
title:  "Generate Jekyll XML Sitemap Manually Without Using Plugin"
permalink: /jekyll-xml-sitemap/
category: Jekyll
description: Learn How to generate jekyll XML sitemap automatically with plugin and without plugin.
---
In this post, I will tell you, how to generate an XML sitemap without using any <a href="https://github.com/jekyll/jekyll-sitemap" rel="nofollow" target="_blank">plugin</a>. Most of people use Jekyll because of flexibility, in above plugin, you can’t customize your XML sitemap, but if you make your own code, then you can play with your XML sitemap, so here is code, that I used in my website, just copy it and **save the file name as sitemap.xml**

	{% raw %}
    ---
    layout: null
    sitemap: false
    ---
    <?xml version="1.0" encoding="UTF-8"?>

    <urlset xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9 http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd" xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
    
      {% for page in site.pages %}
    	{% if page.sitemap != false %}
      <url><loc>{{ site.url }}{{ page.url }}</loc></url>
    	 {% endif %}
      {% endfor %}
    
      {% for post in site.posts %}
    <url><loc>{{ site.url }}{{ post.url }}</loc></url>
      {% endfor %}
      
    </urlset>
	{%endraw%}

In the above code, I used this code  `{% raw %}{% if page.sitemap != false %}{%endraw%}` because, such pages like feed.xml, sitemap.xml and main.css is consider as pages on Jekyll, and that pages is not helpful to include in our sitemap.xml file, and hence such a page, you can exclude from the sitemap, just by using this front matter.

## Front Matter to exclude some Jekyll pages. ##
	{% raw %}
    ---
    layout: 
    sitemap: false
    ---
	{% endraw %}

So, whenever you include `sitemap: false` line in your front matter, you can exclude that page from your sitemap.

Here is also not that, I did not exclude my post, but if you want, then you can use the same, *if condition* in your post code, like this.

	{% raw %}
    {% for post in site.posts %}
	  {% if page.sitemap != false %}
    <url><loc>{{ site.url }}{{ post.url }}</loc></url>
      {% endif %}
    {% endfor %}
	{% endraw %}
	

Hope it's clear your doubt to exclude pages as well as posts from your sitemap. In general, I don’t exclude my posts in sitemap, so the first one code is perfectly fine for me.

## Extend sitemap Functionality in Jekyll. ##
If you already look out on the sitemaps.org website, then you will see, you can use many of the tags in your sitemap, and that is helpful for search engine to crawl your specific post and page. You can add any addition tags in *for loops* or just after the `<url>` tag.

`<lastmod>` : You can use this tag, if you want to notify to search engine about, when your post is modified, so they can update your page result in the SERP. I am not using this tag, because spider, showing dates in the search result by using sitemap dates, so If my article is too old, then obviously I got less CTR (Click through rate) in SERP, because no one like to read old article. So in my website, I always post evergreen content, that is not changed for many years, and hence I did not use dates in my post, also in the sitemap, but if you want to use, then you can use this code line just after  `<url>` tag.

    {% raw %}<lastmod>{{ page.update | date_to_xmlschema }}</lastmod>{% endraw %}

And this is front matter code for a specific post or page.

     ---
     layout: 
     update: 2015-07-18 12:30:18
     ---


`<changefreq>`: This tag, you can use, if you want to say, this content is frequently updated, like, always, hourly, daily, weekly, monthly, yearly, never.

In general, I did not use this tag, because I don’t want to waste my times, behind this, We generally use XML sitemap, just because, we can index our all the webpages, so the first one code is perfectly fine. But still, if you want to use, for example, in your coupon code site, then here is the code.


    {% raw %}<changefreq>{{ page.sitemapchangefreq }}</changefreq>{% endraw %}

And here is front matter for a specific post or page.

     ---
     layout: 
     date: 2015-07-18 12:30:18
	 sitemapchangefreq: daily
     ---

`<priority>` : This tag, you can use, if you think, this specific Jekyll post or page should be crawled first, then go for others. But again, I am not using this tag, but if you want, then you can use this code.

    {% raw %}<priority>{{ page.sitemappriority }}</priority>{% endraw %}

And here is front matter for a specific post or page.

     ---
     layout: 
     date: 2015-07-18 12:30:18
	 sitemapchangefreq: monthly
	 sitemappriority: 0.8
     ---

Here is note that, you can set priority from 0.0 to 1.0 and by default the value is 0.5 i.e. if you forgot to mention above front matter for a specific post or page in Jekyll, then Search engine spider assigns default priority value.

## Final Question: Where to add a sitemap.xml file on my website or Github pages. ##
Well, it is not necessary to add sitemap into the root directory, you can place anywhere. Just create your own secret folder, and just add the above codes on it, and save it, as sitemap.xml and you have done,  for example, www.example.com/secret/sitemap.xml.

Hope you like this article, feel free to comment, if you have any doubt. Have a good day :)
