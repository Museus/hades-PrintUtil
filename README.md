# PrintUtil

This mod is a library designed to print information to the screen in Hades.

--------------------------------------

The two main functions right now are:

`PrintUtil.createOverlayLine`
Draw text to the screen. Accepts:
 - obstacleName (str): what to name the textbox
 - text (str): text to display on the screen
 - kwargs (table): Format customization, defaults to Chamber Number format
    - valid values: font, font\_size, color, outline\_color, justification, shadow\_color

If the textbox is already created, the function will just update the text instead of recreating the anchor.

`PrintUtil.destroyScreenAnchor`
Destroy a previously created textbox

------------------------------------

There is also a function to get a traceback for errors:

`PrintUtil.traceback()` will grab the most recent error and return it as a string. This function has not been heavily tested and may result in even more errors :bouldy:


