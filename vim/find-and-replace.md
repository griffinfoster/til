# Find and Replace

The `:substitute` command searches for a text pattern, and replaces it with a text string. There are many options, but these are what you probably want:

Find each occurrence of 'foo' (in all lines), and replace it with 'bar'.

`:%s/foo/bar/g`

Find each occurrence of 'foo' (in the current line only), and replace it with 'bar'.

`:s/foo/bar/g`

Change each 'foo' to 'bar', but ask for confirmation first.

`:%s/foo/bar/gc`

[source](http://vim.wikia.com/wiki/Search_and_replace)