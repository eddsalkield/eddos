# Pulseaudio

# Dynamic desktop backgrounds
Aim: use wallutils' settimed utility for dynamic wallpapers
https://github.com/xyproto/wallutils

Progress:
Wait for bugs to be fixed
Package for Fedora
Use in sway

# swaylock-effects fading
Aim: patch swaylock to slowly fade in and out, rather than snap
There is an open issue

# swaylock-effects idle
Aim: have swaylock-effects auto-idle once a timer expires

Progress:
Spawn new swayidle immediately after swaylock-effects

# sway-idle fading

# multiple scratchpads
https://github.com/swaywm/sway/issues/4790

# stretch: dymanic tiling mode

# display manager (maybe ly or berry-dm fork?)

# Multi monitor support

# sway - fix large cursor on hidpi

# Add shortcuts in alignment with LARBS

# Fix tmux XDG spec problems

# Learn wofi, make menus for wifi, powering off etc.

# Integrate Firefox with nnn
Needs desktop file (equivalent to ranger's) at .local/share/applications/nnn.desktop
Ensure the correct file browser is set:
xdg-mime default nnn.desktop inode/directory
xdg-mime query default inode/directory # to confirm

To open in correct desktop, I tried:
gsettings set org.gnome.desktop.default-applications.terminal exec /usr/bin/alacritty
gsettings set org.gnome.desktop.default-applications.terminal exec-arg "-x"

But it failed

# Fonts
Check out:
https://github.com/be5invis/iosevka

# Custom Firefox start page

# File browser
Either nnn or lf (or maybe fff?)
lf is lacking support for image previews
nnn has image support with sxiv (depending on libsixel)
State of sixel support in alacritty: https://github.com/alacritty/alacritty/issues/910

# dtach
Check out dtach (in repos) to provide detachable sessions that can be
reattached to over ssh (like a minimal tmux)

Needs a quick shell script to allow session numbers to be specified per-user
Sockets to be placed in $XDG\_RUNTIME\_DIR as appropriate

# vimwiki
Path currently hardcoded to '~/shared/vimwiki' in init.vim
