# Ubuntu
[![cc][cc_image]][cc_url]

my ubuntu setting

## Version

* Ubuntu 21.04 (Hirsute Hippo)

## Installation

### Tool

```plaintext
$ sudo -i
# apt install bat
# apt install curl
# apt install exa
# apt install fd-find
# apt install fish
# apt install fzf
# apt install git
# apt install golang
# apt install neovim
# apt install python3-pip
# apt install ripgrep
# apt install tmux
```

### Service

```plaintext
$ sudo -i
# apt install chrony
# apt install openssh-server
# apt install snmpd snmptrapd
# apt install squid
```

### go

```plaintext
$ su - ubuntu
$ go get github.com/x-motemen/ghq
```

### Font

* [HackGen](https://github.com/yuru7/HackGen/releases)

## Settings

### Gnome Terminal

* Preferences＞Unnamed＞Text
  * Custom fontを指定してチェックを入れる

### fish

```plaintext
chsh -s /usr/bin/fish
curl https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish
fisher install decors/fish-ghq
fisher install jethrokuan/fzf
fisher install jethrokuan/z
set -g fish_user_paths "$HOME/go/bin" $fish_user_paths
ghq get kazurri/dotfiles
Ctrl+g -> dotfiles
cp -pr .config/fish ~/.config/
```

### neovim

```plaintext
[C-g] -> dotfiles
cp -pr .config/nvim ~/.config/
```

### tmux

```plaintext
mkdir -p ~/.tmux/plugins
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
[C-g] -> dotfiles
cp -p .tmux* ~/
```

## License

[![cc][cc_image]][cc_url]

## Author

[Kazuhiro Namigata](mailto:kazurri@gmail.com)

[cc_image]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg?style=flat-square
[cc_url]: http://creativecommons.org/licenses/by/4.0/
