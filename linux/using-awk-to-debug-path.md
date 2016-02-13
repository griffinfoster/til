# Using awk to debug $PATH

If you ever tried printing your system PATH environment variable using `echo $PATH` you probably got something like this: 

```sh
/usr/local/heroku/bin:/usr/local/bin:/Users/username/.rvm/gems/ruby-2.2.2/bin:/Users/username/.rvm/gems/ruby-2.2.2@global/bin:/Users/username/.rvm/rubies/ruby-2.2.2/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/opt/X11/bin:.git/safe/../../bin:/Users/username/.bin:/usr/local/sbin:/Users/username/.rvm/gems/ruby-2.2.2/bin:/Users/username/.rvm/gems/ruby-2.2.2@global/bin:/Users/username/.rvm/rubies/ruby-2.2.2/bin:/Users/username/.rvm/bin:/Users/username/.rvm/bin:/Users/username/Dropbox/Developer/gocode/bin
```

Not a pleasant read.

I thought that would be a good opportunity to practice my `awk` scripting skills and came up with this:

```sh
echo $PATH | awk '{ n = split($0, paths, ":"); for (i=0; ++i <= n;) print i, paths[i] }'
```

It prints a numerically indexed list of the paths and prints them in separate lines.

```
1 /usr/local/heroku/bin
2 /usr/local/bin
3 /Users/username/.rvm/gems/ruby-2.2.2/bin
4 /Users/username/.rvm/gems/ruby-2.2.2@global/bi
5 /Users/username/.rvm/rubies/ruby-2.2.2/bin
6 /usr/local/bin
7 /usr/bin
8 /bin
9 /usr/sbin
10 /sbin
11 /opt/X11/bin
12 .git/safe/../../bin
13 /Users/username/.bin
14 /usr/local/sbin
15 /Users/username/.rvm/gems/ruby-2.2.2/bin
16 /Users/username/.rvm/gems/ruby-2.2.2@global/b
17 /Users/username/.rvm/rubies/ruby-2.2.2/bin
18 /Users/username/.rvm/bin
19 /Users/username/.rvm/bin
20 /Users/username/Dropbox/Developer/gocode/bin
```

You can alias this command if you use it often:

```sh
alias print-path=`echo $PATH | awk '{ n = split($0, paths, ":"); for (i=0; ++i <= n;) print i, paths[i] }'`
```

You may want to check out another rocketeer's (Josh Branchaud) solution to this problem, written in Rust: https://github.com/jbranchaud/ppp

[source](https://til.hashrocket.com/posts/db8289acbb-using-awk-to-debug-path)
