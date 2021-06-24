# git-playground

## Your branch and 'origin/main' have diverged and have 2 and 3 different commits each, respectively.

To get this message:
```
On branch main
Your branch and 'origin/main' have diverged,
and have 3 and 4 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean
```

1. clone this repo
2. `git rebase -i HEAD~4`
3. delete the first commit (at the top)
4. do a `git status`

Note: doing a `git pull` will give:
```
git pull
fatal: Not possible to fast-forward, aborting.
```

Fix:

`git rebase origin/main`

