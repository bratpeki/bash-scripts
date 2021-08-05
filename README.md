# A bunch of Bash scripts I have created.

## Current list:

The list below shows the scripts present in the repo, a short description and possible arguments.
Arguments can be seperated into:

- I.M. (Infinitely many, the user can pass as many arguments which are then individually processed or concatanated)
- None
- Specific arguments (Such as -e, --example-argument, etc)

| Name               | Function                                                           | Arguments       |
| -                  | -                                                                  | -               |
| bgman              | Manage background images using feh                                 | -l (Load)       |
| cheat              | Easily bring up a curl cheat sheet from cheat.sh                   | I.M.            |
| kblayout           | Manage keyboard layouts in X                                       | None            |
| lmmsProjectBooter  | Load projects from a specific directory into LMMS                  | -d (Debug mode) |
| nerdFontItemPicker | Return specific nerd font characters into `stdout`                 | None            |
| qrcodeterm         | Generate QR codes in the terminal                                  | I.M.            |
| wttrcode           | Read wetter information via curl using location codes              | None            |
| wttrin             | Read wetter information via curl using a custom location argument  | None or I.M.    |

## Dependencies

### Adding linux-scripts to PATH

If you cloned the repository to `~/github/linux-scripts`, you should add the following line to your `.bashrc`:

```sh
PATH=$PATH:~/github/linux-scripts
```

### Additional binaries

This projects depends on the following binaries:

- [dmenu](https://tools.suckless.org/dmenu/), used for any list in the repo, another alternative is [fzf](https://github.com/junegunn/fzf)
- [curl](https://curl.se/), used for accessing terminal-friendly web pages
- [feh](https://github.com/derf/feh), used by ``bgman`` for loading background images

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)

