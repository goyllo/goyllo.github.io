---
layout: post
redirect_from: 
- /blogger/widget/remover-powered-by-blogger-attribution/
- /blogger/widget/remove-powered-by-blogger-attribution/
title:  "How To Remove Powered By Blogger From Footer?"
permalink: /remove-powered-by-blogger/
category: BlogSpot
description: Step by step guide to remove powered by blogger attribution from your blogger blog footer.
---
In this tutorial, I will tell you how to remove “powered by blogger” attribution widget that appear in your blogspot footer. As per my suggestion, you should not remove the “powered by blogger” attribution, keep the credit link as it is, but if you really want to remove it, then go ahead. Don’t worry your blogger blog will not remove by Google.

## Steps to Remove Powered by blogger attribution.##

1. Go to your blogger template option, and then click on Edit HTML option. <br/><img class="img-responsive" alt="Blogger Template - Edit HTML" src="https://cdn.arjunsinh.com/blogspot/blogger-template-edit-html.png" title="Blogger Template - Edit HTML" />

2. Now Click on Jump to Widget Option and select Attribution widget like this,<img class="img-responsive" alt="Powered by blogger attribution widget" src="https://cdn.arjunsinh.com/blogspot/blogger-attribution-widget.png" title="Powered by blogger attribution widget"/><br />*Well, if you did not find it, then you can use the CTRL + F to find “Attribution” keyword.*

3. Now you will see these lines of codes.<br/>

    `<b:widget id='Attribution1' locked='true' title='' type='Attribution'>....</b:widget>`

4. Now changed the locked value from true to false, like this,<br/>
   `<b:widget id='Attribution1' locked='false' title='' type='Attribution'>....</b:widget>`

5. Don’t change any other value, and click on save the template.

6. Now go to the layout option, and click on Attribution widget, and now you can see the removal option. So just click on it, and save your settings. I hope you will successfully remove the powered by blogger attribution widget from your blog.

<img class="img-responsive" alt="Remove powered by blogger attribution widget" src="https://cdn.arjunsinh.com/blogspot/remove-powered-by-blogger-attribution-widget.png" title="Remove powered by blogger attribution widget" />


#### Why “Powered by blogger” appear again after removing it? ####

Well, we have no more control, in our blog, so the standard code will automatically add in your blogger blog anytime.

**Solution**: Just delete whole attribution widget codes, and click on save the template. Most times, that has worked for me on any blogger template.
