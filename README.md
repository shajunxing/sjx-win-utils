# Some windows command-line utilities

## Send Alt-Enter to current console to toggle fullscreen.

`alt-enter`

## Clear as much memory as possible.

`memmaker`

If whole system needs to be cleanup, right click it and select "Run as administrator", or use `uac` to run it.

## Show seletable menu.

`menu <menuitem> [menuitem] [menuitem] ...`

Up/Down to select, Enter to confirm, ESC to cancel. Return code is number of menu rows you selected, starting from 1, or 0 if canceled, or -1 in case of error.

## Run with elevated permissions by poping up UAC dialog.

`uac [--file=...] [--parameters=...] [--directory=...]`

## Create windows process, wait for it's window appears.

`winwait [--application-name=...] [--command-line=...] [--current-directory=...] [--class-name=...] [--window-name=...]`

`--window-name` supports wildcards.

If `--class-name=` or `--window-name` exists, program will search for top window corresponding to these information. Or will search using process id.

