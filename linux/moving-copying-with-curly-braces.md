# Moving/Copying with Curly Braces

This might be old news, but it's relatively new to me, so here: you can move/copy files using curly braces; the text before the comma is replaced with the text after, so instead of this:

```bash
$ mv awesome/explosion.gif rad/explosion.gif
```

Do this:

```bash
$ mv {awesome,rad}/explosion.gif
```

Works great for any subset of the argument (even partial file/folder names).

[source](https://til.hashrocket.com/posts/c32f2c4f86-moving-copying-with-curly-braces)
