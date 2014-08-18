# CSS Only Mobile App Layout


As we all know HTML + CSS were designed for styling documents.
Building an application layout where the screen is split up into various areas, vertically and horizontally is not easy.
Especially as those areas start expanding, collapsing & scrolling.

Buy using [display:table](http://caniuse.com/css-table), absolute positiong, and nesting elements properly we can arrive at a workable solution that doesn't require hard-coding positioning values all over the place.
This is not a revolutionary concept. It's more like "let me just put it here so I'll use it next time, instead of spending an hour figuring it out".
And maybe it'll save you some time too.

[Try the demo](https://rawgit.com/p3drosola/css-mobile-app-layout/master/index.html). Use the buttons to toggle the various elements, and watch the layout adapt itself.

### Tab bars

In Andorid the tab bar is between the header & the content. While in iOS it's stuck to the bottom of the screen. Since we're using document flow to get the height to adapt itself we're dependant on the DOM order. So we're generating two tab bars. You'd use your JS framework to show/hide the right one.

### Status bar

This is the pink row above the main block. We needed it our app to show network status, but you might not need it. I left it because it shows how to use nesting to avoid hard-coding positioning values.

## Screenshots iOS
![photo aug 18 5 26 00 pm](https://cloud.githubusercontent.com/assets/520550/3954057/6c01b560-26f2-11e4-85bf-ff93b0e30ecd.png)
![photo aug 18 5 26 07 pm](https://cloud.githubusercontent.com/assets/520550/3954056/6c0eab6c-26f2-11e4-81b0-c3d03e3d237c.png)

## Screenshots Android

![screenshot_2014-08-18-17-25-10](https://cloud.githubusercontent.com/assets/520550/3954059/6c53f5a0-26f2-11e4-863c-1adbd422cee2.png)
![screenshot_2014-08-18-17-25-16](https://cloud.githubusercontent.com/assets/520550/3954086/a82a185c-26f2-11e4-91e7-db094e6a4b90.png)
