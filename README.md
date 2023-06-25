# My-aliases

# git aliases

```
alias gs="git status"
alias gl="git log --pretty=format:'%C(auto)%h - %C(bold blue)%an%Creset, %C(dim yellow)%ar%Creset : %s'"
```

```
alias gco="git checkout "
alias gcm="git checkout master"
alias gcd="git checkout develop"
alias gcu="git checkout uat"
alias gcq="git checkout qa"
```

# git set staging
```
alias gaa="git add ."
alias gc="git commit -m "
```

# git set upstream
alias gp="git push "

# git reset
alias nah="git reset --xhard &6 git clean -df"

# git get remote url name
alias grn="git remote get-url origin"

# git set url name
alias gsu="git remote set-url origin"

# Go to git repo alias
function openPjGitHubRepo() {
  gitUrl=$(git config --get remote.origin.url)
  open $gitUrl
}
alias gh="openPjGitHubRepo"
