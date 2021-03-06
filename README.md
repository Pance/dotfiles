# Pance’s dotfiles
These dotfiles contain mostly Vim settings and the [Solarized color scheme](http://ethanschoonover.com/solarized) for Vim. These dotfiles are intended to be used alongside [oh-my-zsh](https://github.com/Pance/oh-my-zsh).
Additionally, this project installs [pathogen.vim](https://github.com/tpope/vim-pathogen) plugins as [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules):
* [vim-colors-solarized](https://github.com/altercation/vim-colors-solarized)
* [vim-airline](https://github.com/bling/vim-airline)

This project is a customized fork of the excellent [dotfiles by Mathias Bynens](https://github.com/mathiasbynens/dotfiles)

## Installation

**Warning:** If you want to give these dotfiles a try, you should first fork this repository, review the code, and remove things you don’t want or need. Don’t blindly use my settings unless you know what that entails. Use at your own risk!

### How to install using Git and the bootstrap script

```bash
git clone https://github.com/Pance/dotfiles.git --recursive && cd dotfiles && source bootstrap.sh
```

To update, `cd` into your local `dotfiles` repository and then:

```bash
# update each git submodule before running bootstrap.sh
git submodule foreach git pull origin master
source bootstrap.sh
```

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

```bash
./brew.sh
```
