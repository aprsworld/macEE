# macEE

## Setting MAC address in /etc/network/interfaces

Setting the MAC address on an up or down interface doesn't work. Doing it
while bringing the interface down, prior to bringing it up, does work.

```
iface eth0 inet dhcp
        pre-up ifconfig eth0 down hw ether `/home/aprs/getMAC`
```
