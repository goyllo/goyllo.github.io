---
layout: post
title:  "Jekyll vs Wordpress"
permalink: /jekyll-vs-wordpress/
category: Jekyll
description: Here, is my personal review about Jekyll vs Wordpress, and Why I like jekyll over WordPress.
---
Jekyll is static site generator based on ruby programming language. If you love to write codes then this is fantastic blogging platform for you. But it is not easy to setup, also you should ready to waste some of time to make things works, while in Wordpress everything is ready maid. But Jekyll may give you many benefits like below.

## Speed ##
The speed of any static site generator is can’t beat by any CMS. Because static site does not wait for process like executing query on database. If you are a WordPress developer, then you will note, every time, whenever any page is loaded, then the query is executed on the database server and hence it’s taken some millisecond (ms) to process those queries. So, the modern static site generator like Jekyll, Hugo, Hexo is too fast compared to any CMS.

## Security ##
No SQL query, No database. It's simply secure your website from SQLI (SQL Injection) leet or 1337 or Master, because there is nothing to **inject**.

## Custom permalink for a specific post ##
Jekyll support all the permalink features that WordPress gives you. Also you can setup your own custom permalink in any post. For example

    Permalink: test1/test2/test3/custom-title-of-post/ 

Output will be look like this.

    www.example.com/test1/test2/test3/custom-title-of-post/

First, I was using categories into my permalink but after finding this solution, I can use any of permalink for my post. Even I can set two different permalinks for two different posts. For example


    Permalink: test1/test2/test3/custom-title-of-post // post 1 permalink
    Permalink: 2015/06/custom-title-of-post           // post 2 permalink


It's not awesome? Where In WordPress, Once you choose any permalink format, it's applied to all posts, but in Jekyll you can customize it.

## Custom layout for a specific post ##
I am not a master in WordPress, so I don't know really much more about the post layout in WordPress, But Does WordPress supports different layouts for different post? Absolutely not. It's painful for WordPress developers, where in Jekyll you can. For example.

You have posted many things in your blog, and places some ads or newsletter or something else in your site sidebar, but not all the peoples are interested. For example, if you post articles about blogging then blogger will click on it and you get maximum results from blogger visitors, because it is relevant to him/her. But what about the other peoples? Your sidebar is simply displayed in all your posts, and it is fixed. But what happens if you can change the sidebar layout according to your post. For example, in blogger post you can display blogger layout and for social media tips you can display other layout. It's not awesome? Not only sidebar but you can create your own layout for any post. You just need to specify which layout you want to use for your post in single line, like this.

    Layout: Post              //I used this layout for my posts
    Layout: Page              //I used this layout for my pages like about 
    Layout: Directory         //I used this layout for directory like /google/
    Layout: NoAds             //I used this layout if I don't want to display ads
    Layout: Blogger           //I used this layout for blogger post only 

## Custom Directory ##
Well, this is what I loved about the Jekyll, as I said above I can create custom permalink as per my choice, but you can even create your own directory and you can put anything you like from simple about us pages to very complex directory like categories and tags pages. Even you can list (Blog Posts) from two/many different categories into one page.

## Powerful Backup ##
There are two different scenarios in the backup process. In WordPress, user write the post and publish it. Most of all user backup its data weekly, and some of pay for backup to host provider. Where in Jekyll, you can test your post in local host, and most of them, including me test out the post in local host first, and then deploy it to server. So you have already backup of your all posts in local machine. So whenever you need to change the host server, just upload all the data to new host. No other cost is required.

## Developer Team ##
WordPress developed by master of master. They assign code is poetry. But there are many of plugin developers, they charges for the plugin, but in Jekyll, all the developers are free to help. Even I was finding all the necessary codes from stack overflow and github, and then I am changing it according to my need.

## Github-Pages Support ##
Well, <a href="https://pages.github.com" rel="nofollow">Github pages</a> provide you free hosting for Jekyll. With Github pages, your site use Github CDN (Content Delivery Network). It will accelerate your website access and delivery web pages from different location. Currently I am also using Github pages, to host this website, but later I am thinking to use the Amazon S3 cloud.

So, this is just a small comparison between **Jekyll vs Wordpress**, If you know some few basic of HTML then I highly recommended to give it try to static site generator like Jekyll, Hugo or any others.
