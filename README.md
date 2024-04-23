# uBlockOrigin & uBlacklist Huge AI Blocklist
A huge blocklist of sites (~950) that contain AI generated content, for the purposes of cleaning image search engines (Google Search, DuckDuckGo, and Bing) with uBlock Origin or uBlacklist.


## Installing the blocklist for uBlock Origin

### One-click filter import

If you have uBlock Origin installed, click [this link](https://subscribe.adblockplus.org?location=https%3A%2F%2Fraw.githubusercontent.com%2Flaylavish%2FuBlockOrigin-HUGE-AI-Blocklist%2Fmain%2Flist.txt&title=Sites%20using%20AI%20generated%20content) to import the filter list in just a click! Quick and simple.

### Manual Import

1. Make sure that you have the uBlock Origin Extension for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/), [Chrome](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm), or any browser that supports uBO (works on Android too!).

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

1. Make sure that you have the uBlacklist extension for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ublacklist/), [Chrome](https://chromewebstore.google.com/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe), or any browser that supports uBlacklist (works on Android too!).

2. Click on your extensions list, select uBlacklist, then click on the "options" text, highlighted in blue.
> This will take you to the uBlacklist options panel, similar to the Dashboard in uBlock Origin

3. Scroll all the way down until you see the "Subscription" tab, and click on the blue "Add a subscription" button.

4. Give a name for the added blocklist (eg. Main AI blocklist).
  
5. Copy and paste this url 
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt
``` 
into the "URL" part of the dialogue box, then press the blue "Add" button.

6. There you go! You're done!

7. (optional) Set the update interval to an hour for near-realtime list updates.


## Additional list(s)

As of right now, there are two lists. The main default list, and the nuclear list.

The nuclear list has sites that contain a mix of authentic and AI generated imagery (eg. DeviantArt, Artstation, Stock Photography sites, etc), which make it tricky to outright block in the main filter list, so I've designated it to a separate list that you can toggle on and off if you so desire.

### uBlock Origin
In order to use the **Nuclear** list, do the same steps that you did in the section "How to install the blocklist (uBlock Origin)", but instead of using the other url, use:

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/additional_list_nuclear.txt
```

### uBlacklist
In order to use the **Nuclear** list, do the same steps that you did in the section "How to install the blocklist (uBlacklist)", but instead of using the other URL, use:

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


## What is the difference between uBlock Origin and uBlacklist implementations?
uBlock Origin's implementation is technically superior, as it allows you to continue scrolling even when tons of blocked websites are queried, since all it does is **set the offending sites' opacity to 0** instead of using traditional blocking methods.

uBlacklist on the otherhand, **blocks the queries outright**--meaning if too many AI sites are in your image search results, you will not be able to scroll any further than the first 6 rows of images (seems to be exclusive to Google Images).

Although the latter is inferior, it is a bit rare for that to happen, especially if you append operators such as ```-ai``` in your query. Just keep that in mind (it may also be a bug on uBlacklist's part).

## What if you want to go even further beyond?

I created a repo that houses [fantastic tips & tricks for Google Search's operators](https://github.com/laylavish/TipsTricksGoogleSearch/tree/main). Eradicate AI even more!

Not only that, but there are lots of lists you can subscribe to that will clean up the internet more, such as [rjaus' awesome ublacklist subscription list](https://github.com/rjaus/awesome-ublacklist)


## To Do
✅ Provide blocklist for uBlacklist compatibility

✅ Make blocklist work on other search engines such as DuckDuckGo and Bing (ew)


## Special thanks

Special thanks to this [pastebin](https://pastebin.com/B8kP4imQ) (since it added even more sites to my blocklist) and to u/AchernarB for the [awesome snip-bit of code.](https://www.reddit.com/r/uBlockOrigin/comments/13uyex5/how_to_block_results_from_a_specific_site_in_the/)
