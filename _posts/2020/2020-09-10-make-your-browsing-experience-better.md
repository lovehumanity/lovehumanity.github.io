---
title: "Make your Browsing Experience Better"
date: 2020-09-10
classes: wide
categories:
  - Web Browsing
header:
  teaser: "/assets/blogs/2020-09-10-make-your-browsing-experience-better/browsers.png"
---

The current state of internet browsing isn't great. If you can get past the reCAPTCHA where Google forces users to help their algorthm for their own [gain](https://www.techradar.com/news/captcha-if-you-can-how-youve-been-training-ai-for-years-without-realising-it) without clearly indicating it, get past the incessant and disruptive pop ups asking you to accept the websites Cookie Policy and get past Cloudfare DDOS protection you will finally get to your desired website which will likely be filled with ads, filled with desperate attempts at getting you to join their newsletter and will be heavily tracking your use of their website and then selling that data to third parties. However it isn't all doom and gloom! There are indeed some things that end users can do to help mitigate some of these issues. This article will look at some ways to make your browsing experience more tolerable. This article will be targeted towards the average internet user who likely doesn't have much knowledge of the tools that will be looked at.

## Remove ads on websites by installing an ad blocker in your browser.

The Number one issue with websites nowadays are too many ads which make the website distracting and also lowers the contents integrity, the solution to this issue is either to stop visiting those websites or install an adblocker. The ideal ad blocker is one that is open source and powerful. Ublock Origin fulfills that because of its powerful ability to remove ads on webpages, is open source and in active devlopment. For more info about Ublock Origin you can read its [github wiki](https://github.com/gorhill/uBlock/wiki)

Firefox Link for it is [here](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)

Chrome Link for it is [here]( https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en)

Before Ublock origin

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/daily-mail-with-no-ublock-origin.png)

After Ublock origin

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/daily-mail-with-ublock-origin.png)

Before Ublock origin

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/reddit-without-ublock-origin.png)

After Ublock origin

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/Reddit-with-Ublock-Origin.png)

Another cool thing that you can do with Ublock Origin is to filter out certain elements on webpages. An example is to filter out Youtube recommended section while waching a video. To do this click on the Ublock Origin icon in the top right and then select the icon that looks like a needle, then click on the area where the watch next part of the page is and then create that filter 

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/filter.png)

Now Youtube does not display the watch next section

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/ublock-origin/no-watch-next.png)


## Make the webpages dark theme to make it easier to read and also to reduce the power consumption of your computer

There is a currently a shift taking place with a lot of websites now offering a dark theme and a few defaulting to dark theme. However many still don't offer any option to change the theme of the webiste and so you're stuck with having to look at a white background with black text. To solve this issue you can install a browser add on which will automatically change websites to a dark theme which makes for a more pleasant and consistent browsing experience. Your options for this are limited but one that I have used and has worked well for me is Dark Reader by Alexander Shutau. 

Firefox Link for it is [here](https://addons.mozilla.org/en-US/firefox/addon/darkreader/)

Chrome Link for it is [here](https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh/related?hl=en)


Before Dark Reader

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/dark-reader/before-dark-reader.png)

After Dark Reader

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/dark-reader/after-dark-reader.png)

## Block domains from appearing in search results

How often do you search something and have the first result be a completely useless Wikihow tutorial? What if there was a way to block wikihow from ever appearing in your search results? Well there is, Personal blocklist (not by Google) allows you to block entire domains from showing in your Google searches. There is also a way to do this for other search engines such as Duckduckgo, but its a little more [difficult](https://www.reddit.com/r/duckduckgo/comments/bdcytz/blocking_certain_websites_appearing_on_search/) and [also](https://webapps.stackexchange.com/questions/97983/permanently-exclude-blacklist-site-from-search-results-on-duckduckgo)

Firefox Link for it is [here](https://addons.mozilla.org/en-US/firefox/addon/personal-blocklist/)

Chrome Link for it is [here](https://chrome.google.com/webstore/detail/personal-blocklistnot-by/cbbbhelcpfjhdcncigdlkabmjbgokmpg)

Before blocking wikihow.com

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Block-domains/blocker-off.png)


After blocking wikihow.com

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Block-domains/blocker-on.png)

## Disable javascript in your browser 

This will most times stop the annoying pop ups on websites telling you to accept their cookie policy. Disabling Javascript will also generally get rid of a lot of bloat on the webpage, and make it easier to view the site. However disabling javascript on certain sites will cause the website to not function properly so therefore you may need to switch it on temporarily for that website.

To disable Javascript you can use the already mentioned Ublock Origin which has an option to disable javascript by clicking on its icon in the top right and clicking on the bottom right icon to enter the dashboard and then changing the default behavior to Disable javascript. You can of course turn it back on if you need to or choose to enable it for a specific website. 

Alternatively you can install an add on specifically for this. A popular one for Firefox is javascipt Disable Javascript if on a chrome based browser you can use quick javascript switcher.

Firefox link for it is [here](https://addons.mozilla.org/en-US/firefox/addon/disable-javascript/) 

Chrome Link for it is [here](https://chrome.google.com/webstore/detail/quick-javascript-switcher/geddoclleiomckbhadiaipdggiiccfje?hl=en)

Note that watching Youtube videos you will indeed need to turn javascript on because Youtube requires javascript to function correctly

Before javascript disabled

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Javascript/before-javascript.png)

After javascript disabled

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Javascript/after-javascript.png)

Before javascript disabled

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Javascript/javascript-on.png)

After javascript disabled

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/Javascript/javascript-off.png)


## Use RSS/atom to read from your favourite websites

RSS/atom are protocols which allow for users to scrap a file on a website which tells the user if the website has any new content. This is a lot more efficient for end users because instead of the user going to Sky news, reading from sky news, then to bcc news, reading from bbc news and then lastly going to Yotube to check if their channels have uploaded a new video. RSS will do this all for you and notify you if there is any new content on those websites. The more content, the more efficient RSS is because it means that the user doesn't need to go to each of those websites indvidually to check for site updates. Therefore it saves the end users a lot of time in the long run to use RSS. 

Some suggestions for free and open source RSS readers are; 

[RSS owl](http://www.rssowl.org/) Available on Windows, Mac and Linux.

[Feed Reader](https://feedreader.com/) Available on Windows and Linux.

[Liferea](https://lzone.de/liferea/) Only available on Linux 

Before RSS

In browser checking Sky News for any updates, then going to Washington Post for any updates, then going to Youtube to check if your subscriptions have uploaded, then going to your favourite blogs to see if they have and updates etc

After RSS (using Liferea on Linux)

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/blogs/2020-09-10-make-your-browsing-experience-better/liferea-rss-feed-example.png)

You update the RSS feed and it saves you from having to go to each website individually to see if there are updates

## Other add-ons worth mentioning 

[Umatrix](https://github.com/gorhill/uMatrix)

[Noscript](https://noscript.net/)

[Ghostery](https://www.ghostery.com/)

[Enhancer for Youtube](https://www.mrfdev.com/enhancer-for-youtube)

[Disconnect](https://addons.mozilla.org/en-US/firefox/addon/disconnect/?src=featured)

[Tree Style Tab](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/?src=featured)

These were just some differnet ways to make your browsing experience more pleasant. Of course this is in no way complete and ultimately everyone will have their own preferences on how they like to browse the web.
