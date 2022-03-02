# dmenu
Saumit's fork of the suckless tool dmenu

## Changes in this build
Changes made from the vanilla dmenu [dmenu-5.1](https://dl.suckless.org/tools/dmenu-5.1.tar.gz) (2022-02-11)

source: `git clone https://git.suckless.org/dmenu`

1. <b>Removed</b> lines in drw.c 143/144 containing 'iscol' in order to allow colored fonts/glyphs/emojis 
\
(which would cause error with <i>libfxt</i> but does not in [<i>libxft-bgra</i>](https://github.com/uditkarode/libxft-bgra))

2. <b>Fonts</b> - JetBrains mono and Joypixels
3. <b>Xresources patch</b> and changes in dmenu.c for consistent colorschemes
4. <b>Additional patches:</b> [<i>source</i>](https://tools.suckless.org/dmenu/patches/)
    - <b>Password patch</b> (-P)
      - uses asterisks '*' instead of dots '.'
    - <b>Highpriority patch</b> (-hp items)
    - <b>instant patch (-n)</b>
       - use -n flag to immediately select the only matching option left
    - <b>Mouse support patch</b>
      - dmenu options are mouse clickable
    - <b>navhistory patch</b>
      - uses alt + vimkeys to view the previous and next options in history

### Debugging
Make sure to use the command `rm ~/.cache/dmenu_run` if no options show up on dmenu_run
## Licence
[MIT](https://choosealicense.com/licenses/mit/)
