---
layout: post
title:  "How to Change your Blogger/Blogspot URL Address?"
permalink: /change-blogspot-url-address/
category: BlogSpot
description: Learn how to change your Blogger/Blogspot URL address step by step.
---
If you did mistake by selecting the wrong username for your blogger blog OR you may not like your current Blogspot URL address, and you want to change your Blogspot URL address ( from example.blogspot.com to somethingelse.blogspot.com), then follow below steps. 

## Steps to Change your Blogspot URL Address. ##

1. First off go to your blogger dashboard.

2. Click on setting option from the left side menu, then select the basic option.

3. Now click on edit option and enter your new blog URL Address.

<img class="img-responsive" alt="Change your blogspot URL address" src="https://cdn.arjunsinh.com/blogspot/change-blogspot-url-address.png"><br />

You should note that by changing URL address may cause many problems if you blog is already getting traffics from social media or search engine like Google and Bing. For example, let’s say you have shared your blog post on Facebook and you’re getting daily few clicks from it. Now if you change your blog URL address to something else then that visitors will see 404 Error page, means page not found. Same thing applies if you’re getting traffic from Google or Bing search results.

There is two solution about that. 

*Remember that, you need to do these things only if your blog is getting tons of traffic, so if your blog is new then feel free to skip all things, because you're getting very less or no traffic at all. So there is no need to redirect your visitors from old blog to new one.*

1. If you’ve blog `example.blogspot.com` and you want to use different URL address, then buy a custom domain name for your blog(like goyllo.com), which will do proper 301 redirection automatically from `example.blogspot.com` to your `www.domain.com`. It will do redirection at nested level like from `example.blogspot.com/2017/06/some-post.html` to `www.example.com/2017/06/some-post.html`

2. Use meta refresh tag in your `old.blogspot.com` template so that it will redirect your all visitors from `old.blogspot.com` to `new.blogspot.com`. *If you can’t create a new blog with old username, even after changing its username, then use import/export functionality and let your old blog as it is*. This solution does not do proper 301 redirection. It means your `old.blogspot.com/2017/06/some-post.html` and all other pages will redirect only to your `new.blogspot.com` It does not support nested level redirection because it is client side solution and works on the browser side.<br/> `<meta http-equiv="refresh" content="0;URL='http://new.blogspot.com/'" />`<br/>
This tag should be placed in your old blog template. To do that go to the theme option from your blogger dashboard >> Select Edit HTML option >> Place above Meta Tag anywhere into head section (from `<head>` to `</head>` anywhere).

Add your comments if you need any help :) Have a good day :)
