
# USB device on WSL2

Following:
- https://learn.microsoft.com/en-us/windows/wsl/connect-usb
- https://superuser.com/questions/1686414/e-unable-to-locate-package-linux-tools-5-4-0-77-generic-on-wsl-debian-11

In the commands below <param-name/example>

## Installation
On Windows install usbipd (PowerShell admin)
```
winget install --interactive --exact dorssel.usbipd-win
```
In WSL2
```
sudo apt install usbip hwdata usbutils
```

## Usage
Windows
```
usbipd wsl list
usbipd bind --busid <BUDID/9-1>
# Stop
usbipd unbind --busid <BUSID/9-1>
```
WSL2
```
sudo usbip attach -r $HOSTNAME.local -b <BUSID/9-1>

# Stop
sudo usbip port
sudo usbip detach -p <Port xx/00>
```