# Resolve Merge Conflicts

Many time, when we do git push/pull or git merge, we end up with conflicts.

In most cases, solution to merge-conflict is as simple as discarding local changes or remote/other branch changes. Following is useful in those cases.

Find files with merge conflict by searching for all conflicting files.

```
grep -lr '<<<<<<<' .
```

Above will list all files which has marker special marker <<<<<<< in them.

At this point you may review each files. If the solution is to accept local/our version, run:

```
git checkout --ours PATH/FILE
```

If the solution is to accept remote/other-branch version, run:

```
git checkout --theirs PATH/FILE
```

[source](https://easyengine.io/tutorials/git/git-resolve-merge-conflicts/)