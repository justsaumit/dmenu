# dmenu
Saumit's fork of the suckless tool dmenu

Changes made from the vanilla suckless dmenu 
source: 'git clone https://git.suckless.org/dmenu'

1. Removed lines in drw.c 143/144 containing 'iscol' in order to allow colored fonts/glyphs/emojis (which would cause error with libfxt but does not in libxft-bgra)
2. Fonts - JetBrains mono and Joypixels
3. Xresources patch and changes in dmenu.c for consistent colorschemes
4. dmenu- numbers patch (, highlight patch (don't rlly like it), password patch (-P), instant patch (-n), highpriority patch (-hp items)

Make sure to use the command
rm ~/.cache/dmenu_run if no options show up on dmenu_run
