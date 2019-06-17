# Gnome Settings in i3

Lets imagine a sitation, you installed the i3 window manager on your normal ubuntu machine which was running gnome before and you are missing the settings application. This til should solve your problem. 

To start the settings apllication from the terminal you just enter: 

```
env XDG_CURRENT_DESKTOP=GNOME gnome-control-center
```

but doing this from the terminal is not really cool/convenient, so we are going to add it to your application launcher. 

# dmenu

Dmenu ,which is the standard launcher in i3, compared to other launcher looks at your ```$PATH``` variable instead of your ```.desktop``` entries. To checko your $PATH Variable just enter ```$PATH``` in your Terminal. 

Now we have to add a little "script" at the right place with the right permissions. The script content is just the line from before and the name is whatever you want. I choosed ```settings```.

I put mine in ```~/.local/bin```. And changed the permissions with ```chmod 0777 settings``` (which is propably overkill). 

After that i reloaded i3 with ```Mod+Shift+r``` and everything worked. 


# rofi

TODO
