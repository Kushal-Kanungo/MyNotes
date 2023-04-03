After installing **OH MY ZSH** copy this code in '~/.zshrc'

## .zshrc
```sh

export ZSH="$HOME/.oh-my-zsh"

# <======================| HISTORY SETTINGS STARTS |===========================>
HISTSIZE=1000000
SAVEHIST=1000000
HISTFILE=~/.zsh_history

# Ignores these commands to write in history
export HISTORY_IGNORE="(ls|cd|pwd|exit|sudo reboot|history|cd -|cd ..|eb|clr|wrsb|wrsf|wdf|wdb|gs|x|obs|ng s|rails s|ps|code .|h|src|pgs|..)"

# Do not write duplicate commands to write in history file
setopt HIST_IGNORE_ALL_DUPS

# <=======================| HISTORY SETTINGS ENDS |===============================>

# ZSH_THEME="powerlevel10k/powerlevel10k"

plugins=(git zsh-autosuggestions zsh-syntax-highlighting history sudo web-search copyfile dirhistory history-substring-search colorize you-should-use)

source $ZSH/oh-my-zsh.sh

source $HOME/.config/zsh/.zsh_aliases

# Clone (https://github.com/rupa/z.git) first than give its path
. $HOME/.config/zsh/z.sh

# Installl Starship First 
eval "$(starship init zsh)"

# HomeBrew PATH
# echo '# Set PATH, MANPATH, etc., for Homebrew.' >> /home/kushal/.profile
# echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> /home/kushal/.profile
# eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"

#PATH for openssl 3
export PATH="/home/linuxbrew/.linuxbrew/opt/openssl@3/bin:$PATH"
export PATH="/home/linuxbrew/.linuxbrew/opt/icu4c/bin:$PATH"
export PATH="/home/linuxbrew/.linuxbrew/opt/icu4c/sbin:$PATH"

# asdf path
. /home/linuxbrew/.linuxbrew/opt/asdf/libexec/asdf.sh
export PATH="$PATH:/home/kushal/.asdf/shims"

# curl path
export PATH=$HOME/curl/bin:$PATH

export PKG_CONFIG_PATH="/home/linuxbrew/.linuxbrew/opt/openssl@3/lib/pkgconfig"

# openssl
export LDFLAGS="-L/home/linuxbrew/.linuxbrew/opt/openssl@3/lib"
export CPPFLAGS="-I/home/linuxbrew/.linuxbrew/opt/openssl@3/include"

# readline
export LDFLAGS="-L/home/linuxbrew/.linuxbrew/opt/readline/lib"
export CPPFLAGS="-I/home/linuxbrew/.linuxbrew/opt/readline/include"

# zlib
export LDFLAGS="-L/home/linuxbrew/.linuxbrew/opt/zlib/lib"
export CPPFLAGS="-I/home/linuxbrew/.linuxbrew/opt/zlib/include"

source <(ng completion script)
```

## .zsh_aliases
```zsh
# =============== ALIASES====================

# Custom Aliases
alias m='micro'
alias update='sudo apt update'
alias upgrade='sudo apt upgrade'
alias c='code'
alias eb='code ~/.zshrc'
alias ep='micro ~/.profile'
alias ea='micro ~/.zsh_aliases'
alias cls='clear'
alias get='sudo apt install'
alias cat='batcat'
alias x='exit'
alias e='echo'
alias src='source ~/.zshrc'

#Version Checks
alias rv='ruby --version'
alias rav='rails --version'
alias nv='node --version'
alias av='ng version'
alias bi='bundle install'

# Git aliases
alias add='git add'
alias commit='git commit -m'
# alias gs='git status'
alias branch='git checkout '
# alias ga='git add'
# alias gd='git diff'
alias gl='git log --oneline'

#asdf aliases
alias a='asdf'
alias ai='asdf install'
alias ali='asdf list'
alias alir='asdf list ruby'
alias alin='asdf list nodejs'
alias aliar='asdf list all ruby'
alias alian='asdf list all nodejs'
alias alr='asdf local ruby'
alias agr='asdf global ruby'
alias aln='asdf local nodejs'
alias agn='asdf global nodejs'

# Install LSD first to get colored ls
alias ls='lsd'

# Start
alias pgs='pg_ctl start'
alias wdb='cd ~/WRS/WDBackend'
alias wdf='cd ~/WRS/WDFrontend'
alias rs='rails server'
alias rc='rails console'
alias ngs='ng server'
alias wrsb='cd ~/WRS/WRSBackend' 
alias wrsf='cd ~/WRS/WRSFrontend' 
alias obs='nohup ~/Downloads/Obsidian-1.1.9.AppImage &'
alias src='source ~/.zshrc'
alias rd='bundle exec rdbg --open -n -c -- bundle exec rails s'
# ================ ALIASES END==================

```
