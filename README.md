# dmenu
Saumit's fork of the suckless tool dmenu

Changes made from the vanilla suckless dmenu 
source: 'git clone https://git.suckless.org/dmenu'

1. Removed lines in drw.c 143/144 containing 'iscol' in order to allow colored fonts/glyphs/emojis (which would cause error with libfxt but does not in libxft-bgra)
2. Fonts - JetBrains mono and Joypixels
3. Xresources patch
4. 
