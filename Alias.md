# Alias
To add alias write:

`git config --global alias.<Alias Name> <Alias command>`


These alias is written as:

<Alias name> `<Alias command>` <Alias description>


## General

alias `config --get-regexp ^alias\.` This lists all alias.

addandcommit `!git add -A && git commit` This stages all files and commits them.

rename `!git branch -m` Rename your current branch.

pum `pull upstream master` Pulls upstream master.

por `push origin $(git branch-name)` Pushes active branch to origin

cm `checkout master` Checkout master

stashdiff `!sh -c 'git difftool stash@{$1}' -` See diffs between a stash and current branch exampe use: `git stashdiff 1`.

exclude `!sh -c 'echo "$1" >> .git/info/exclude' -` add file to the exclude file


## Management and status

currenthash `rev-parse HEAD` Gets the current hash.

discardall `"!git stash save "CHECKPOINT - discardAll"; git stash apply; git checkout -- ."` Creates a checkpoint in stash and discards all that is staged.

checkpoint `"!git stash save "CHECKPOINT"; git stash apply"` Creates a checkpoint in the stash.

resetfile `checkout --` Reset a file.

