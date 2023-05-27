# tmux scratchpad

The plugin provides a shell script to either create a popup window if a session
doesn't exist or switch to the session if it does exist. Requires tmux version
3.2 or greater.

## Installation

In your `.tmux.conf`, add the following to install the plugin

```
set -g @plugin 'dtpike/tmux-scratchpad'
```
Then install all plugins (`prefix + I`).

## Config

The plugin doesn't automatically set a key binding to use the scratchpad.
Choose an unused key binding and set it to run the `toggle` command. This is
installed with the plugin in the scripts directory.

For example, add the following to bind `prefix + p` to toggle the scratchpad:

```
bind-key p run $TMUX_PLUGIN_MANAGER_PATH/tmux-scratchpad/scripts/toggle
```

Reload your tmux environment after setting up the key binding.



