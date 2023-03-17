# lshidraw

`lshidraw` is a command-line tool that lists the available HID (Human Interface Device) devices in the system, along with their corresponding HIDRAW devices. It is written in bash.

## Usage

```
lshidraw [-h] [-v] [-j] [-V]
```

### Options

* `-h`: Show the help message and exit.
* `-v`: Show more information, including the VID (Vendor ID) and PID (Product ID) of each device, as well as the driver that is used to handle the device.
* `-j`: Output the information in JSON format.
* `-V`: Show the version of the `lshidraw` tool.

## Example Output
```
$ lshidraw
hidraw0 USB OPTICAL MOUSE
hidraw1 USB OPTICAL MOUSE
hidraw2 SYNA30A6:00 06CB:CDEC
```

```
$ lshidraw -v
HIDRAW  	 VID 	 PID 	 DRIVER               DEVICE
hidraw0 	 18F8 	 0F99 	 hid-generic          USB OPTICAL MOUSE 
hidraw1 	 18F8 	 0F99 	 hid-generic          USB OPTICAL MOUSE 
hidraw2 	 06CB 	 CDEC 	 hid-multitouch       SYNA30A6:00 06CB:CDEC
```

## License

`lshidraw` is distributed under the terms of the MIT license.