# Command Memo repo

<br><br>

## Git Command

```bash
# in git bash

# setting config
$ git config --global user.name "hoge"
$ git config --global user.email "hoge@hige.com"


# initialize with clone version
$ git clone <url to repository>.git

# initialize with remote add version
$ git init # create .git files
$ git branch -M main # master -> main
$ git add <file or directory name>
$ git commit -m "commit message (In general, use 'initialize repository')"
$ git remote add origin <https://github.com/Yuto02D2-E2/repository name>
$ git push -u origin main # is the origin a local repository?
$ git pull origin main


# second or later time
$ git add <file or directory name> # select add files
  git add . # add all changed files
$ git commit -m "commit message"
$ git push
  git push -u origin <branch name> # when in a branch except main
$ git pull


# about branch
$ git branch <branch name to create>
$ git checkout <next work branch name>
$ git branch -b <create and next work branch name>
$ git branch -D <branch name to delete>
$ git push --delete origin <branch name to delete>
$ git branch -m <branch name to rename>
$ git merge <branch name to merge with main>


# other command
$ git reset --soft/hard HEAD~{n} # reset n prev version
$ git commit --amend "new commit message" # reset commit message
$ git log
$ git status
$ git diff
$ git show <hash-value>
$ git rm -f <file name> # delete file


# not sure or never used
$ git fetch
$ git stash


# how to use branch (ex: branch name is dev)
$ git branch -b dev # create and move
$ git add .
$ git commit -m "commit message"
$ git push origin dev
$ git checkout main
$ git merge dev
$ git push origin main
```

<br><br>

## Linux Command
```bash

$ man <command name> # MANual
$ systemctl poweroff/reboot # SYSTEM ConTroL
$ systemctl start/stop/restart/reload/status/enable/disable <service>
$ systemctl daemon-reload
$ su <user-name:root/hoge> # Switch User

# check info
$ htop
$ lscpu
$ uname -a

# network
$ ip addr/ipconfig/ifconfig
$ ping
$ netstat
$ ssh # Secure SHell
$ scp # Ssh CoPy

# file
$ touch hoge.txt # make file
$ mkdir -p hoge-dir/fuga-dir # make directory with parent
$ rm hoge.txt # delete file
$ rm -r hoge-dir # delete directory
$ mv hoge.txt fuga.txt # rename or move file
$ cp <name:from> <name:to> # CoPy file or directory
$ chmod u/g/o/a +/-/= <permission> <file name> # CHange MODe
$ diff hoge.txt fuga.txt

# tool
$ grep hoge

```

<br><br>

## Vi Command
```vim
" use double quotation to comment out

:wq! " Write/Quit/force
:u " Undo
:redo
:set <hoge>
:/%s/hoge/fuga/gc " swap string

" search
/hoge " next/prev -> n/N
/\vhoge " use regular expression

h/j/k/l " move cursor (left/down/up/right)
V " visual mode (select line)
o/O " insert blank line
p/P " paste
i/I " switch to insert mode
a/A
```

### Tips

```vim
" write code to .vimrc or set it in command mode
set nocompatible " turn off compatibility mode
set backspace=indent,eol,start " enable backspace
```

<br><br>

## References
- [Git docs](https://git-scm.com/docs)
- [GitHub docs](https://docs.github.com/ja/github)
