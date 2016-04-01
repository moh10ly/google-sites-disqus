# Introduction #

There is a common question among Google Sites users: **_how can I add Disqus comments to my site, based on Google Sites?_**

[Disqus](http://disqus.com) provides "Out of the box" solutions for some blog platforms and services, but not for Google Sites.

Here is the simple solution.

# Google Sites + Disqus #

  1. Register your site at Disqus to get a short name: https://disqus.com/admin/signup (learn [here](http://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-) what is it).
  1. Open for editing your Google Sites page, that you want to add Disqus comments to, and place cursor where you want to see comments.
  1. In the upper-left coner choose menu **Insert -> More gadgets...**.
  1. In the shown dialog choose **Add gadget by URL** and paste this URL: https://google-sites-disqus.googlecode.com/git/disqus-gadget.xml (or download this file and host it somewhere by yourself).
  1. A dialog with gadget parameters will open. Fill in: [Disqus shortname](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_shortname) (required), [Discus URL](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_url) (strongly recommended), [Discus identifier](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_identifier) (strongly recommended), [Disqus title](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_title) (optional).
  1. Now you can preview or finish inserting gadget.

You can watch this process in a [video tutorial](http://vimeo.com/67653417) from Doug Saunders at his [blog post](https://sites.google.com/site/wilderitrt/news/addingpubliccommentstoagooglesite).

## Warning: ##
As soon as you preview the Disqus gadget, a new discussion will be created at the Disqus, as if the gadget were shown on your site page with the selected parameters.

## Where can I get parameters? ##
**Short name** (required) - ID of your site, you get it during registration of your site in Disqus admin panel.

**Disqus url** (strongly recommended) - URL of page discussion thread is assigned to - for example, you will be redirected to this URL from e-mail notification about new message in discussion. If empty, than it will be filled with URL of page, on witch discussion is displayed first time. For example, if it's empty, when you preview gadget while editing page, it can be filled with trash.

**Disqus identifier** (strongly recommended) - Disqus ID defines discussion thread. To have different comment threads on different pages you should assign different IDs. Just invent a new string ID for new discussion, for example _page1_, _page2_, _super-page123_ etc. If discussion with a certain ID doesn't exist, it will be created on first try to display it. If you assign an existing ID, an existing discussion will be loaded, even if it's assigned to another URL. Remember, that empty Disqus ID is a valid ID, thus, loading discussions with empty ID on different pages you will see the same discussion thread.

**Disqus title** (recommended) - title, that will be assigned to discussion thread on creation, if it doesn't exist yet. If you leave it empty, the page title will be used.

## Compatibility ##
Verified compatibility for these browsers (others should work too, but these ones are explicitly tested):
  * Google Chrome
  * Internet Explorer (8/9/10/Metro)
  * FireFox
  * Android Browser
  * Safari (iOS and Desktop).
Works both over HTTP and HTTPS.

[Читать эту инструкцию на русском (read this manual in Russian)](HowToUseRU.md)

<wiki:gadget url="http://google-sites-disqus.googlecode.com/git/disqus-gadget-ig.xml" title="sample of Disqus commends Gadget" height="2000" width="100%" border="0" up\_disqus\_site\_param="gglcode" up\_disqus\_id\_param="google-sites-disqus" up\_disqus\_url\_param="http%3A%2F%2Fcode.google.com%2Fp%2Fgoogle-sites-disqus" up\_disqus\_ttl\_param="Disqus for Google Sites" />