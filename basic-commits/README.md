# Git Kata: Basic Commits
This kata will introduce you to the `git add` and `git commit` commands.

This is a very introductory kata. if you have used `git status`, `git log --oneline --graph`, `git add` and `git commit` extensively you should probably skip it.

You can look at the bottom of this file, if you have not yet done basic git configuration.

## Setup:

1. Run `. setup.sh` (or `.\setup.ps1` in PowerShell)

## The task

1. Use `git status` to see which branch you are on.
2. What does `git log` look like?
3. Create a file
4. What does the output from `git status` look like now?
5. `add` the file to the staging area
6. How does `git status` look now?
7. `commit` the file to the repository
8. How does `git status` look now?
9. Change the content of the file you created earlier
10. What does `git status` look like now?
11. `add` the file change
12. What does `git status` look like now?
13. Change the file again
14. Make a `commit`
15. What does the `status` look like now? The `log`?
16. Commit the newest change

## Useful commands
- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` to create a file (or `sc filename ''` in PowerShell)
- `echo content > file` to overwrite file with content (or `sc filename 'content'` in PowerShell)
- `echo content >> file` to append file with content (or `ac filename 'content'` in PowerShell)


## Git Initial Configuration
1. `git config --global user.name "John Doe"`
1. `git config --global user.email "johndoe@example.com`

For the vim scared:
- `git config --global core.editor nano`

For the windows peeps:
- `git config --global core.editor notepad`

Other editor options:
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst"`


Answers:
Part 2
fatal: your current branch 'master' does not have any commits yet

Part 4 
 On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        sam.txt

nothing added to commit but untracked files present (use "git add" to track)

Part 6
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   sam.txt

Part 8
On branch master
nothing to commit, working tree clean

Part 10
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   sam.txt

no changes added to commit (use "git add" and/or "git commit -a”)

Part 12
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   sam.txt

Part 15
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   sam.txt

no changes added to commit (use "git add" and/or "git commit -a”)

Log:
commit 58ba29b7561f7e2c01348c0ad5b3a9b9e0fa70e4 (HEAD -> master)
Author: Simran Ahuja <simran8072@gmail.com>
Date:   Fri Jan 24 14:30:59 2020 -0800

    more editing

commit 3aed1cabad1a6a8d7534c32c0215a1c385c17b79
Author: Simran Ahuja <simran8072@gmail.com>
Date:   Fri Jan 24 14:28:03 2020 -0800

    editted

Part 16
On branch master
Changes not staged for commit:
        modified:   sam.txt

no changes added to commit
