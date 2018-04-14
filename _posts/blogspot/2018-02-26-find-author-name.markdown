---
layout: post
title:  "How To Find Author Name Behind Any Blogspot Blog?"
permalink: /find-blogger-author-name/
category: BlogSpot
description: The secret trick to find out who owns particular Blogspot blog. Get the blog author name, and Google Plus profile.
---
Sometimes blogger using BlogSpot as a subdomain, so their registration details, we can’t find out from <a href="https://who.is/" rel="nofollow" target="_blank">who is database</a>, also many bloggers use who is protection with custom domain to hide their registry details. Also, some of the blogger does not include their name or profile URL in the sidebar and in below post content. So in this all case, it is hard to find out who owns this blog, 

But normally many of pro blogger, using their own profile to create an anonymous blog and hiding their profile details on the blog post. Also, some of code master remove the rel=author attribute from blogger template, so you cannot find out the name in the source code as well.

But we all know blogger does not give you more control in our blog for example, in [blogger sitemap](/blogger-sitemap/), permalink structure, and ATOM feed :) so blogger can’t edit those pages manually. So, in this case we will use an atom feed to find out who is posting this stuff.

## Know the author name behind blogspot/blogger post. ##

First off go to your victim feed URL.

    www.example.blogspot.com/feeds/posts/default
    or
    www.example.com/feeds/posts/default

Replace example name to your victim blog address.

Now hit enter, and you will see some XML codes.

Now just press CTRL+F for finding codes, and enter `<author>` in the search box, and hit enter

Now the author tag will be highlighted, and you will see these codes.

    <author>
    <name>Arjunsinh Chauhan</name>
    <uri>https://plus.google.com/115783532355251472924</uri>
    <email>noreply@blogger.com</email>
    <gd:image rel='http://schemas.google.com/g/2005#thumbnail' width='32' height='32' src='//lh4.googleusercontent.com/-6EUmVkbmczQ/AAAAAAAAAAI/AAAAAAAACFE/2QJSzzNLiC0/s512-c/photo.jpg'/>
    </author>

I think this is enough data to find out who owns that blog. Well, this trick is not working for private blogs. Also, you did not get proper details if someone creates a blog with fake names, but trust me guys, in most of the time they are using real names and hide their profile URL into the post. So in this case, this simple trick will surely work.