## Installing Arch Linux _(no encryption)_

### Connect to the wifi...

```shell
iwctl --passphrase <<passphrase>> station wlan0 connect <<network name>>
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
