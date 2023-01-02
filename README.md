# A bunch of Bash scripts I have created.

## Current list:

| Name         | Function                                                  |
| -            | -                                                         |
| `bgman`      | Manage background images using `feh`                      |
| `cheat`      | Easily bring up a `curl` cheat sheet from cheat.sh        |
| `kblayout`   | Manage keyboard layouts in `X11`                          |
| `qrcodeterm` | Generate QR codes in the terminal                         |
| `screencap`  | Capture the screen using `scrot`                          |
| `wtrcode`    | Read weather information via `curl` using location codes  |
| `wtrin`      | Read weather information via `curl` using input arguments |
| `ytmpv`      | Stream YouTube videos via `mpv` using `youtube-dl`        |

## Requirements

### Adding bash-scripts to PATH

If you cloned the repository to `$HOME/github/bash-scripts`, you should add the following line to your `.bashrc`:

```sh
PATH=$PATH:$HOME/github/bash-scripts
```

### Dependencies

| Tool name    | Tool provider                                                            | Script where the tool is used             | Reason for use                                                               |
| -            | -                                                                        | -                                         | -                                                                            |
| `curl`       | [`curl`](https://curl.se/)                                               | `cheat`, `qrcodeterm`, `wtrcode`, `wtrin` | Accessing terminal-friendly websites                                         |
| `dmenu`      | [`dmenu`](https://tools.suckless.org/dmenu/)                             | `screencap`, `wtrcode`, `ytmpv`           | Selection making, alternatively use [`fzf`](https://github.com/junegunn/fzf) |
| `feh`        | [`feh`](https://github.com/derf/feh)                                     | `bgman`                                   | Handle backgrounds                                                           |
| `localectl`  | [`systemd`](https://systemd.io/)                                         | `kblayout`                                | Getting supported keyboard layouts                                           |
| `mpv`        | [`mpv`](https://mpv.io/)                                                 | `ytmpv`                                   | Playing video information                                                    |
| `scrot`      | [`scrot`](https://manpages.ubuntu.com/manpages/xenial/man1/scrot.1.html) | `screencap`                               | Screenshot making                                                            |
| `setxkbmap`  | [`X11`](https://www.x.org/wiki/)                                         | `kblayout`                                | Setting the keyboard layout                                                  |
| `youtube-dl` | [`youtube-dl`](https://youtube-dl.org/)                                  | `ytmpv`                                   | Getting YouTube's video formats                                              |

## Configuration

You can configure the scripts that have configuration files via
```sh
$HOME/.config/bash-scripts/
```

Scripts that use configuration files are listed below:

| Script             | Intended use                      | Should it be manually edited? |
| -                  | -                                 | -                             |
| kblayout           | Favorite layouts                  | ✔️                             |
| wtrcode            | Weather codes                     | ✔️                             |

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)
