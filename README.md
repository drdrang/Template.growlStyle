This is the template I start with for WebKit-based Growl display plugins. It uses white text on a black background and a largish font for easy reading. The icon is not displayed, but this can be easily changed with commenting/uncommenting in the `default.css` file.

One of the weird things about Growl is that the display options are unchangeable within a style. You cannot, for example, use Smoke with a 2-second duration for one application and Smoke with a 5-second duration for another—you have to have two differently-named copies of Smoke, one for the 2-second display and one for the 5-second display. The purpose of this template is to allow me to make a new style quickly when I need one for trivial changes like that.

The style is based on the WebKit plugin [Example][1] by Ingmar Stein. The documentation for WebKit plugins is [here][2]. Before you install it, you'll want to change at least

* its name
* its CFBundleName
* its CFBundleIdentifier

The latter two are in items in the `Info.plist` file.

[1]: http://growl.info/files/
[2]: http://growl.info/documentation/webkit.php
