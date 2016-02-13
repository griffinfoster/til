# Open Files in vim Splits

You can open multiple files with Vim in vertical or horizontal splits. To demonstrate, I'll create some test files.

```
$ touch a.txt b.txt c.txt d.txt e.txt
```

From the command line, `vim -o *.txt` will open these five files in vertical splits. `vim -O *.txt` will open them in horizontal splits. This is great for quickly comparing two files side-by-side.

[source](https://til.hashrocket.com/posts/70ce551e7a-open-files-in-vim-splits)
