# Ubuntu
[![cc][cc_image]][cc_url]

my ubuntu setting

## Version

* Ubuntu 21.04 (Hirsute Hippo)

## Installation

### Tool

```shell
$ sudo -i
# apt install git curl fzf
# apt install python3-pip golang
```

### Service

```shell
$ sudo -i
# apt install chrony
# apt install openssh-server
# apt install snmpd snmptrapd
# apt install squid
```

### cargo

* cargoのインストール

```shell
$ sudo -i
# apt install cargo
```

* rustツールのインストール

```shell
$ cargo install gitui bat lsd fd-find ripgrep
```

* 設定

```shell
$ set -g fish_user_paths "$HOME/.cargo/bin" $fish_user_paths
```

### ghq

```shell
$ go get github.com/x-motemen/ghq
```

* 設定

```shell
$ set -g fish_user_paths "$HOME/go/bin" $fish_user_paths
```

### neovim

* インストール

```shell
$ sudo -i
# apt install neovim
```

* 設定

```shell
$ ghq get kazurri/dotfiles
[C-g] -> dotfiles
$ cp -pr .config/nvim ~/.config/
```

### fish

* fishのインストール

```shell
$ sudo -i
# apt install fish
```

* fisherとツールのインストール

```shell
$ url https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish
$ fisher install decors/fish-ghq
$ fisher install jethrokuan/fzf
$ fisher install jethrokuan/z
```

* 設定

```shell
$ chsh -s /usr/bin/fish
[C-g] -> dotfiles
$ cp -pr .config/fish ~/.config/
```

### starship

* インストール

```shell
$ curl -fsSL https://starship.rs/install.sh | sh
```

* 設定

```shell
[C-g] -> dotfiles
$ cp -p .config/starship.toml ~/.config/
```

### tmux

* インストール

```shell
$ sudo -i
# apt install tmux
```

* TPMのインストール

```shell
$ mkdir -p ~/.tmux/plugins
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

* 設定

```shell
[C-g] -> dotfiles
$ cp -p .tmux* ~/
```

### Gnome Terminal

* Preferences＞Unnamed＞Text
  * Custom fontを指定してチェックを入れる

### Font

* [HackGen](https://github.com/yuru7/HackGen/releases)

## License

[![cc][cc_image]][cc_url]

## Author

[Kazuhiro Namigata](mailto:kazurri@gmail.com)

[cc_image]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg?style=flat-square
[cc_url]: http://creativecommons.org/licenses/by/4.0/
