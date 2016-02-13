# Create with Timestamp

Today I learned how to interpolate a timestamp at the command line. Here are two examples:

For a file:

```
$ touch test_$(date +%s).md
$ ls
test_1435435401.md
```

For a git branch:

```
$ git checkout -b pull_request_$(date +%s)
Switched to a new branch 'pull_request_1435435344'
```

The timestamp represents seconds since the UNIX epoch.

[source](https://til.hashrocket.com/posts/192721096f-create-with-timestamp)
