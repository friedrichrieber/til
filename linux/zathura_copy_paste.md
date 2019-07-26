# Zathura Copy Paste

On newer version just put this 

```bash
# to enable copy paste
URxvt.keysym.Shift-Control-V: eval:paste_clipboard
URxvt.keysym.Shift-Control-C: eval:selection_to_clipboard
# to disable keycap insert mode (which interferes with copy and paste)
URxvt.iso14755: false
URxvt.iso14755_52: false
```

in ```~/.Xdefaults```.

# Source 
https://unix.stackexchange.com/questions/444773/how-to-disable-the-ctrlshift-binding-iso-14755-in-urxvt
https://wiki.ubuntuusers.de/rxvt-unicode/#Copy-Paste
