# Git aliases
## Setting up the aliases
1. Open git global configuration:
```
git config --global -e
```

2. Append this:
```
[alias]
        co = checkout
        cob = checkout -b
        br = branch
        ci = commit
        st = status
        cim = commit -m
        cia = commit --amend --no-edit
        ciam = commit --ammend -m
        rb = rebase
        rbi = rebase -i
        pl = pull
        ft = fetch
        ftp = fetch --prune
        aa = add .
        ps = push
        psf = push -f
        cfg = config --global
        lg = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(auto)%d%C(reset)' --all
        s = status --short
        cbr = branch --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) %(color:green)(%(committerdate:relative)) [%(authorname)]' --sort=-committerdate
```
