# frida-tool-configuration
$ pip install frida-tools

$ frida --version

## abd configuration 
$ sudo apt-get install adb

$ adb connect <Device_IP>

$ adb push ca.der /data/local/tmp

$ adb push frida-server /data/local/tmp


## In Android device
## You need to know the processor type of the device (Emulator or physical device). Run below command
$ adb shell

$ cd /data/local/tmp

$ mv ca.der cer-der.crt

$ chmod 777 frida

$ ./frida server

## In PC
$ frida-ps

$ frida-ps -U

# List running applications
$ frida-ps -Ua

# List installed applications
$ frida-ps -Uai

# Connect Frida to the specific device

$ frida-ps -D 0736027d1d6d3b02

## For SSl pining Bypass
$ frida -U -f <package-name> -l script.js

## for Activity bypass check
$ adb shell am start -n  Package_Name/Activity_Name

## To check the log of apk
$ adb logcat | grep -i uid
