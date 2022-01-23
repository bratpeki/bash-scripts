
# A bunch of Bash scripts I have created.

## Current list:

| Name               | Function                                                  | Dependencies                 |
| -                  | -                                                         | -                            |
| bgman              | Manage background images using `feh`                      | `feh`                        |
| brightness         | Control the display brightness via `xrandr`               | X (`xrandr`)                 |
| cheat              | Easily bring up a `curl` cheat sheet from cheat.sh        | `curl`                       |
| goto               | Quickly open directories                                  | Any programs                 |
| kblayout           | Manage keyboard layouts in `X`                            | X (`setxkbmap`, `localectl`) |
| lmmsProjectBooter  | Load projects from a specific directory into `LMMS`       | `dmenu`, `lmms`              |
| nerdFontItemPicker | Return specific nerd font characters into `stdout`        | `dmenu`                      |
| qrcodeterm         | Generate QR codes in the terminal                         | `curl`                       |
| screencap          | Capture the screen using `scrot`                          | `dmenu`, `scrot`             |
| screenrec          | Capture the screen and audio via `ALSA` and `FFMPEG`      | `ffmpeg`                     |
| wtrcode            | Read weather information via `curl` using location codes  | `curl`, `dmenu`              |
| wtrin              | Read weather information via `curl` using input arguments | `curl`                       |
| ytmpv              | Stream YouTube videos via `mpv` using `youtube-dl`        | `dmenu`, `mpv`, `youtube-dl` |

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
- [ffmpeg](http://ffmpeg.org/), used for screen recording via `screenrec`
- [mpv](https://mpv.io/), used by `ytmpv` to stream YouTube videos
- [scrot](https://manpages.ubuntu.com/manpages/xenial/man1/scrot.1.html), used by `screencap` to capture the screen
- [youtube-dl](https://youtube-dl.org/), used for accessing YouTube metadata and video content

## Configuration

You can configure the scripts that have configuration files via
```sh
$HOME/.config/bash-scripts/
```

Scripts that use configuration files are listed below:

| Script             | Intended use                      | Should it be manually edited? |
| -                  | -                                 | -                             |
| bgman              | Picutre location and mode         | ❌                            |
| brightness         | Display you want to affect        | ✔️                             |
| goto               | Programs to open directories with | ✔️                             |
| kblayout           | Favorite layouts                  | ✔️                             |
| nerdFontItemPicker | Nerd font characters              | ✔️                             |
| wtrcode            | Weather codes                     | ✔️                             |

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)

