```zsh
[ -f "$HOME/.local/share/zap/zap.zsh" ] && source "$HOME/.local/share/zap/zap.zsh"

# History Settings
export HISTSIZE=1000000
export SAVEHIST=1000000
export HISTFILE=~/.zsh_history
export HISTTIMEFORMAT="[%F %T] "

setopt HIST_FIND_NO_DUPS
setopt INC_APPEND_HISTORY
setopt EXTENDED_HISTORY
setopt HIST_IGNORE_ALL_DUPS

# Aliases File
plug "$HOME/.config/zsh/aliases.zsh"

# plugins
plug "zsh-users/zsh-syntax-highlighting"
plug "zsh-users/zsh-autosuggestions"
plug "$HOME/.config/zsh/sudo.plugin.zsh"
. /home/linuxbrew/.linuxbrew/opt/asdf/libexec/asdf.sh

# z jump around
. $HOME/.config/zsh/z/z.sh

# Tab navigation
autoload -Uz compinit && compinit
compinit
zstyle ':completion:*' menu select

# Caseinsenstive Completion
zstyle ':completion:*' matcher-list '' 'm:{a-zA-Z}={A-Za-z}'

# PowerLevel 10k
# [[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
# source ~/powerlevel10k/powerlevel10k.zsh-theme

eval "$(starship init zsh)"

```

### Aliases
```zsh
# Hisotry Aliases
alias h='history'
alias hs='history | grep'
alias hsi='history | grep -i'

# List directory contents
alias lsa='ls -lah'
alias l='ls -lah'
alias ll='ls -lh'
alias la='ls -lAh'

# APT
alias i='sudo apt install '
alias update='sudo apt update'
alias upgrade='sudo apt upgrade'

# Change Directories
alias ..='cd ..'
alias -g ...='cd ../..'
alias -g ....='cd ../../..'
alias -g .....='cd ../../../..'
alias -g ......='cd ../../../../..'

# Copy Files content keyboard
function copyfile {
  emulate -L zsh
  clipcopy $1
}

alias md='mkcd '
alias cls='clear'
alias x='exit'

function mkcd takedir() {
  mkdir -p $@ && cd ${@:$#}
}

function takeurl() {
  local data thedir
  data="$(mktemp)"
  curl -L "$1" > "$data"
  tar xf "$data"
  thedir="$(tar tf "$data" | head -n 1)"
  rm "$data"
  cd "$thedir"
}

function takegit() {
  git clone "$1"
  cd "$(basename ${1%%.git})"
}

function take() {
  if [[ $1 =~ ^(https?|ftp).*\.(tar\.(gz|bz2|xz)|tgz)$ ]]; then
    takeurl "$1"
  elif [[ $1 =~ ^([A-Za-z0-9]\+@|https?|git|ssh|ftps?|rsync).*\.git/?$ ]]; then
    takegit "$1"
  else
    takedir "$@"
  fi
}

# Rails Aliases
alias rc='rails console'
alias rs='rails server'
alias rdm='rails db:migrate'
alias rds='rails db:seed'

```