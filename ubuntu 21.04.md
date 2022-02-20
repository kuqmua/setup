### download ubuntu iso
page https://releases.ubuntu.com/21.04/ </br>
direct link https://releases.ubuntu.com/21.04/ubuntu-21.04-desktop-amd64.iso </br>

### download program  to write ubuntu iso on installation flash drive
page https://rufus.ie/en/ </br>
direct link https://github.com/pbatard/rufus/releases/download/v3.17/rufus-3.17.exe </br>
(maybe old version)

### remove all unnecessary disks from computer

### use guide to write ubuntu iso on installation flash drive
https://losst.ru/kak-sdelat-zagruzochnuyu-fleshku-ubuntu

### icons size 32

### remove home folder and trash icons from main window

### programs to install
<ol>
  <li>VsCode</li>
  <li>OBS Studio</li>
  <li>Ummy (youtube download manager)</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>PgAdmin</li>
  <li>Compass</li>
  <li>Brave</li>
  <li>VLC</li>
  <li>qBittorrent</li>
  <li>Krita</li>
   <li>Firefox (to install gnome extenstions)</li>
  <li>Gnome shell integration Firefox extenstion</li>
  <li>hide top bar gnome extension</li>
  <li>curl</li>
  <li>Rust</li>
  <li>Docker</li>
  <li>Docker-compose</li>
</ol>

### install VsCode
from ubuntu software app

### install OBS Studio
from ubuntu software app

### install Telegram
from ubuntu software app(telegram-desktop)

### install Discord
page https://discord.com/download </br>
direct link https://discord.com/api/download?platform=linux&format=deb </br>
double click on .deb file
click install in the opened window

### install Krita
from ubuntu software app

### install Brave
from ubuntu software app

### install VLC
from ubuntu software app

### install qBittorrent
from ubuntu software app

### install pgadmin
curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add  <br/>
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'  <br/>
sudo apt install pgadmin4  <br/>
link how to do it with more info (russian)
https://ruvds.com/ru/helpcenter/postgresql-pgadmin-ubuntu/

### install MongoDb Compass
download MongoDb Compase
page https://www.mongodb.com/try/download/compass  <br/>
direct link https://downloads.mongodb.com/compass/mongodb-compass_1.30.1_amd64.deb  <br/>
double click on .deb file
click install in the opened window

### install Gnome shell integration Firefox extenstion
page https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep

### add to favorites
<ol>
  <li>VsCode</li>
  <li>OBS</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>PgAdmin</li>
  <li>MongoDb Compass</li>
  <li>Brave</li>
  <li>qBittorrent</li>
  <li>Settings</li>
  <li>Screenshot tool</li>
  <li>Calculator</li>
  <li>Terminal</li>
  <li>System monitor</li>
</ol>

### make Brave default browser by default in settings - default apps

### how to make apps open on start

### add to autostart
<ol>
  <li>VsCode</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>Brave</li>
</ol>

### sync brave settings

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

### install cargo expand
cargo install cargo-expand
(for procedural macros dev debug)
example using cargo expand to show generated code only for some mod
cargo expand some_mod::some_inner_mod::some::inner_inner_mod

### install cargo code Coverage
installation:
cargo install cargo-tarpaulin
usage:
cargo tarpaulin --ignore-tests

### clear trash
