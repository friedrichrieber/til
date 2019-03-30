# Custom Battery Prompt

After i installed the i3 window manager i no longer had a low battery prompt, which resulted in my laptop just suddenly turning.

I wanted to write a script which used my application selectors ```rofi``` message function. 

I found a fitting script on stackoverflow which i modiefied to use rofi.

```
#!/bin/bash
while true
do
    battery_level=`acpi -b | grep -P -o '[0-9]+(?=%)'`
    if [ $battery_level -le 30 ]; then
       	rofi -e  "Battery is lower 30%!"
    elif [ $battery_level -le 20 ]; then
 	rofi -e "Battery is lower than 20%!"
    elif [ $battery_level -le 10]; then 
	rofi -e "Battery is lower than %10!"
    fi
    sleep 300 # 300 seconds or 5 minutes
done
```

After that i put this line
```
sh /home/f/skripte/battery_status.sh &
```
into ```/etc/rc.local```. And rebooted

[Stackoverflow Source](https://askubuntu.com/questions/518928/how-to-write-a-script-to-listen-to-battery-status-and-alert-me-when-its-above)


