## Installing Arch Linux _(no encryption)_

### Connect to the wifi...

```shell
iwctl station wlan0 connect <<network name>>
```

### Download and execute bootstrap script

```shell
curl -LO https://github.com/chfourie/bootstrap/raw/master/arch/noencrypt  
chmod +x ./noencrypt  
./noencrypt
```

If you are actively working on the script, you might need to run curl as follows...

```shell
curl -LO -H 'Cache-Control: no-cache, no-store' https://github.com/chfourie/bootstrap/raw/master/arch/noencrypt  
```
### After first reboot

```shell
sudo modprobe ppp_generic
# Rather use the applet so that we don't have to enter our password on the console
# sudo nmcli device wifi connect <<network name>> password <<PASSWORD>>
nm-applet
```
