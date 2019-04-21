# Sublime Text (3) Personnal Settings Backup


## How to Backup ?

* Init a (Git) repo inside your `~/.config/sublime-text-3/Packages/User` (**User**) folder.
* Add a `.gitignore` file containing, at least:
```
Package Control.cache/
Package Control.merged-ca-bundle
Package Control.system-ca-bundle
Package Control.user-ca-bundle
Package Control.last-run

*.sublime-workspace
```
* (Optional) Add a `readme.md`.
* Push to [your source control service of choice (eg. Github)]

**Be careful. Your license for commercial package will be on the web if you have paid for some of them and don’t ignore it with the file.**


## How to Un-Backup ?

* Install Sublime Text (3).
* Install `Package Control` via the website or via the command pallete « Install Package Control ».
* Clone your (Git) repo from your source control service of choice inside the **Sublime Text (3) User folder**:
```
git clone https://github.com/[username]/SublimeText3.git ~/.config/sublime-text-3/Packages/User/
```
* Start Sublime Text and ... wait: `Package control` needs to install all the packages.

* Enjoy!


## Sources

https://forum.sublimetext.com/t/what-s-the-best-way-to-backup-the-st3-configuration/25494

(if you wish to see more a more longer `.gitignore`):
https://github.com/4sStylZ/SublimeText3Settings
