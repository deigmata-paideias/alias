# Alias

alias for Mac

## cd

alias ".."="cd .."

alias "..."="cd ../.."

alias "...."="cd ../../.."

## kubectl

alias clr="clear"

alias mk="make"

alias k="kubectl"

alias kg="kubectl get"

alias ka="kubectl apply"

alias kcf="kubectl create -f"

alias kd="kubectl describe"

alias klf="kubectl logs -f"

## git

～/.gitconfig

```
[alias]
    br = branch
    c  = commit -s -m
    co = checkout
    ch = cherry-pick
    dump = cat-file -p
    hist = log --pretty=format:'%C(yellow)[%ad]%C(reset) %C(green)[%h]%C(reset) | %C(red)%s %C(bold red){{%an}}%C(reset) %C(blue)%d%C(reset)' --graph --date=short
    st = status
    type = cat-file -t
```

## docker

## python 

alias py="python3"

alias pi="pip3 install"

alias sv="source venv/bin/active"

# grep/egrep

alias grep="grep --color=auto"
