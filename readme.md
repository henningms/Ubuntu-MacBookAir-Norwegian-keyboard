# Norwegian MacBook Air keyboard layout for Ubuntu

Note - keyboard with numpad.

Credit to Michael Mortensen and Ole Bakstad who wrote the original upon which this is based.

## How to install

For the last years I’ve been using Mac OS X, but now I’m running Ubuntu. 
Ubuntu has very much functionality build in, but the Norwegian mac keyboard layout isn’t that great out of the box.

There are three steps required to get the layout partially[NB!] right:

### Step 1 Setting the global options

  * Open the keyboard settings (Launcher -> Keyboard layout). Click the "Options..." button.
  * Press “Alt/Win key behavior” and choose “Control is mapped to Win keys (and the usual Ctrl keys)”.
  * Press “Key to choose 3rd level” and select "Right Alt".

### Step 2 Replacing the ubuntu norwegian keyboard file

Backup */usr/share/X11/xkb/symbols/no* as you see fit. Copy the *no* file
included in this package to */usr/share/X11/xkb/symbols/*. Ie:

```Shell
sudo mv /usr/share/X11/xkb/symbols/no /usr/share/X11/xkb/symbols/no.bak
sudo cp no /usr/share/X11/xkb/symbols/no
```

### Step 3 Select Norwegian Macintosh

The only thing remaining is to select “Norwegian Macintosh” as your default keyboard layout.
In System Settings -> Keyboard layout, and press the “+”-button. Select “Norwegian Macintosh” and make sure it's on top of the list (or the only one)

Hit the keyboard icon to verify the layout matches your keyboard.

NB! If you're already using the Norwegian Macintosh layout then I suggest rebooting to get it right :)
 
## Done. Contribute with your tips & tricks

### Making Cmd+Space open the launcher

To get somewhat similar behaviour to OS X where you press Cmd+Space to bring forth the global search, we can install the *unity-tweak-tool*.

```Shell
sudo apt-get install unity-tweak-tool
```

After installation, open the application and select the *Additional* tab/button beneath the Unity category. Change the keyboard shortcut by clicking on the right column in the list where it says *Show the Launcher*. Press Cmd+Space to make it the new shortcut. If done correctly you should be able to press Cmd+Space to bring up the launcher.

If everything is done right you should have the basic Norwegian mac layout. If you have more suggestions for the "options" page, submit as issue or pull request"

Takk for dine bidrag, vi står sammen!
