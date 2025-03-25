# My dotfiles

This directory contains the dotfiles for my system.

## What is GNU stow?

GNU stow is a useful utility that centralizes your files in a single directory
and creates symlinks for them, meaning the program can still access the
configuration files.

Here is a great tutorial on
[how to get stated with GNU stow in 8 minutes](https://www.youtube.com/watch?v=y6XCebnB9gs).

## Requirements

Ensure you have the following installed on your system:

### Git

```sh
sudo apt install git
```

### Stow

```sh
sudo apt install stow
```

## Installation

Download the repo in your $HOME directory using git

```sh
cd $HOME
git clone https://github.com/erikvelf/dotfiles.git
```

Then use GNU stow to create symlinks

```sh
cd $HOME/dotfiles
stow .
```

To see the configuration files use tree command

```sh
tree -I ".git" -a $HOME/dotfiles
```
