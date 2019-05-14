---
title: "Remove commit history"
layout: default
date: 2019-05-14
---
- [how-to-delete-all-commit-history-in-github](https://stackoverflow.com/questions/13716658/how-to-delete-all-commit-history-in-github) from stackoverflow

1. Checkout

    `git checkout --orphan latest_branch`

2. [Update the index](https://git-scm.com/docs/git-add#Documentation/git-add.txt--A) git Documentation

    `git add -A`

3. Commit the changes

    `git commit -am "commit message"`

4. Delete the branch

    `git branch -D master`

5. Rename the current branch to master

    `git branch -m master`

6. Finally, force update your repository

    `git push -f origin master`
