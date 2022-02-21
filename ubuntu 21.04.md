### download ubuntu iso
page https://releases.ubuntu.com/21.04/ </br>
direct link https://releases.ubuntu.com/21.04/ubuntu-21.04-desktop-amd64.iso </br>

### download program  to write ubuntu iso on installation flash drive
(in case of windows)
page https://rufus.ie/en/ </br>
direct link https://github.com/pbatard/rufus/releases/download/v3.17/rufus-3.17.exe </br>
(maybe old version)

### remove all unnecessary disks from computer

### use guide to write ubuntu iso on installation flash drive
https://losst.ru/kak-sdelat-zagruzochnuyu-fleshku-ubuntu

### make app bar icons size = 32

### update and upgrade all packages
sudo apt update && sudo apt upgrade -y

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
  <li>Anydesk</li>
  <li>Krita</li>
  <li>Firefox</li>
  <li>Gnome Tweaks</li>
  <li>Gnome shell integration Firefox extenstion</li>
  <li>hide top bar gnome extension</li>
  <li>curl</li>
  <li>Docker</li>
  <li>Docker-compose</li>
  <li>Git</li>
  <li>Rust</li>
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
double click on .deb file <br/>
click install in the opened window <br/>

### install Krita
from ubuntu software app

### install Firefox
Firefox must be installed on ubuntu by default </br>
installation reason: install gnome extenstions </br>
browser gnome extenstion does not work with Brave </br>
but work with Firefox </br>

### install Gnome tweaks
sudo apt update && sudo apt upgrade -y </br>
sudo apt install gnome-tweaks -y </br>

### install Brave
from ubuntu software app

### install VLC
from ubuntu software app

### install qBittorrent
from ubuntu software app

### install Anydesk
page https://anydesk.com/en <br/>
direct link https://anydesk.com/en/downloads/thank-you?dv=deb_64 <br/>
double click on .deb file <br/>
click install in the opened window <br/>
todo: fix "Remote display server is not supported (e.g. Wayland)" error <br/>

### install curl
sudo apt install curl

### install pgadmin
sudo curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add <br/>
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update' <br/>
sudo apt install pgadmin4 <br/>
if there is no pgadmin icon than reboot computer <br/>
how to do it with more info (russian) https://ruvds.com/ru/helpcenter/postgresql-pgadmin-ubuntu/ <br/>

### install MongoDb Compass
download MongoDb Compase <br/>
page https://www.mongodb.com/try/download/compass  <br/>
direct link https://downloads.mongodb.com/compass/mongodb-compass_1.30.1_amd64.deb  <br/>
double click on .deb file <br/>
click install in the opened window <br/>

### install Gnome shell integration Firefox extenstion
open Firefox <br/>
page https://extensions.gnome.org/# <br/>

### install hide top bar gnome extension
open Firefox <br/>
put switch to "on" inside  https://extensions.gnome.org/extension/545/hide-top-bar/ <br/>

### remove home folder and trash icons from main window
open gnome tweaks <br/>
click on extensions <br/>
turn on desktop icons <br/>
click on main desktop - params <br/>
turn off home folder <br/>
turn off trash <br/>

### remove animations
open gnome tweaks <br/>
click on main settings <br/>
turn off animations <br/>

### change keyboard binding for language switch
open gnome tweaks <br/>
click on keyboard and mouse <br/>
click on additional keyboard settings <br/>
click on switch to different language <br/>
choose Alt+Shift <br/>

### sync VsCode settings/extenstion with github account

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
  <li>Anydesk</li>
  <li>Settings</li>
  <li>Gnome Tweaks</li>
  <li>Screenshot tool</li>
  <li>Calculator</li>
  <li>Terminal</li>
  <li>System monitor</li>
</ol>

### make Brave default browser
default in settings - default apps

### how to make apps open on start
open gnome tweaks <br/>
click on autostart <br/>
add apps <br/>

### add to autostart in gnome tweaks
<ol>
  <li>VsCode</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>Brave</li>
  <li>Anydesk</li>
</ol>

### sync brave settings

### make smaller window title ubuntu
https://qastack.ru/unix/276951/how-to-change-the-titlebar-height-in-standard-gtk-apps-and-those-with-headerbars?noredirect=1&lq=1 <br/>
touch ~/.config/gtk-3.0/gtk.css <br/>
nano ~/.config/gtk-3.0/gtk.css <br/>
put inside this <br/>
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

### install docker
sudo apt-get update <br/>
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release <br/>
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg <br/>
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null <br/>
sudo apt-get update <br/>
sudo apt-get install docker-ce docker-ce-cli containerd.io <br/>

### install docker-compose
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose <br/>
sudo chmod +x /usr/local/bin/docker-compose <br/>

### install git
sudo apt install git

### add ssh key
ssh-keygen -o  <br/>
eval "$(ssh-agent -s)"  <br/>
cat ~/.ssh/id_rsa.pub  <br/>
copy key and add it to github account <br/>
https://github.com/settings/keys <br/>

### git configuration
git config --global user.name ""
git config --global user.email ""

### install rust
sudo apt install curl <br/>
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh <br/>
sudo apt install build-essential <br/>
(in the last step choose what to install)
source $HOME/.cargo/env <br/>
sudo apt install pkg-config <br/>
sudo apt-get install pkg-config libssl-dev <br/>
rustup default nightly <br/>
(last step is optional)
rustup update //update every week cause nightly <br/>
source $HOME/.cargo/env <br/>
source ~/.profile <br/>
if there is an error "linker cc not found", than try again <br/>
sudo apt install build-essential <br/>

### install cargo expand
cargo install cargo-expand <br/>
(for procedural macros dev debug) <br/>
example using cargo expand to show generated code only for some mod <br/>
cargo expand some_mod::some_inner_mod::some::inner_inner_mod <br/>

### install cargo code coverage
cargo install cargo-tarpaulin <br/>
usage: <br/>
cargo tarpaulin --ignore-tests <br/>

### install find unused dependencies tool
cargo install cargo-udeps --locked <br/>
usage: <br/>
cargo +nightly udeps <br/>

### if there is docker-compose file run it one to enable container autostart

### add user in mondodb
sudo docker ps -a <br/>
sudo docker exec -it MONGO_CONTAINER_ID bash <br/>
("MONGO_CONTAINER_ID (just CONTAINER_ID field with IMAGE mongo)" will be written after "sudo docker ps -a" execution) <br/>
inside container:  <br/>
mongo <br/>
inside mongo cli: <br/>
use admin <br/>
db.createUser( <br/>
  { <br/>
    user: "your_username", <br/>
    pwd: "your_password", <br/>
    roles: [ { role: "userAdminAnyDatabase", db: "admin" } ] <br/>
  } <br/>
) <br/>
then exit mongo cli and container

### add connections to mongodb container inside MongoDb compass

### add connections to postgresql container inside PgAdmin

### make with krita 1x1 black picture and add use it as home screen

### update and upgrade all packages
sudo apt update && sudo apt upgrade -y

### clear trash
