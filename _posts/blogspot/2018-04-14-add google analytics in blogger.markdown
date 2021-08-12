---
layout: post
title:  "How to Add Google Analytics in Blogger Blog?"
permalink: /add-google-analytics-in-blogger/
category: BlogSpot
description: Step by step guide to add Google Analytics tracking code to your blogger blog.
---
In this post, I will show you, How to add/install google analytics tracking code to your blogger blog, so you can track how your visitors are interacting with your blog, so let’s first free signup on Google Analytics.

1. Go to the <a href="https://www.google.com/analytics/web" rel="nofollow" target="_blank">Google Analytics Webpage</a>, and click on Signup button.<img class="img-responsive" src="https://cdn.arjunsinh.com/blogspot/signup-to-google-analytics.png" alt="Singup to Google Analytics" />

2. Now, you need to enter your website details. Don’t worry Google Analytic did not provide a different kind of dashboard if you selected any other industry category for your site. Here, standard time zone gives you accurate reports in hours, so do not forget to choose the right time, as per your country name.<br/><img class="img-responsive" src="https://cdn.arjunsinh.com/blogspot/create-new-account-in-google-analytics.png" alt="Fill up your website details in Google Analytics" />

3. Then, Click On Get tracking ID.<img class="img-responsive" src="https://cdn.arjunsinh.com/blogspot/get-google-analytics-tracking-id.png" alt="Get Google analytics tracking ID" />

4. Now accept terms of service. (If you don’t see "accept button" then press CTRL + - (CTRL and Minus) button, to minimize your browser screen size).

5. Now, you will see a tracking code window, like this.<br/><img class="img-responsive" src="https://cdn.arjunsinh.com/blogspot/get-google-analytics-tracking-codes.png" alt="Accept Google Analytics TOS" />

Now you can follow any of one method to add Google Analytic in your blogger blog. The first method might not work for you if you're using custom blogger template from third party website.

## Method 1: Add Google Analytic Tracking ID directly in Blogger Setting. ##

This method is very simple if you’re using Blogger official theme. Because in this method you just need your tracking ID, and blogger will place complete JavaScript code automatically in your theme.

1. Go to the setting menu and then click on other option.<br/><img class="img-responsive" alt="Add Google Analytics ID to Blogger Blog" src="https://cdn.arjunsinh.com/blogspot/Add-Google-Analytics-ID-to-Blogger-Blog.png" title="Add Google Analytics ID to Blogger Blog"/>

2. Now, scroll down a little bit, and you will see Google analytic option, so just place your Analytics ID (for example UA-70093885-1), and click on save settings.

This method sometimes does not work with custom/third party blogger theme, so check your source code to know whether the analytic code is implemented successfully or not.

## How to Check Google Analytics code is implemented successfully or not? ##

First of visit any of your blog URL, and right click on anywhere, and select view page source from browser option. Now press CTRL+F(To find codes) and search your analytic ID, like this.

<img class="img-responsive" alt="Checkout Google Analytics Code in Blogger" src="https://cdn.arjunsinh.com/blogspot/checkout-google-analytics-code-in-blogger.png" title="Checkout Google Analytics Code in Blogger"/>

So if you found your analytic ID, it means you have successfully implemented Google Analytics code. And if you did not find it, it means something is wrong with your blogger theme, and you need to follow the second method.

## Method 2: Add Google Analytics Codes Manually in your Blogger Theme. ##

1. First of go to the template option and click Edit HTML option.
2. Now, Press CTRL+F from your keyboard and find the `</body>` tag in your template, and paste your analytic codes just above it. Refer below screenshot for better understanding.<br/><br/><img class="img-responsive" alt="Add Google Analytics Code To Blogger Template" src="https://cdn.arjunsinh.com/blogspot/Add-Google-Analytics-Code-To-Blogger-Template.png" title="Add Google Analytics Code To Blogger Template"/>

Now, [check out your source page again](#how-to-check-google-analytics-code-is-implemented-successfully-or-not) to make sure, you have implemented code successfully or not. Make sure there are no twice codes. Otherwise, you’ll see double/wrong reports in your Google analytic dashboard. 
