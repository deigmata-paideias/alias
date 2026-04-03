# Alias

alias for Linux/Mac

> Tips: use `alias` show system alias.

## nefetch and onefetch

alias sf="neofetch"

alias of="onefetch"

alias ff="fastfetch"

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
    st = "!f() { stats=$( { if git rev-parse --verify HEAD >/dev/null 2>&1; then git diff --numstat HEAD --; else git diff --cached --numstat --; git diff --numstat --; fi; } 2>/dev/null | { add=0; del=0; while\n  read -r a d _; do [ -z \"$a\" ] && a=0; [ \"$a\" = \"-\" ] && a=0; [ -z \"$d\" ] && d=0; [ \"$d\" = \"-\" ] && d=0; add=$((add + a)); del=$((del + d)); done; printf \"%s %s\" \"$add\" \"$del\"; } ); add=${stats% *}; del=${stats#* }; total=$((add + del));\n  green=$(git config --get-color \"\" green); red=$(git config --get-color \"\" red); reset=$(git config --get-color \"\" reset); echo \"Change lines: $total  ${green}+${add}${reset}  ${red}-${del}${reset}\"; git status \"$@\"; }; f"
    type = cat-file -t
```

alias gg="git clone"

alias gpl="git pull"

alias gps="git push"

alias ga="git add ."

alias gss="git stash save"

alias gsp="git stash pop"

// fzf search branch name and checkout

alias gco="git branch | fzf | xargs git checkout"

## docker

alias dex="sudo docker exec -it"

alias drm="docker rm $(docker ps -a -q)" # remove all containers

alias dclean="docker system prune -af" # clean system

## python 

alias py="python3"

alias pi="pip3 install"

alias sv="source venv/bin/active"

alias pyserve="python3 -m http.server" # pyserve 58080

# macos ip
alias myip=ifconfig en1 | grep inet | grep -v inet6 | cut -d ' ' -f2
