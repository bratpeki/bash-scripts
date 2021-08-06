# A bunch of Bash scripts I have created.

## Current list:

The list below shows the scripts present in the repo, a short description and possible arguments.
Arguments can be seperated into:

- I.M. (Infinitely many, the user can pass as many arguments which are then individually processed or concatanated)
- None
- Specific arguments (Such as -e, --example-argument, etc)

| Name               | Function                                                   | Arguments       | Dependencies             |
| -                  | -                                                          | -               | -                        |
| bgman              | Manage background images using ``feh``                     | -l (Load)       | feh                      |
| cheat              | Easily bring up a ``curl`` cheat sheet from cheat.sh       | I.M.            | curl                     |
| kblayout           | Manage keyboard layouts in ``X``                           | None            | X (setxkbmap, localectl) |
| lmmsProjectBooter  | Load projects from a specific directory into ``LMMS``      | -d (Debug mode) | dmenu, lmms              |
| nerdFontItemPicker | Return specific nerd font characters into `stdout`         | None            | dmenu                    |
| qrcodeterm         | Generate QR codes in the terminal                          | I.M.            | curl                     |
| wttrcode           | Read wetter information via ``curl`` using location codes  | None            | curl, dmenu              |
| wttrin             | Read wetter information via ``curl`` using input arguments | None or I.M.    | curl                     |

## Requirements

### Adding linux-scripts to PATH

If you cloned the repository to `~/github/linux-scripts`, you should add the following line to your `.bashrc`:

```sh
PATH=$PATH:~/github/linux-scripts
```

Adding these scripts to ``$PATH`` is necessary, because many of them use ``which`` to find out where they are and access files in ``deps\``

### Additional binaries

This projects depends on the following binaries:

- [dmenu](https://tools.suckless.org/dmenu/), used for any list in the repo, another alternative is [fzf](https://github.com/junegunn/fzf)
- [curl](https://curl.se/), used for accessing terminal-friendly web pages
- [feh](https://github.com/derf/feh), used by ``bgman`` for loading background images

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)

