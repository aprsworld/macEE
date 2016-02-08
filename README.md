# macEE

## Setting MAC address in /etc/network/interfaces

```
iface eth0 inet dhcp
        pre-up ifconfig eth0 down hw ether `/home/aprs/getMAC`
```
