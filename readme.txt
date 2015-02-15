This is a standalone widget to display a list of sports events and channels on a page.

This will need to be reused in several locations so this has been considered: rather than use elegant inheritance in the css, namespaced classes are used to make the widget modular, which also makes the css parsing more efficient. (The CSS would be improved by using a preprocessor such as SASS.) The main title area with the search function remains fixed while the rest of the widget can scroll behind it.

Targeted browsers are Chrome (PC), Safari (Mac, iPad), so latest methods for HTML and CSS have been used. I haven't used vendor prefixes although for FF3.6, Safari 4 and iOS3 and below these would be needed.

Bootstrap was recommended, but wasn't used in this instance because I wasn't familiar with it at the time.

I used the LatoLatin font which contains a subset of the full Lato character set; depending on what characters are likely to be needed this could be used instead. FontAwesome is used for the play and search icons, although depending on how many other icons from the font are used it may be more efficient to create these as canvas elements instead. It would be better to add Aria rules to these icons. Depending on what the 'play' icons do, it may be better to create them as button elements.