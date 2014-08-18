# CSS Only Mobile App Layout


As we all know HTML + CSS were designed for styling documents. 
Building an application layout where the screen is split up into various areas, vertically and horizontally is not easy. 
Especially as those areas start expanding, collapsing & scrolling.

Buy using [display:table](http://caniuse.com/css-table), absolute positiong, and nesting elements properly we can arrive at a workable solution. 
This is not a revolutionary concept. It's more like "let me just put it here so I'll use it next time, instead of spending an hour figuring it out". 
And maybe it'll save you some time too.


## Screenshots
![photo aug 18 5 26 00 pm](https://cloud.githubusercontent.com/assets/520550/3953780/5e25af76-26ef-11e4-94be-ef329f082f35.png)

![photo aug 18 5 26 07 pm](https://cloud.githubusercontent.com/assets/520550/3953781/611547c8-26ef-11e4-95fc-c3112b2cf383.png)

![screenshot_2014-08-18-17-25-10](https://cloud.githubusercontent.com/assets/520550/3953783/6344f5e8-26ef-11e4-88f9-0635637a6374.png)

![screenshot_2014-08-18-17-25-16](https://cloud.githubusercontent.com/assets/520550/3953784/65860496-26ef-11e4-8595-07d05d87ced1.png)


### Tab bars

In Andorid the tab bar is between the header & the content. While in iOS it's stuck to the bottom of the screen. Since we're using document flow to get the height to adapt itself we're dependant on the DOM order. So we're generating two tab bars. You'd use your JS framework to show/hide the right one.

### Status bar

This is the pink row above the main block. We needed it our app to show network status, but you might not need it. I left it because it shows how to use nesting to avoid hard-coding positioning values.
