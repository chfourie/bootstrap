## Installing Arch Linux _(no encryption)_

### Connect to the wifi...

> iwctl --passphrase <<passphrase>> station wlan0 connect <<network name>>

### Download and execute bootstrap script
> curl -LO https://github.com/chfourie/bootstrap/raw/master/arch/noencrypt
> chmod +x ./noencrypt
> ./noencrypt
