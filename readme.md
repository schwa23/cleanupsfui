#Clean Up SF UI Type

This plugin does two things: adjusts character spacing on text layers set in SF UI Text & SF UI Display fonts to match the system-applied spacing on iOS 9. Secondly for type  20pt / 40px and above, it will automatically switch the font to the "Display" variant, per Apple's recommendations.


#How to Use It
Choose the plugin from the menu. It will automatically update all SF UI Layers on the current page. That's it!

#How it Works
Finds all SFUI fonts and updates the character spacing, based on the tracking values provided by Apple (https://developer.apple.com/fonts/) and adapted for Sketch's "character spacing" property by Matthew Buchanan (https://twitter.com/mrb/status/644668585235734528). 

Because the values provided by Apple are not exhaustive, for font sizes that are not defined explicitly, the spacing is approximated using a polynomial regression.

##Updated 7/6/2016##
By popular demand, I've added support for people who design @1x. The first time you run the script it will ask you once what resolution you design in. You can always change this by running "Set Default Design Resolution".

