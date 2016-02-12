# Set display for session over SSH

Often, for what ever reason, the display ID changes after leaving a remote tmux session. This requires exporting the new display ID in the session to display X figures.

Before reattaching to tmux session determine the current display ID:

`echo $DISPLAY`

Reattach to a tmux session and run:

`export DISPLAY=<DISPLAYID>`
