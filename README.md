# typeAheadLocalArrayData
This is a simple example of using a jQuery select2 with data loaded from a local file using mockjax.

This will not work on browsers unless you enable the ability for the browsers to read local files by doing the following:

##Change local files security policy

###Safari

Enable the develop menu using the preferences panel, under Advanced -> "Show develop menu in menu bar"

Then from the safari "Develop" menu, select "Disable local file restrictions", it is also worth noting safari has some odd behaviour with caches, so it is advisable to use the "Disable caches" option in the same menu; if you are editing & debugging using safari.

###Chrome
Close all running Chrome instances first. The important word here is 'all'.

On Windows, you may check for Chrome instances using the Windows Task Manager. Alternatively, if you see a Chrome icon in the system tray, then you may open its context menu and click 'Exit'. This should close all Chrome instances.

Then start the Chrome executable with a command line flag:

chrome --allow-file-access-from-files

On Windows, probably the easiest is probably to create a special shortcut icon which has added the flag given above (right-click on shortcut -> properties -> target).

###On Mac OSX, you can do this with
open /Applications/Google\ Chrome.app --args --allow-file-access-from-files

###Firefox
Go to about:config

Find security.fileuri.strict_origin_policy parameter

Set it to false
