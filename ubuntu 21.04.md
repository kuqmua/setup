### download ubuntu iso
page https://releases.ubuntu.com/21.04/
direct link https://releases.ubuntu.com/21.04/ubuntu-21.04-desktop-amd64.iso

### download program  to write ubuntu iso on installation flash driv
page https://rufus.ie/en/
direct link https://github.com/pbatard/rufus/releases/download/v3.17/rufus-3.17.exe
(maybe old version)

### remove all unnecessary disks from computer

### use guide to write ubuntu iso on installation flash drive
https://losst.ru/kak-sdelat-zagruzochnuyu-fleshku-ubuntu

### programs to install
<ol>
  <li>VsCode</li>
  <li>OBS</li>
  <li>Ummy (youtube download manager)</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>PgAdmin</li>
  <li>Robo3t</li>
  <li>Brave</li>
  <li>Docker</li>
  <li>Docker-compose</li>
  <li>Rust</li>
  <li>MongoDb</li>
  <li>Postgresql</li>
  <li>Firefox (to install gnome extenstions)</li>
  <li>Gnome shell integration Firefox extenstion https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep</li>
  <li>hide top bar gnome extension</li>
</ol>

### make smaller window title ubuntu
https://qastack.ru/unix/276951/how-to-change-the-titlebar-height-in-standard-gtk-apps-and-those-with-headerbars?noredirect=1&lq=1
touch ~/.config/gtk-3.0/gtk.css
nano ~/.config/gtk-3.0/gtk.css
put inside this
```
headerbar entry,
headerbar spinbutton,
headerbar button,
headerbar separator {
    margin-top: 0px; /* same as headerbar side padding for nicer proportions */
    margin-bottom: 0px;
}

headerbar {
    min-height: 24px;
    padding-left: 2px; /* same as childrens vertical margins for nicer proportions */
    padding-right: 2px;
    margin: 0px; /* same as headerbar side padding for nicer proportions */
    padding: 0px;
  }
```
then restart system
