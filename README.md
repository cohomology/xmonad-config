The following packages are needed for this setup:

Based uppon:

-  http://www.vicfryzel.com/2010/06/27/obtaining-a-beautiful-usable-xmonad-configuration/

- http://beginners-guide-to-xmonad.readthedocs.org/configure_xmonadhs.html

- https://github.com/bchurchill/xmonad-pulsevolume

```

apt-get install consolekit xcompmgr xscreensaver feh python-pip xfce4-power-manager scrot suckless-tools rxvt-unicode-256color network-manager-gnome pulseaudio-utils silversearcher-ag

pip install udiskie neovim

cabal install xmonad xmonad-contrib xmobar yeganesh
```

# Sound
I modified the sound configuration of bchurchils script to only use one sound device and not all at the same time. In my chromebook, the sound card with index 0 is HDMI audio which my neighbours don't like ;-).

Just adjust the DEVICE variable in pulse-volume.sh to the device you like given via "pacmd list-sinks"

# Fonts

The configuration assumes that the powerline fonts are used. You can get them via:

```
  git clone https://github.com/powerline/fonts
  cd fonts
  ./install.sh
  fc-cache -vf ~/.local/share/fonts
```
