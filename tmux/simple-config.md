# Simple tmux config file

```
#if modified run: tmux source-file ~/.tmux.conf

#change bind-key to control-a
set-option -g prefix C-a

#turn off repeated arrow movement between panes
bind-key Up    select-pane -U
bind-key Down  select-pane -D
bind-key Left  select-pane -L
bind-key Right select-pane -R

#go to last pane
bind-key C-a last-pane

#remove delay between bind-key and command
set -s escape-time 0

# Start numbering at 1
set -g base-index 1
```
