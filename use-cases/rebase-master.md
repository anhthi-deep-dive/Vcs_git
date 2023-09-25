# Rebase master

```
  /* Make sure master branch is updated */

  git checkout master
  git pull origin master

  /* Move feature/todo branch on top of master */

  git checkout feature/todo
  git rebase origin master
  git push origin feature/todo -f
```

In case of conflicts with master branch

```
  // ...resolve the conflicts

  git add .
  git rebase --continue
  git push origin feature/todo -f
```
