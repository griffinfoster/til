# Confirm each find replace in vim

If you are running a find replace on the whole file, you might want to use the `c` flag at the end of your replace command which will make vim  confirm each replace.

Example:

```viml
:s/(.*)/test/gc
```

h/t @joshbranchaud
