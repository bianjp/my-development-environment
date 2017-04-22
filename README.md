# My development environment

My choices and configurations about development environment.

## Operating System

[Arch Linux](https://www.archlinux.org/)

Use [archlinux-installer](https://github.com/bianjp/archlinux-installer) to install it.

## Desktop Environment

Gnome 3 with numix themes([numix-gtk-theme](https://www.archlinux.org/packages/community/any/numix-gtk-theme/), [numix-circle-icon-theme-git](https://aur.archlinux.org/packages/numix-circle-icon-theme-git/))

## Browsers

* Firefox for primary use
* Google chrome as an alternative

## Dotfiles

Such as .vimrc, .bashrc, .bash_profile, .gitconfig, .gemrc

Save in Dropbox and link via symbolic link.

## Editor

### Sublime Text 3

```
yaourt -S sublime-text-dev-imfix2

# sublime configurations
# rm -r ~/.config/sublime-text-3/Packages/User
git clone https://github.com/bianjp/sublime-settings.git ~/.config/sublime-text-3/Packages/User
```

### Vim

```
sudo pacman -S vim
```

## Languages

### Java

```
sudo pacman -S jdk8-openjdk openjdk8-doc
```

## Lint tools

### Shell Script

```
sudo pacman -S shellcheck
```

### CSS

```
yaourt -S stylelint
yaourt -S stylelint-config-standard

cat <<EOF > ~/.stylelintrc
{
  "extends": "/usr/lib/node_modules/stylelint-config-standard/"
}
EOF
```

## Utilities

```
yaourt -S besttrace

yaourt -S java-repl-git
```
