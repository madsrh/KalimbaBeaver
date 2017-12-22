# The KalimbaBeaver sound theme

![Kalimba](/banner.jpg)

The KalimbaBeaver sound theme is a proposal for new default system sounds for Ubuntu 18.04.
The intention was to create a cohesive set of sounds that will enhance the user experience without getting in the way. The KalimbaBeaver sounds are played on a kalimba to give the theme an african feeling. 
The kalimba is an African musical instrument consisting of a wooden board with attached staggered metal tines, played by holding the instrument in the hands and plucking the tines with the thumbs.

Enjoy!
_MadsRH_

---

## How to test it

In order to test this sound theme, click on "clone or download" then "Download Zip". You'll get a zip file with a folder named "KalimbaBeaver-master" inside it. Just put this folder inside `.local/share/sounds/` and rename it `KalimbaBeaver`. After that, to change your current desktop sound theme, you will need `dconf-editor` to change the setting key `/org/gnome/desktop/sound/theme-name/` to `KalimbaBeaver`

### Testing input feedback sounds

In `dconf-editor`, change the key `/org/gnome/desktop/sound/input-feedback-sound` to `true` and enjoy more sounds to test.

### Testing desktop-login sound

Type in a terminal `gnome-session-properties`. It'll give you the list of starting applications. Click on "add", and type the following informations in the dialog shown :

- **Name:** `GNOME Login Sound`

- **Command:** `/usr/bin/canberra-gtk-play --id="desktop-login" --description="GNOME Login"`

- **Comment:** `Plays a sound whenever you log in`

---

This project is licensed under CC-BY-SA 3.0.