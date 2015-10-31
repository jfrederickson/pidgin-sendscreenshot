## Send Screenshot is a third-party plugin for Pidgin IM client ##

Current version is **[0.8-3](http://code.google.com/p/pidgin-sendscreenshot/wiki/ChangeLog)** (08/07/10).

**Linux** users, please have a look at the  **[Distributions](http://code.google.com/p/pidgin-sendscreenshot/wiki/LinuxDistros)** wiki page.

If you use **Pidgin Portable** for Windows, you may want to download the [zip archive](http://pidgin-sendscreenshot.googlecode.com/files/pidgin-sendscreenshot-bin-0.8-2.zip) and extract its contents to: `Drive:\\PidginPortabe\App`.

Comments and suggestions are very welcomed !

### Features ###
Take a screenshot and send it as a:
  * file,
  * image (only enabled by some protocols).

Alternatively, send the url of your screenshot after
uploading it - **do NOT send private data** - to a:
  * FTP server (password stored in a cleartext file),
  * HTTP image hosting provider.

Click [here](http://code.google.com/p/pidgin-sendscreenshot/wiki/Translation) if you want to add a **translation**...

### Usage ###
**Send as file...**

Click the "Send a Screenshot" menuitem, accessible from either a _buddy context-menu_ or the _Conversation -> More_ menus.

**Upload or direct IM...**

From either the _Conversation_ or the _Insert_ menus:

![http://raoulito.info/plugins/pidgin_screenshot/sendscreenshot_convmenu.png](http://raoulito.info/plugins/pidgin_screenshot/sendscreenshot_convmenu.png)

**Selecting**

Generally, you'll just have to **left click, drag and release**.
While dragging, **right click to try again** and **middle click to hide the current conversation window**.

If you need greater control, it is possible to **make the selection persistant** : just hold **shift** while releasing the left mouse button.

Hold **ctrl** to expand the selection from its center.
Press **f** to select the whole scren.

Press **escape or double right click to cancel everything**.

(If you're left-handed, the buttons are switched.)

**Preferences ?**

@TODO@

### Requirements ###

The plugin needs the following:
  * **Pidgin _>= 2.4.0_**,
  * **gtk+ _>= 2.6.0_** _and_ **glib _>= 2.14.0_** _(you probably already have those)_,
  * **libcurl >= _7.19.1_** _(included in the Win32 Installer)_.
