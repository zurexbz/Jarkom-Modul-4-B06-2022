# Jarkom-Modul-4-B06-2022

| **No** | **NRP** | **Nama** | 
| ------------- | ------------- | --------- |
| 1 | 5025201100 | Hansen Idden | 
| 2 | 5025201109 | Mohammad Firman Fardiansyah |
| 3 | 5025201167 | William Zefanya Maranatha |

# CIDR

Menggabungkan node paling jauh dari sumber NAT dan kita cluster dengan node terdekatnya hingga menjadi satu cluster besar.

## GNS 3
![image](https://user-images.githubusercontent.com/62301187/204098538-af6deb6d-4079-4804-b26c-1aecf6421891.png)

## Network Configuration

1. Guideau
```
auto eth0
iface eth0 inet static
address 10.6.0.2
netmask 255.255.252.0
gateway 10.6.0.1
```

2. The minister 
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.8.2
netmask 255.255.255.252
gateway 10.6.8.1

auto eth1
iface eth1 inet static
address 10.6.0.1
netmask 255.255.252.0

auto eth2
iface eth2 inet static
address 10.6.5.1
netmask 255.255.255.252
```

3. The Order
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.32.2
netmask 255.255.255.252
gateway 10.6.32.1

auto eth1
iface eth1 inet static
address 10.6.16.1
netmask 255.255.255.192

auto eth2
iface eth2 inet static
address 10.6.8.1
netmask 255.255.255.252
```

4. The Dauntless
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.5.2
netmask 255.255.255.252
gateway 10.6.5.1

auto eth1
iface eth1 inet static
address 10.6.4.1
netmask 255.255.255.0
```

5. Phanora
```
auto eth0
iface eth0 inet static
address 10.6.4.2
netmask 255.255.255.0
gateway 10.6.4.1
```

6. Johan
```
auto eth0
iface eth0 inet static
address 10.6.4.3
netmask 255.255.255.0
gateway 10.6.4.1
```

7. Ashaf
```
auto eth0
iface eth0 inet static
address 10.6.16.2
netmask 255.255.255.192
gateway 10.6.16.1
```

8. The Resonance
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
address 10.6.32.1
netmask 255.255.255.252

auto eth2
iface eth2 inet static
address 10.6.144.1
netmask 255.255.255.252

auto eth3
iface eth3 inet static
address 10.6.160.1
netmask 255.255.255.252

auto eth4
iface eth4 inet static
address 10.6.64.1
netmask 255.255.255.252
```

9. The Instrument
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.144.2
netmask 255.255.255.252
gateway 10.6.144.1

auto eth1
iface eth1 inet static
address 10.6.138.1
netmask 255.255.255.128

auto eth2
iface eth2 inet static
address 10.6.132.1
netmask 255.255.255.252

auto eth3
iface eth3 inet static
address 10.6.137.1
netmask 255.255.255.252
```

10. Matt Cugat
```
auto eth0
iface eth0 inet static
address 10.6.138.2
netmask 255.255.255.128
gateway 10.6.138.1
```

11. The Firefist
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.132.2
netmask 255.255.255.252
gateway 10.6.132.1

auto eth1
iface eth1 inet static
address 10.6.130.1
netmask 255.255.255.0

auto eth2
iface eth2 inet static
address 10.6.128.1
netmask 255.255.254.0
```

12. Keith
```
auto eth0
iface eth0 inet static
address 10.6.130.2
netmask 255.255.255.0
gateway 10.6.130.1
```

13. The Queen
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.130.3
netmask 255.255.255.0
gateway 10.6.130.1

auto eth1
iface eth1 inet static
address 10.6.131.1
netmask 255.255.255.252
```

14. The Witch
```
auto eth0
iface eth0 inet static
address 10.6.131.2
netmask 255.255.255.252
gateway 10.6.131.1
```

15. Oakleave
```
auto eth0
iface eth0 inet static
address 10.6.128.2
netmask 255.255.254.0
gateway 10.6.128.1
```

16. The Profound
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.137.2
netmask 255.255.255.252
gateway 10.6.137.1

auto eth1
iface eth1 inet static
address 10.6.136.129
netmask 255.255.255.128

auto eth2
iface eth2 inet static
address 10.6.136.1
netmask 255.255.255.128
```

17. Helga
```
auto eth0
iface eth0 inet static
address 10.6.136.130
netmask 255.255.255.128
gateway 10.6.136.129
```

18. Spendrow
```
auto eth0
iface eth0 inet static
address 10.6.136.2
netmask 255.255.255.128
gateway 10.6.136.1
```

19. The Magical
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 10.6.160.2
netmask 255.255.255.252
gateway 10.6.160.1

auto eth1
iface eth1 inet static
address 10.6.192.1
netmask 255.255.254.0
```

20. Corvekt
```
auto eth0
iface eth0 inet static
address 10.6.192.2
netmask 255.255.254.0
gateway 10.6.192.1
```

21. Haines
```
auto eth0
iface eth0 inet static
address 10.6.192.3
netmask 255.255.254.0
gateway 10.6.192.1
```

22. The Beast
```
auto eth0
iface eth0 inet static
address 10.6.64.2
netmask 255.255.255.252
gateway 10.6.64.1
```

## Routing Setiap Node di GNS3

### The Minister
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.8.1
route add -net 10.6.4.0 netmask 255.255.255.0 gw 10.6.5.2

route add -net 10.6.5.0 netmask 255.255.255.252 gw 10.6.5.2
```

### The Dauntless
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.8.2
```

### The Order
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.32.1
route add -net 10.6.0.0 netmask 255.255.252.0 gw 10.6.8.2
route add -net 10.6.5.0 netmask 255.255.255.252 gw 10.6.8.2
route add -net 10.6.4.0 netmask 255.255.255.0 gw 10.6.8.2

route add -net 10.6.8.0 netmask 255.255.255.252 gw 10.6.8.2
```

### The Resonance
```
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 10.6.0.0/16

# The Order
route add -net 10.6.0.0 netmask 255.255.252.0 gw 10.6.32.2
route add -net 10.6.8.0 netmask 255.255.255.252 gw 10.6.32.2
route add -net 10.6.16.0 netmask 255.255.255.192 gw 10.6.32.2
route add -net 10.6.5.0 netmask 255.255.255.252 gw 10.6.32.2
route add -net 10.6.4.0 netmask 255.255.255.0 gw 10.6.32.2

# The Instrument 
route add -net 10.6.138.0 netmask 255.255.255.128 gw 10.6.144.2
route add -net 10.6.137.0 netmask 255.255.255.252 gw 10.6.144.2
route add -net 10.6.136.0 netmask 255.255.255.128 gw 10.6.144.2
route add -net 10.6.130.0 netmask 255.255.255.0 gw 10.6.144.2
route add -net 10.6.132.0 netmask 255.255.255.252 gw 10.6.144.2
route add -net 10.6.136.128 netmask 255.255.255.128 gw 10.6.144.2
route add -net 10.6.131.0 netmask 255.255.255.252 gw 10.6.144.2
route add -net 10.6.128.0 netmask 255.255.254.0 gw 10.6.144.2

# The Magical
route add -net 10.6.192.0 netmask 255.255.254.0 gw 10.6.160.2
```

### The Instrument
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.144.1
route add -net 10.6.130.0 netmask 255.255.255.0 gw 10.6.132.2
route add -net 10.6.131.0 netmask 255.255.255.252 gw 10.6.132.2
route add -net 10.6.128.0 netmask 255.255.254.0 gw 10.6.132.2

route add -net 10.6.132.0 netmask 255.255.255.252 gw 10.6.132.2
```

### The Firefist
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.144.2
route add -net 10.6.131.0 netmask 255.255.255.252 gw 10.6.130.3

route add -net 10.6.130.0 netmask 255.255.255.252 gw 10.6.130.3
```

### The Queen
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.132.2
```

### The Profound
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.144.2
```

### The Magical
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.6.160.1
```

# VLSM
Perhitungan IP

