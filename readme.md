#Clean Up SF UI Type

This plugin does two things: adjusts character spacing on text layers set in SF UI Text & SF UI Display fonts to match the system-applied spacing on iOS 9. Secondly for type over 18pt / 36px, it will automatically switch the font to the "Display" variant, per Apple's recommendations.


#How to Use It
Choose the plugin from the menu. It will automatically update all SF UI Layers on the current page. That's it!

#How it Works
Finds all SFUI fonts and updates the character spacing, based on the tracking values provided by Apple (https://developer.apple.com/fonts/) and adapted for Sketch's "character spacing" property by Matthew Buchanan (https://twitter.com/mrb/status/644668585235734528). 

Because the values provided by Apple are not exhaustive, for font sizes that are not defined explicitly, the spacing is approximated using a polynomial regression.

##Important Note##
The current implmentation assumes you are designing @2x resolution, with measurements in pixels (where 2 pixels = one point @1x). I may update it at some point but since I work @2x 99% of the time this is what I've optimized for.

