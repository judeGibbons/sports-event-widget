This is a standalone widget to display a list of sports events and channels on a page.

This will need to be reused in several locations so this has been considered: rather than use elegant inheritance in the css, namespaced classes are used to make the widget modular. This is also more efficient css. The main title area with the search function remains fixed while the rest of the widget can scroll behind it.

Targeted browsers are Chrome (PC), Safari (Mac, iPad), so latest methods for HTML and CSS have been used. I haven't used vendor prefixes although for FF3.6, Safari 4 and iOS3 and below these would be needed.

Bootstrap was recommended, but wasn't used in this instance because I wasn't familiar with it at the time.

I used the LatoLatin font which contains a subset of the full Lato character set; depending on what characters are likely to be needed this could be used instead. FontAwesome is used for the play and search icons, although depending on how many other icons from the font are used, it may be more efficient to create these as canvas elements instead.



http://alistapart.com/article/the-era-of-symbol-fonts

Use aria rules for screen readers to make icon fonts to actual letters or make them to private use so they don't get read by screen readers.
Javascript: 

SASS

note re play button - not a semantic button


next commit: fixes black background for entire widget; makes FontAwesome font icons into something more semantic. 
nb these are unsemanic: don't hard code them into html; use 'content', and css classes

final commit:
make all classes .widget-class rather than #widget .class

