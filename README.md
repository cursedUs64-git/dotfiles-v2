# dotfiles-v2
## NOTES:

I use:

```

emerge -avuDN

```
to always install my packages.

To use `.bashrc`, install oh-my-bash, ble.sh and lsd (LS but made with Rust, icons, and more colourful)


To use `gentoo/portage/make.conf`, you can either link (`ln -sf`) it to `/etc/portage/make.conf` OR you can copy-paste it to `/etc/portage`.

## INSTALLATION

### 1 - Install Packages

My dotfiles are still a WIP and im lazy for now, so you have to find the packages by yourself and install them. (Specifically, for NeoVim, Hyprland, Waybar). Install KiTTY for the Terminal Emulator.

### 2 - Clone the Repo

```

git clone --bare https://github.com/cursedUs64-git/dotfiles-v2.git $HOME/.dotfiles

alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

dotfiles checkout

```

## SYNCING

### Sync

You can sync using the `dotfiles` alias I have included in `.bashrc` by the following:
```

dotfiles pull

```

# File Structure

```

gentoo/portage - Has make.conf

.config - Has my actual dotfiles

.bashrc - BASH config

Pictures - Has wallpaper

```
