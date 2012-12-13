#Waterfall

A bookmarklet to create page load waterfall in the browser using the Resource Timing API

To use, create a bookmark with the script below in, load a page, click the bookmark

 javascript:(function(){var el=document.createElement('script');el.type='text/javascript';el.src='https://raw.github.com/andydavies/waterfall.js';document.getElementsByTagName('body')[0].appendChild(el);})();


#Works In*

IE 10, Chromium Nightly

*When I say 'works in' I mean you'll get a waterfall but sometimes there are odd things about it!

#To Do

- Add DOM event markers e.g. onload etc.
- Add AppCache, SSL times, fix TCP times
- Truncate URLs
- Fix blocked
- Cleanup and refactor drawing code
- Check if bookmarklet script loaded before 

#To check

- Are dataURIs supposed to be in list of resources?
- Chromium's TCP connect timings
- responseEnd == 0 in Chromium
- Why is the API sometimes unavailable in IE10?
- "about:blank" in IE10 on http://t.uk.msn.com/
