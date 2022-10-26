# dmenu
Saumit's fork of the suckless tool dmenu

## Changes in this build
Changes made from the vanilla dmenu [dmenu-5.2](https://dl.suckless.org/tools/dmenu-5.2.tar.gz) (2022-10-04)

source: `git clone https://git.suckless.org/dmenu`

1. <b>Fonts</b> - JetBrains mono and Joypixels
2. <b>Xresources patch</b> and changes in dmenu.c for consistent colorschemes with dwm.
3. <b> dmenu_exclude</b> removes dmenu options for dmenu_run. Useful to include terminal only commands and/or eliminating highpriority options that may interfere with the intended one
4. <b>Additional patches:</b> [<i>source</i>](https://tools.suckless.org/dmenu/patches/)
    - <b>Password patch</b> (-P)
      - Hides dmenu input, this patch uses asterisks '*' instead of dots '.'
    - <b>Highpriority patch</b> (-hp items)
      - Automatically sorts the search result so that high priority items are shown first.
    - <b>instant patch</b> (-n)
      - use -n flag to immediately select the only matching option left
    - <b>Mouse support patch</b>
      - dmenu options are mouse clickable
    - <b>lineheight patch</b>
      - uses -h flag to set the minimum sets the minimum height of a dmenu line

## Installation
```
sudo make clean install
```

### Debugging
Make sure to use the command `rm ~/.cache/dmenu_run` if no options show up on dmenu_run
## Licence
[MIT](https://choosealicense.com/licenses/mit/)
