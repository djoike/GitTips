# Alias
To add alias write:
`git config --global alias.<Alias Name> <Alias command>`

These alias is written as:
<Alias name> `<Alias commad>` <Alias description>

## General
alias `config --get-regexp ^alias\.` This lists all alias.
addandcommit `!git add -A && git commit` This stages all files and commits them.
rename `!git branch -m` Rename your current branch.
pum `pull upstream master` Pulls upstream master.

## Management and status
currenthash `rev-parse HEAD` Gets the current hash.
discardall `checkout -- .` Discards all that is staged.
resetfile `checkout --` Reset a file.