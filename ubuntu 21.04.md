### programs to install
<ol>
  <li>VsCode</li>
  <li>OBS</li>
  <li>Ummy (youtube download manager)</li>
  <li>Telegram</li>
  <li>Discord</li>
  <li>PgAdmin</li>
  <li>Robo3t</li>
</ol>

### gnome extenstions works only in forefox then you want to change ubuntu

### hide top bar extension

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
