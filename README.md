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

## Penggabungan Node
Kondisi Node Awal

<img width="697" alt="A CIDR" src="https://user-images.githubusercontent.com/83849481/204120060-8106faf7-d26f-4a34-a364-6f2209dc8ab5.png">

| **Subnet** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | --------- |
| A1 | 1001 | 22 | 
| A2 | 251 | 24 |
| A3 | 2 | 30 |
| A4 | 2 | 30 | 
| A5 | 51 | 26 |
| A6 | 2 | 30 |
| A7 | 121 | 25 | 
| A8 | 211 | 24 |
| A9 | 501 | 23 |
| A10| 2 | 30 | 
| A11| 71 | 25 |
| A12| 121 | 25 |
| A13| 2 | 30 |
| A14| 2 | 30 | 
| A15| 2 | 30 |
| A16| 271 | 23 |
| A17| 2 | 30 | 
| A18| 2 | 30 |

Penggabungan Node Pertama yaitu B

<img width="747" alt="B CIDR" src="https://user-images.githubusercontent.com/83849481/204120074-88d2d48d-12b2-4054-9920-3fab78bd9139.png">


| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| B1 | A2, A3 | 251 | 23 |
| B2 | A18, A8 | 211 | 23 |
| B3 | A11, A12 | 121 | 24 |

Penggabungan Node Kedua yaitu C

<img width="746" alt="C CIDR" src="https://user-images.githubusercontent.com/83849481/204121755-859a0ed8-5a8d-4e16-9866-5289e7cd5e07.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| C1 | A1, B1 | 1001 | 21 |
| C2 | A9, B2 | 501 | 22 |
| C3 | A13, B3 | 121 | 23 |

Penggabungan Node Ketiga yaitu D

<img width="753" alt="D CIDR" src="https://user-images.githubusercontent.com/83849481/204121793-7eb11a55-807d-43b6-991d-2fe8fc3b748b.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| D1 | A4, C1 | 1001 | 20 |
| D2 | A10, C2 | 501 | 21 |
| D3 | A7, C3 | 121 | 22 |

Penggabungan Node Keempat yaitu E

<img width="787" alt="E CIDR" src="https://user-images.githubusercontent.com/83849481/204121895-5f87c9fe-aa3e-4d0b-a7e0-034d5a28df98.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| E1 | A5, D1 | 1001 | 19 |
| E2 | D2, D3 | 501 | 20 |

Penggabungan Node Kelima yaitu F

<img width="794" alt="F CIDR" src="https://user-images.githubusercontent.com/83849481/204121952-5ffc0507-c731-47c0-8e1d-ced2c185a327.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| F1 | A6, E1 | 1001 | 18 |
| F2 | A14, E2 | 501 | 19 |

Penggabungan Node Keenam yaitu G

<img width="806" alt="G CIDR" src="https://user-images.githubusercontent.com/83849481/204122002-1134c3e7-97bf-4163-891c-659d8fa728a5.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| G1 | A17, F1 | 1001 | 17 |
| G2 | A15, F2 | 501 | 18 |

Penggabungan Node Ketujuh yaitu H

<img width="875" alt="H CIDR" src="https://user-images.githubusercontent.com/83849481/204122034-041b1f27-4c8e-4406-a60f-28a788eed6db.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| H1 | A16, G2 | 501 | 17 |

Penggabungan Node Kedelapan yaitu I

<img width="840" alt="I CIDR" src="https://user-images.githubusercontent.com/83849481/204122054-6f3720bc-5baf-4f76-9644-235ac3733761.png">

| **Subnet** | **Alias** | **Jumlah IP** | **Netmask** | 
| ------------- | ------------- | ------------- | --------- |
| I1 | H1, G1 | 1001 | 16 |

## Sehingga dihasilkan tree sebagai berikut


# VLSM
Perhitungan IP

