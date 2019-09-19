# Creating Windows Install USB Sticks on Linux

To create bootable Windows USB Sticks i use the tool ```woeusb```. 

## Installation on Ubuntu

To install ```woeusb``` first add ppa repository with this line 

```
add-apt-repository ppa:tomtomtom/woeusb 
```

Then install the programm itself with this line 

```
sudo apt-get install woeusb 
```

## Usage 

There are two ways to use the the command line version. The ```--device``` Way where the USB Stick is completely **WIPED** or the ```-partition``` were you copy windows to only one partition. 

I recommend the ```--device``` option where the syntax is as follows: 

``` sudo woeusb --device /path/to/windows_10_image.iso /dev/NAME_OF_STORAGE_DEVICE```

You get the name of the storage device the ```lsblk``` command. If you dont understand the output read about how linux handles storage devices. Be careful when chossing the storage device because choosing the wrong one can end in **lost** data

## Sources 

- https://wiki.ubuntuusers.de/WoeUSB/
