# My Dotesfiles

## Installation

### In Linux/POSIX emulation (MSYS2, Cygwin, Git bash)

1. `alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'`
2. `git clone --bare git@github.com:ReeceRGGIL/dotfiles.git $HOME/.cfg`
3. `config checkout`
4. `config config --local status.showUntrackedFiles no`

## Command Prompt/Powershell

TODO

## Dotfiles

- .bash_aliases: Commands aliases are listed in this file. This file is sourced by .bashrc
- .bash_logout: Executed by bash when login shell exits
- .bash_profile: Executed for login shells (at login)
- .bashrc: Executed for interactive non-login shells (running a terminal emulator)
- .config/nvim/init.vim: Neovim configuration
- .gitconfig: Git configuration
- .gitignore: Global git ignore
- .inputrc: GNU Readline configuration file
- .tmux.conf: Tmux configuration file

## Requirements Expectations Considerations Side-effects

- .bash_aliases: None
- .bash_logout: None
- .bash_profile
- .bashrc
- .config/nvim/init.vim
    - Uses `curl` to download `plug`
    - Setup for 24-bit color support from the terminal. Colors will be wrong and/or broken without that support
    - Expects `$VIMCONFIG` to be set
- .gitconfig: None
- .gitignore: None
- .inputrc: None
- .tmux.conf: None

## Sources

- [The best way to store your dotfiles: A bare Git repository - Atlassian Developer](https://developer.atlassian.com/blog/2016/02/best-way-to-store-dotfiles-git-bare-repo/)
- [StreakCobra Comment - Ask HN: What do you use to manage dotfiles? - Hacker News](https://news.ycombinator.com/item?id=11070797)

## Resources

- [Github does dotfiles - dotfiles.github.io](gitfiles.github.io)
- [Awesome dotfiles - webpro - Github.com](https://github.com/webpro/awesome-dotfiles)
