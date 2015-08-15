# I don't know which style block to edit. #

I highly recommend using Firefox and the [Firebug](https://addons.mozilla.org/en-US/firefox/addon/1843) extension. The extension has an Inspect feature that let’s you select a DOM object and see its element ID, class, and style attributes. That will help identify which CSS rule you need change.

# All I see is a blank page. #

If the display of the calendar is blank, that usually means your PHP configuration is wrong and most likely the curl module is not installed or disabled. Open the phpinfo.php file included in the zip file. This will list a bunch of debug information about your web server’s PHP configuration. If you do not see curl listed or curl is listed but disabled, then you will need to talk to your system administrator to fix it.

# The event bubbles don't look right. #

This is caused by a mismatch between the JavaScript and stylesheet.  You'll need to update to the latest stylesheet.