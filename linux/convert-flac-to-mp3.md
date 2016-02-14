# Convert FLAC to mp3

Make sure flac and lame is installed:

```
sudo apt-get install flac
sudo apt-get install lame
```

Then in the folder with all the .flac files:

`for f in *.flac; do flac -cd "$f" | lame -b 320 - "${f%.*}".mp3; done`

[source](http://www.boback.com/2013/how-to-convert-flac-to-mp3-ubuntu-command-line/)
