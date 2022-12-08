# Ubuntu
[![cc][cc_image]][cc_url]

my ubuntu setting

## Version

* Ubuntu 22.10 (Kinetic Kudu)

## Installation

### Tool

```sh
$ sudo -i
# apt install git curl fzf
# apt install python3-pip golang
```

### Service

```sh
$ sudo -i
# apt install chrony
# apt install openssh-server
# apt install snmpd snmptrapd
# apt install squid
```

### fish

* fishのインストール

```sh
$ sudo -i
# apt install fish
```

* fisherとツールのインストール

```sh
$ fish
> curl https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish
> fisher install decors/fish-ghq
> fisher install jethrokuan/fzf
> fisher install jethrokuan/z
```

* 設定

```sh
> chsh -s /usr/bin/fish
```

### starship

* インストール

```sh
> curl -fsSL https://starship.rs/install.sh | sh
```

### tmux

* インストール

```sh
$ sudo -i
# apt install tmux
```

* TPMのインストール

```sh
> mkdir -p ~/.tmux/plugins
> git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### rust

* rustのインストール

```sh
> curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

* rustツールのインストール

```sh
> cargo install gitui bat lsd fd-find ripgrep
```

### ghq

```sh
> go install github.com/x-motemen/ghq@latestls
```

### neovim

* インストール

```sh
$ sudo -i
# apt install neovim
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
