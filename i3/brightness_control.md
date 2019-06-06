# Brightnes Control

After installing i3-wm i could not use the my keyboard buttons to control the brightness of the laptop screen. 

The first google result is not working on my Ubuntu 19.04 machine but did work on my Ubuntu 18.04 machine 

```
# (not working on ubuntu 19.04!)
bindsym XF86MonBrightnessUp exec xbacklight -inc 20 # increase screen brightness
bindsym XF86MonBrightnessDown exec xbacklight -dec 20 # decrease screen brightness
```

I found out that it has something to do with a driver switch to something called modesetting drivers. (see the comment by Hans de Goede [here](https://bugzilla.redhat.com/show_bug.cgi?id=1354662)). In this command a tool with the name ```brightnessctl``` is mentioned which can change the brightness on my machine. Only propblem is that it by default needs root permission which means that i cant use in my i3 config file. There is a workaround for this which have not understood yet [brightnessctl github page](https://github.com/Hummer12007/brightnessctl). 

So for now i am manually entering something like this in my terminal: 

```
sudo brightnessctl set 50%
```
