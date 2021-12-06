# bash-profile
Useful settings for a new machine

## extend command history
```
sudo nano ~/.bashrc
HISTSIZE=900000000
HISTFILESIZE=9000000
```

## fancy prompt
```
export PS1="\[\e[90m\][\[\e[36m\]SVRNAME\[\e[90m\]]\[\e[m\]\[\e[96m\]\w\[\e[m\]\\$ "
```

## bash aliases
```
nano ~/.bash_aliases
````

## system
```
alias ll='ls -l'
alias la='ls -A'
alias gigs='du -h --max-depth=3 * | grep "[0-9]G\>"'
alias sz='du -h --max-depth=1 | sort -hr'
```

## git
```
alias gs='git status'
alias co='git checkout'
alias gb='git for-each-ref --sort=committerdate refs/heads/ --format="%(HEAD) %(color:red)%(objectname:short)%(color:reset): %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) - %(authorname) (%(color:green)%(committerdate:relative)%(color:reset))"'
```
