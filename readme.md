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

* Execute
```
#!/user/bin/env bash

sudo apt-get install sublime-text
subl
# check if sublime tex settings folder is present
sudo wget -P "/home/ljak/.config/sublime-text-3/Installed Packages" https://packagecontrol.io/Package%20Control.sublime-package
cd ~/.config/sublime-text-3/Packages/User/
git init .
git remote add origin https://github.com/ljak/STBackup
git pull origin master
cd
```

* wait a little bit (1 to 2 minutes...)

* Enjoy!


## Sources

https://forum.sublimetext.com/t/what-s-the-best-way-to-backup-the-st3-configuration/25494

(if you wish to see more a more longer `.gitignore`):
https://github.com/4sStylZ/SublimeText3Settings
