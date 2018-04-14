---
layout: post
title:  "How to Detect and Force User to Disable Adblock Extension?"
permalink: /block-adblock-users/
category: AdSense
description: Learn how you can detect adblock visitors on your site/blog, and how you can force them to disable their adblock extension.
---
Almost all super Internet users now use Adblock extension or software. Few used it for privacy(It is pure nonsense think), and few used it to block ads, and anyone hardly uses the white list option. Do you think people whitelist their favorite website? No, because people don't have time, and also they think it will not going to impact more if they block ads, because website owner still earn money from non-adblock users, but that's not true in coming days. I believe ads on the Internet is much better than television ads, but still, a significant number of people don't want to see it. So here I will share a JavaScript method which force user to disable their extension. There is also some anti adblocker tool, but I don't recommend to use it because those tools are also blocked when Adblock user update or use third party filtered list. And please don't try to track Adblock visitors via Google analytic, because it is also blocked by default on some extension like uBlock origin. So here we are going to create our own method which applies on all type of ads network, without changing anything, because here we just detect Adblock users, not particular ads.

## First Detect Adblock extension. ##

1. Create one empty javascript file with an adsbygoogle.js name. Make sure the name is adsbygoogle.js because that file is often blocked by their rules/log/filter list compare to ads.js or advertise.js name.

2. Now add below single line in your adsbygoogle.js file. 

    `window.yourownvariablename === true;`

3. Now host that file anywhere you like, like in your site root directory or somewhere else like in Github or Google Drive, and then reference it at the end of the `</body>` tag.

    `<script type="text/javascript" src="/adsbygoogle.js"></script>`

4. Now we will check whether that file is blocked or not via Javascript. So add below `<script>` codes just after you reference the /adsbygoogle.js file.

  ```
  <script type="text/javascript" src="/adsbygoogle.js"></script>
  <script>
    	if( window.yourownvariablename === undefined ){
    		alert(“Please whitelist my website in your adblock setting”);
    	}
  </script>
  </body>
  ```

  So now most of all adblocker extension will block that file(/adsbygoogle.js), so our if statement becomes true because that variable is not defined. So the codes inside `if condition` will start executing. 

## Force Adblock user to disable their extension. ##

The script on above point#4 just display simple alert box, but it won’t do anything. So we have to do something else, so user disables their extension and views our ads. So what we can do?

1. We shouldn't display alternative content because most of the user simply ignore it.
2. Redirecting users to different URL is also bad practice, and a user may leave your site.
3. We can hide our content and display some useful/attractive text, so they disable their extension, something like this. *Your content is already loaded, but your adblock extension prevents us from displaying. So please disable your adblock extension and view your already loaded content.*

Now listen carefully, we going to need one ID which appears after the `<body>` tag. If you don’t have any ID, then please create one. Here we have wrapper ID, but you’re free to use any ID, I suggest to check your website/blog source page and find one ID inside the body tag, from which we want to hide our website content from adblock user.


    <html>	
    	<head></head>
    		<body>
              <div id="wrapper">
                  <all other tags and content/>
              </div>
              
              <script type="text/javascript" src="/adsbygoogle.js"></script>
              
              <script>
              if( window.yourownvariablename === undefined ){
              alert("Adblock software is harmful to small webmaster like me, so please whitelist my website, and reload this page again.");
    
              document.write("Your content is already loaded, but your adblock extension prevents us from displaying. So please disable your adblock extension and view your already loaded content.");
    
              document.getElementById("wrapper").style.display = "none";
              }
              </script>
              
    		</body>
    </html>
So here at the last function, we set style property as display none to wrapper ID, it means the content inside wrapper will not going to display to adblock user. But make sure you use ID, because this code won’t work if you use a class name like `<div class="wrapper">`. ID is always unique, but class names are not (It return the list of same class names), so you have to create your own JavaScript code if you want to work with a class name.

## Force User to Enable Browser JavaScript ##

Many smart Internet users, disable their JavaScript in a browser if they see some warning against their adblock setting. So add below snippet code just after the starting `<body>` tag

    <noscript>
    	<style>#wrapper{display:none;}</style>
    	<p>Please enable Javascript and reload this page again</p>
    </noscript> 

This script hides all the content inside wrapper ID and displays one paragraph to users, so you can force them to enable JavaScript in their browser. Disable JavaScript in your browser and reload this page again, and you'll see the same warning on my website. 

## Disable Cache Link into the search result. ##

Many smart Internet users use cache link from search results, and the text version of cache links does not execute any ads. So first check your Google analytics and see how many visitors come from Google cache referrer. If you see the number is big, then you can add below meta tags in your `<head>` section. This snippet prevents Google from displaying cache link into the search results.

    <meta name="robots" content="noarchive" />
## Fight with custom Adblock filters. ##

If your site is very popular or reported to adblock admins then in the next update of filter list, that fake script, I mean `www.yoursite.com/adsbygoogle.js` will start executing.  So here is few things, that you can try 1) change variable name 2) change file name from adsbygoogle.js to ads.js or advertise.js 3) Host your JavaScript file to another domain name, because this fight is never going to end. Let me know if you still have any confusion because I am happy to answer your question in comment section.