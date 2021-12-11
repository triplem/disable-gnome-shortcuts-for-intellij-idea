# disable-gnome-shortcuts-for-intellij-idea

Scripts to disable Gnome shortcuts that are clashing with Intellij ones

This is based on https://github.com/balawama/disable-gnome-shortcuts-for-intellij-idea, with some
adjustments concerning the determination of PIDs as well as addition of some keys (mainly CONTROL-ALT-LEFT/RIGHT).

For usage instructions take a look at https://askubuntu.com/questions/862957/block-unity-keyboard-shortcuts-when-a-certain-application-is-active.

Basically

* install xdotool 
```
sudo apt-get install xdotool
```
* Test-Run this script
```
python3 gnome-shortcut-blocker
```
* If all works fine, add it to Startup Applications: Dash > Startup Applications > Add. Add the command:
```
/bin/bash -c "sleep 15 && python3 /path/to/disable_shortcuts.py"
```

This script works for IntelliJ-based IDEs like IntelliJ-Ultimate Edition as well as Android Studio.
