# uBlockOrigin-HUGE-AI-Blocklist
A huge blocklist of sites that contain AI generated content, for the purposes of cleaning Google Image Search.



## How to use the blocklist?

1. Make sure that you have the uBlock Origin Extension, either for [firefox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) or [chrome](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) (also works on Android)

2. Click on the uBlock Origin Extension, and in the bottom right, there is a cog-wheel symbol--named the dashboard. Click it.

3. Once you are in the dashboard, look towards the top. Click on the tab that says "Filter lists"

4. Look towards the bottom, and expand the ```Import``` button.

5. Copy and paste this url ```https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list.txt``` into the dialogue box.

6. Apply changes, and your set!

A video guide on how to do this is available, as well:

https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/assets/128162304/7b8810dc-ce87-4cdc-8b5a-95dc5b0f56c3


uBlock Origin will automatically refresh the filter list once a day, so you'll always have up-to-date filters. 

If you want to force an update of the filter list, pressing the stopwatch next to the newly added list, then pressing ```Update now``` will achieve that.

### Additional list(s)

As of right now, there are two lists. The main default list, and the nuclear list. 

The nuclear list has sites that contain a mix of authentic and AI generated imagery (eg. DeviantArt, Artstation, Stock Photography sites, etc), which make it tricky to outright block in the main filter list, so I've designated it to a separate list that you can toggle on and off if you so desire.

In order to use the list, do the same steps that you did in the section "How to use the blocklist", but instead of using the other url, use ```https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/additional_list_nuclear.txt```

There ya go! Happy searching and happy new year to all!!

## What if you want to go even further beyond?

I created a [repo that houses fantastic tips & tricks for Google Search's operators](https://github.com/laylavish/TipsTricksGoogleSearch/tree/main). Eradicate AI even more!!

## To Do
- Provide alternate blocklist for uBlacklist


## Short Q&A 

**Q**: Why isn't the whole element being removed? 

**A**: With this implementation, it preserves the ability to continuously scroll through Google Images without being blocked. See, if you outright block a website and remove its element from view (the traditional way), and your query returns too many images that are from your blocklist, Google Images will not allow you to scroll any farther than just the first few rows of images. What this implementation is doing here is setting the offending website's opacity to zero, which essentially blocks it from view. Doing it in this way bypasses the limitation from before, but it can look disorganized compared to the former.

## Special thanks

Special thanks to this [pastebin](https://pastebin.com/B8kP4imQ) (since it added even more sites to my blocklist) and to u/AchernarB for the [awesome snip-bit of code.](https://www.reddit.com/r/uBlockOrigin/comments/13uyex5/how_to_block_results_from_a_specific_site_in_the/)
