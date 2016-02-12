# Basics

default prefix: `CTRL+B`

## PANES:

* Split pane into left and right panes: `<prefix> %`
* Split pane into top and bottom panes: `<prefix> "`


* move between panes: `<prefix> <UP/DOWN/LEFT/RIGHT ARROW>`
* move to previously active pane: `<prefix> ;`


* resize pane: `<prefix> CTRL+<UP/DOWN/LEFT/RIGHT ARROW>`


* close current pane: `<prefix> x`

* enter scroll mode: `<prefix> [`
* quit scroll mode: `q`

## WINDOWS:

* create a new window in the session: `<prefix> c`


* move between windows: `<prefix> <window number>`
* move to previous window: `<prefix> p`
* move to next window: `<prefix> n`


* close current window: `<prefix> &`

## GENERAL:

* detach from tmux session: `<prefix> d`
* list tmux session: `tmux ls`
* reattach tmux session: `tmux attach -t <session id>`
* end/kill tmux session: `tmux kill-session -t <session id>`
