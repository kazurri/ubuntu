# Ubuntu
[![cc][cc_image]][cc_url]

my ubuntu setting

## Version

* Ubuntu 21.04 (Hirsute Hippo)

## Installation

### Tool

```bash
$ sudo -i
# apt install bat curl exa fd-find fish fzf git ripgrep tmux
# apt install golang python3-pip
```

### Service

```bash
$ sudo -i
# apt install chrony
# apt install openssh-server
# apt install snmpd snmptrapd
# apt install squid
```

### go

```bash
$ su - ubuntu
$ go get github.com/x-motemen/ghq
```

### neovim

```bash
$ sudo -i
# apt install neovim
```

### Font

* [HackGen](https://github.com/yuru7/HackGen/releases)

## Settings

### Gnome Terminal

* Preferences＞Unnamed＞Text
  * Custom fontを指定してチェックを入れる

### fish

```bash
$ chsh -s /usr/bin/fish
$ url https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish
$ fisher install decors/fish-ghq
$ fisher install jethrokuan/fzf
$ fisher install jethrokuan/z
$ set -g fish_user_paths "$HOME/go/bin" $fish_user_paths
$ ghq get kazurri/dotfiles
[C-g] -> dotfiles
$ cp -pr .config/fish ~/.config/
```

### neovim

```bash
[C-g] -> dotfiles
$ cp -pr .config/nvim ~/.config/
```

### tmux

```bash
$ mkdir -p ~/.tmux/plugins
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
[C-g] -> dotfiles
$ cp -p .tmux* ~/
```

## License

[![cc][cc_image]][cc_url]

## Author

[Kazuhiro Namigata](mailto:kazurri@gmail.com)

[cc_image]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg?style=flat-square
[cc_url]: http://creativecommons.org/licenses/by/4.0/
