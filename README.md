# Dotfiles

This repository contains my personal dotfiles - the configuration files and scripts that shape my Linux desktop environment. From window manager settings to application configurations, these files help me maintain a consistent, productive workflow across my systems.

## Installation

Clone and set up my dotfiles with these commands:

```bash
# Clone the repository as a bare git repository
git clone --bare git@github.com:yaniselbeilk/dotfiles.git $HOME/.dotfiles

# Create a convenient alias for managing dotfiles
alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

# Hide untracked files to keep things clean
config config --local status.showUntrackedFiles no

# Make the alias permanent
echo "alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc
```