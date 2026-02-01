# Alias

alias for Linux/Mac

> Tips: use `alias` show system alias.

## nefetch and onefetch

alias s="neofetch"

alias c="onefetch"

## make

alias mk="make"

## zsh

alias sz="source ~/.zshrc"

## fzf

alias f="fzf"

alias ff='fzf --preview "bat --color=always {}"'

## grep

alias grep="grep --color=auto"

## claude

alias cl='claude --dangerously-skip-permissions --append-system-prompt "$(cat ~/.claude/system-prompt.txt)"'

## du

alias du1="du -hd 1"

## clear

alias clr="clear"

alias c="clear"

## cd

alias "."="cd .."

alias ".."="cd ../.."

alias "..."="cd ../../.."

alias "...."="cd ../../../.."

or:

alias "cd1"="cd .."

alias "cd2"="cd ../.."

alias "cd3"="cd ../../.."

alias "cd4"="cd ../../../.."

## kubectl

alias k="kubectl"

alias kg="kubectl get"

alias ke="kubectl edit"

alias kexec="kubectl exec -it"

alias klf="kubectl logs -f"

alias ka="kubectl apply"

alias kcf="kubectl create -f"

alias kd="kubectl describe"

## git

～/.gitconfig

```
[alias]
    # git branch ==> git b
    br = branch
    # git commit -s -m "xx" ==> git c "xxx"
    c  = commit -s -m
    co = checkout
    ch = cherry-pick
    dump = cat-file -p
    hist = log --pretty=format:'%C(yellow)[%ad]%C(reset) %C(green)[%h]%C(reset) | %C(red)%s %C(bold red){{%an}}%C(reset) %C(blue)%d%C(reset)' --graph --date=short
    st = status
    type = cat-file -t
```

alias gg="git clone"

alias gpl="git pull"

alias gps="git push"

alias ga="git add ."

alias gss="git stash save"

alias gsp="git stash pop"

## docker

alias dex="sudo docker exec -it"

alias drm="docker rm $(docker ps -a -q)" # remove all containers

alias dclean="docker system prune -af" # clean system

## python 

alias py="python3"

alias pi="pip3 install"

alias sv="source venv/bin/active"

alias pyserve="python3 -m http.server" # pyserve 58080

# grep/egrep

alias grep="grep --color=auto"

# macos ip
alias myip=ifconfig en1 | grep inet | grep -v inet6 | cut -d ' ' -f2
