# A bunch of Bash scripts I have created.

## Current list:

| Name               | Function                                                           | Arguments               |
| -                  | -                                                                  | -                       |
| cheat              | Easily bring up a curl cheat sheet from cheat.sh                   | Infinitely many         |
| lmmsProjectBooter  | Load projects from a specific directory into LMMS                  | -d                      |
| nerdFontItemPicker | Return specific nerd font characters into `stdout`                 |                         |
| qrcodeterm         | Generate QR codes in the terminal                                  | Infinitely many         |
| wttrcode           | Read wetter information via curl using location codes              |                         |
| wttrin             | Read wetter information via curl using a custom location arguement | None or infinitely many |

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

## Thanks

The following scripts were made possible by:

- ⭐ [Igor Chubin](https://github.com/chubin)'s [wttr.in](https://github.com/chubin/wttr.in), [qrenco.de](https://github.com/chubin/qrenco.de) and [cheat.sh](https://github.com/chubin/cheat.sh)

