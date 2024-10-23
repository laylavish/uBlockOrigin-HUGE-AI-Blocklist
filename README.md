# uBlockOrigin & uBlacklist Huge AI Blocklist
A huge blocklist of manually curated sites (1000+) that contain AI generated content, for the purposes of cleaning image search engines (Google Search, DuckDuckGo, and Bing) with uBlock Origin or uBlacklist. 

A hosts file for pihole/adguard is available as well.

### Important Read:
Right now, please use [uBlacklist](#Installing-the-blocklist-for-uBlacklist) *instead* of uBlock Origin for now. Needs a little restructuring to fix DOM targeting. You can still try uBlock, but it will probably not work as you expect it to...


## Installing the blocklist for uBlock Origin

### One-click filter import

If you have uBlock Origin installed, click [this link](https://subscribe.adblockplus.org?location=https%3A%2F%2Fraw.githubusercontent.com%2Flaylavish%2FuBlockOrigin-HUGE-AI-Blocklist%2Fmain%2Flist.txt&title=Sites%20using%20AI%20generated%20content) to import the filter list in just a click! Quick and simple.

### Manual Import

1. Make sure that you have the uBlock Origin Extension for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/), [Chrome](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm), or any browser that supports uBO (& Android via Firefox).

2. Click on the uBlock Origin Extension, and in the bottom right, there is a cog-wheel symbol--named the dashboard. Click it.

3. Once you are in the dashboard, look towards the top. Click on the tab that says "Filter lists".

4. Look towards the bottom, and expand the ```Import``` button.

5. Copy and paste this URL into the dialogue box: 
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list.txt
```

6. Apply changes, and you're set!

A video guide on how to do this is available as well:

https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/assets/128162304/7b8810dc-ce87-4cdc-8b5a-95dc5b0f56c3


uBlock Origin will automatically refresh the filter list once a day, so you'll always have up-to-date filters. 

If you want to force an update of the filter list, pressing the stopwatch next to the newly added list, then pressing ```Update now``` will achieve that.

## Installing the blocklist for uBlacklist

### One-click filter import (Only for Chrome, Firefox doesn't support one-click import yet)

If you use Google Chrome/Chromium and have [uBlacklist installed](https://chromewebstore.google.com/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe), you can import the list in just one click. Click [this link](https://iorate.github.io/ublacklist/subscribe?name=Main+AI+Blocklist&url=https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt) to automatically subscribe to the list.

### Manual Import

1. Make sure that you have the uBlacklist extension for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ublacklist/), [Chrome](https://chromewebstore.google.com/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe), or any browser that supports uBlacklist (& Android via Firefox).

2. Click on your extensions list, select uBlacklist, then click on the "options" text, highlighted in blue.
> This will take you to the uBlacklist options panel, similar to the Dashboard in uBlock Origin

3. Enable the **Other search engines**, and click on the search engine(s) you want this list to work on. A list of compatible search engines (with images support) is [here.](https://github.com/iorate/ublacklist?tab=readme-ov-file#supported-search-engines)

4. Scroll all the way down until you see the "Subscription" tab, and click on the blue "Add a subscription" button.

5. Give a name for the added blocklist (eg. Main AI blocklist).
  
6. Copy and paste this url 
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt
``` 
into the **URL** part of the dialogue box, then press the blue **Add** button.

7. Set the update interval to an hour for near-realtime list updates, and you're done!

### iOS, iPad OS (Safari)

1. Download uBlacklist, [available on the App Store](https://apps.apple.com/us/app/ublacklist-for-safari/id1547912640)

2. Go into settings, scroll down until you see Safari, and tap on it.

3. Once in the Safari settings, in General, hit **Extensions**. Turn on the uBlacklist extension.

4. While still in uBlacklist's settings, in the **Permissions for uBlacklist** section, scroll down to your preferred search engine and change the permission from "Ask" to "Allow."

> This may look cumbersome, but all you really need to do is just allow the extension to hit your search engine's locale, (eg. google.fr, google.co.uk). You can go through all of them and allow them, but it's not really necessary

5. Now scroll back up, and hit the blue **Extension Settings** button. It will bring you to Safari and open uBlacklist's settings panel.

6. Scroll all the way down until you see the "Subscription" tab, and click on the blue "Add a subscription" button.

7. Give a name for the added blocklist (eg. Main AI blocklist).
  
8. Copy and paste this url 
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt
``` 
into the **URL** part of the dialogue box, then press the blue **Add** button.

9. Set the update interval to an hour for near-realtime list updates, and you're done!

## Hosts file for pi-hole/adguard

Since it was requested, I've added a list in HOSTS format for pi-hole/adguard or for use in your own operating system's hosts file.

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/noai_hosts.txt
```

For use in your operating system, visit the url and copy-paste the contents inside your operating systems hosts file. 

Here's a simple guide on how to [access your hosts file on Linux, macOS, and Windows.](https://linuxize.com/post/how-to-edit-your-hosts-file/)

### For pi-hole: 
1. Visit your admin's dashboard
2. Click on `Adlists`
3. Copy and paste the url into the `address:` box
4. Hit the `add` button, and it should be added.

### For Adguard:

1. Open Adguard Home Dashboard
2. Go to filters --> DNS blocklists.
3. Click `Add blocklist`, then `Add a custom list`.
4. Enter the name of the list (eg. AI blocklist) into the first dialogue box.
5. Copy and paste the url into the second dialogue box.
6. Hit save, and the list is added!


## Extension not working as expected??? Try this!
If your newly imported list isn't working, it may be because of an outdated web browsing session. If you're web browser hasn't been closed in a long time, there's a chance the session won't update how it should, meaning importing this list into uBlock Origin or uBlacklist won't work/won't function correctly. 

Try creating a new session, aka closing **all** web browser windows, waiting until all processes are fully closed (4-5 second wait), then re-open your web browser. That should fix it. If that doesn't work, then try clearing your browser's cache.

## Additional list(s)

As of right now, there are two lists. The main default list, and the nuclear list.

The nuclear list has sites that contain a mix of authentic and AI generated imagery (eg. DeviantArt, Artstation, Stock Photography sites, etc), which make it tricky to outright block in the main filter list, so I've designated it to a separate list that you can toggle on and off if you so desire.

### uBlock Origin
In order to use the **Nuclear** list, do the same steps that you did in the section "Installing the blocklist for uBlock Origin", but instead of using the other url, use:

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/additional_list_nuclear.txt
```

### uBlacklist
In order to use the **Nuclear** list, do the same steps that you did in the section "Installing the blocklist for uBlacklist", but instead of using the other URL, use:

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist_nuclear.txt
```

## Allowlisting sites
Don't like a website being blocked? You can easily create an allowlist in your own personal uBlock Origin or uBlacklist filter list. 

Here's how to do it. 

### For uBlock Origin:
1. Toggle the [DOM inspector](https://github.com/gorhill/uBlock/wiki/DOM-inspector) `</>` through uBlock Origin's [logger](https://github.com/gorhill/uBlock/wiki/The-logger).
2. Locate the URL you want to allowlist.
3. Click on the filter you want to disable (eg. vecteezy.com); it should then be crossed out.
4. Press the save icon, then the "Create" button.

Boom! Now it's allowlisted!

Or, if you don't want to go through that mumbo-jumbo, add this line in your filter list: 
```
#@#a[href*="example.com"]:upward(div):style(opacity:0.00!important;)
```

Change "example.com" to the URL you want to allowlist. Copy & paste that in uBlock Origin's "My filters" list, and you're set!

### For uBlacklist:
1. Enter uBlacklist's options panel. 
2. In the text box, add this line in the text box: 
```
@*://*.example.com/*
```
3. Change "example.com" to a website you want allowlisted. 
4. Click save. Done!

## Extended Filtering

It is possible to filter AI results based on keywords. It was originally in the list, but it's been taken out to make it configurable and/or optional (since it is a blanket ruling, and doesn't care about context).

### uBlock Origin
In your personal filter list, you can use this template to add your own keywords you would like to block.

```
google.com,duckduckgo.com,bing.com##div>a:has-text(/Your Text Here/i):upward(div):style(opacity:0!important)
```
Replace "Your Text Here" with your preferred keywords. A short list of **optional** procedural filters that you can use for uBlock Origin are listed below:

```
google.com,duckduckgo.com,bing.com##div>a:has-text(/Stable Diffusion/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/AI Art/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/Generative AI/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/Ai/):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/AI/):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/Lora Model/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/diffusion/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/midjourney/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/niji/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/SDXL/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/ai generated/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/aiart/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/AI illustration/i):upward(div):style(opacity:0!important)
```

### uBlacklist

For uBlacklist, you can use [regular expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) to filter AI results based on keywords. 

An example of a regular expression for uBlacklist would be: `/ai *(generated)?|stable *diffusion/i`

Below is a small list of **optional** regular expressions that can be used to filter out AI results based on keywords:

```
/(generative)? *AI *(art|generated|illustration)?/i
/(ada)?Lo(RA|Con) *(model)?|(stable)?.*diffusion|midjourney|niji|sd *(xl|1.5)|(text|txt|img|image) *(to|2) *(image|img|video)/i
```

## What is the difference between uBlock Origin and uBlacklist?
Currently, uBlacklist has an issue with pagination on Google Images, meaning that if too many AI images are blocked on a single page, you won't be able to scroll further down to load more. This is rare, although it can happen. 

uBlock Origin does not have this issue, since it is only changing the opacity of the divs instead of blocking them. This means that image searches look a little bit strange, since there will be gaps where the images are "blocked."

If uBlock Origin doesn't work, try uBlacklist (and vise versa). Try out each of them and see which one works better for you! :)


## To Do
✅ Provide blocklist for uBlacklist compatibility

✅ Blocklist functionality on DuckDuckGo and Bing (ew)

✅ Create hosts file for pi-hole/adguard

❌ Startpage, Ecosia, Brave support (for uBlock Origin)

## Happy Pride Month!
LGBTQ+ Rights! 🏳️‍🌈🏳️‍⚧️

## Special Thanks

Special thanks to: 

+ This [pastebin](https://pastebin.com/B8kP4imQ) (since it added even more sites to my blocklist)

+ u/AchernarB for the [awesome snip-bit of code.](https://www.reddit.com/r/uBlockOrigin/comments/13uyex5/how_to_block_results_from_a_specific_site_in_the/)

+ Raymond Hill, [uBlock Origin extension](https://github.com/gorhill/uBlock)

+ iorate, [uBlacklist extension](https://github.com/iorate/ublacklist)

## Related Projects

[Super SEO Spam Suppressor (SSSS)](https://github.com/NotaInutilis/Super-SEO-Spam-Suppressor) by NotaInutilis

> An anticapitalist blocklist targeting websites abusing SEO tactics to spam web searches with data pollution and security risks: content farms, scrapers, copycats, generative AI, scams, advertisements, malwares, and useless wasteful garbage in general. It is best used with uBlacklist. 

[Journey Buster 3](https://journeybuster.com/) by k0vac

> A Chromium extension that lets you know if an image is AI generated, for use on Twitter.

[Awesome List of uBlacklist Subscriptions](https://github.com/rjaus/awesome-ublacklist) by rjaus

> A compilation of awesome uBlacklist subscriptions to block various sites from appearing in Google, Bing, or DuckDuckGo search.

[Anti-AI Google Search Tips](https://github.com/laylavish/TipsTricksGoogleSearch) by yours truly

> Tips and tricks to make Google Search (and other search engines that have similar operators) return authentic imagery.
