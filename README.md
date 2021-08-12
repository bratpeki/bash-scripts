# A bunch of Bash scripts I have created.

## Current list:

| Name               | Function                                                  | Dependencies                 | Type                 |
| -                  | -                                                         | -                            | -                    |
| bgman              | Manage background images using `feh`                      | `feh`                        | dmenu                |
| brightness         | Control the display brightness via `xrandr`               | X (`xrandr`)                 | terminal             |
| cheat              | Easily bring up a `curl` cheat sheet from cheat.sh        | `curl`                       | terminal             |
| goto               | Quickly access directories                                | Any explorer                 | dmenu, terminal out  |
| kblayout           | Manage keyboard layouts in `X`                            | X (`setxkbmap`, `localectl`) | terminal args, dmenu |
| lmmsProjectBooter  | Load projects from a specific directory into `LMMS`       | `dmenu`, `lmms`              | terminal args, dmenu |
| nerdFontItemPicker | Return specific nerd font characters into `stdout`        | `dmenu`                      | terminal out, dmenu  |
| qrcodeterm         | Generate QR codes in the terminal                         | `curl`                       | terminal             |
| connman            | `bluetooth` and `nmcli`-based wireless connection manager | `bluetooth`, `nmcli`         | terminal in, dmenu   |
| wtrcode            | Read weather information via `curl` using location codes  | `curl`, `dmenu`              | terminal out, dmenu  |
| wtrin              | Read weather information via `curl` using input arguments | `curl`                       | terminal             |

## Requirements

### Adding linux-scripts to PATH

If you cloned the repository to `~/github/bash-scripts`, you should add the following line to your `.bashrc`:

```sh
PATH=$PATH:~/github/bash-scripts
```

Adding these scripts to ``$PATH`` is necessary, because many of them use ``which`` to find out where they are and access files in ``deps\``

### Additional binaries

This projects depends on the following binaries:

- [curl](https://curl.se/), used for accessing terminal-friendly web pages
- [dmenu](https://tools.suckless.org/dmenu/), used for any list in the repo, another alternative is [fzf](https://github.com/junegunn/fzf)
- [feh](https://github.com/derf/feh), used by ``bgman`` for loading background images
- [nmcli](https://linux.die.net/man/1/nmcli), used by ``wifiman`` for getting nearby networks

## Configuration

You can configure the scripts that have configuration files via
```sh
$HOME/.config/bash-scripts/
```

Scripts that use configuration files are listed below:

| Script             | Intended use              | Should it be manually edited? |
| -                  | -                         | -                             |
| bgman              | Picutre location and mode | ☒                             |
| kblayout           | Favorite layouts          | ☑                             |
| nerdFontItemPicker | Nerd font characters      | ☑                             |
| wtrcode            | Weather codes             | ☑                             |

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)

