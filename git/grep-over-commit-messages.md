# Grep over Commit Messages

The `git log` command supports a `--grep` flag that allows you to do a text
search (using grep, obviously) over the commit messages for that repository.
For the git user that writes descriptive commit messages, this can come in
quite handy. In particular, this can be put to use in an environment where
the standard process involves including ticket and bug numbers in the commit
message. For example, finding bug `#123` can be accomplished with:

```bash
$ git log --grep="#123"
```

See `man git-log` for more details.

[source](https://til.hashrocket.com/posts/7ad97e143b-grep-over-commit-messages)
