# Jarkom-Modul-5-E22-2023

| Nama                       | NRP        |
| ---------------------------| -----------|
| Anggara Saputra            | 5025211241 |
| Faizah Nurdianti Maghfirah | 5025211134 |

## SUBNET
![image](https://github.com/fzhmghfrh/Jarkom-Modul-5-E22-2023/blob/main/img/subnet.png)
## TREE
![image](https://github.com/fzhmghfrh/Jarkom-Modul-5-E22-2023/blob/main/img/tree.png)
## CONFIG

### Aura
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
address 192.217.0.1
netmask 255.255.255.252

auto eth2
iface eth2 inet static
address 192.217.0.5
netmask 255.255.255.252
```

### Heiter
```
auto eth0
iface eth0 inet static
	address 192.217.0.2
	netmask 255.255.255.252
	gateway 192.217.0.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1
iface eth1 inet static
	address 192.217.8.1
	netmask 255.255.248.0

auto eth2
iface eth2 inet static
	address 192.217.4.1
	netmask 255.255.252.0
```

### TurkRegion
```
auto eth0
iface eth0 inet static
	address 192.217.8.2
	netmask 255.255.248.0
	gateway 192.217.8.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Sein
```
auto eth0
iface eth0 inet static
	address 192.217.4.2
	netmask 255.255.252.0
	gateway 192.217.4.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### GrobeForest
```
auto eth0
iface eth0 inet static
	address 192.217.4.3
	netmask 255.255.252.0
	gateway 192.217.4.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Frieren
```
auto eth0
iface eth0 inet static
	address 192.217.0.6
	netmask 255.255.255.252
	gateway 192.217.0.5
	up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1
iface eth1 inet static
	address 192.217.0.9
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 192.217.0.13
	netmask 255.255.255.252
```

### Stark
```
auto eth0
iface eth0 inet static
	address 192.217.0.10
	netmask 255.255.255.252
	gateway 192.217.0.9
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Himmel
```
auto eth0
iface eth0 inet static
	address 192.217.0.14
	netmask 255.255.255.252
	gateway 192.217.0.13
	up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1
iface eth1 inet static
	address 192.217.2.1
	netmask 255.255.254.0

auto eth2
iface eth2 inet static
	address 192.217.0.129
	netmask 255.255.255.128
```

### LaubHills
```
auto eth0
iface eth0 inet static
	address 192.217.2.2
	netmask 255.255.254.0
	gateway 192.217.2.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### SchwerMountain
```
auto eth0
iface eth0 inet static
	address 192.217.0.131
	netmask 255.255.255.128
	gateway 192.217.0.129
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Fern
```
auto eth0
iface eth0 inet static
	address 192.217.0.130
	netmask 255.255.255.128
	gateway 192.217.0.129
	up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1
iface eth1 inet static
	address 192.217.0.17
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 192.217.0.21
	netmask 255.255.255.252
```

### Richter
```
auto eth0
iface eth0 inet static
	address 192.217.0.18
	netmask 255.255.255.252
	gateway 192.217.0.17
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Revolte
```
auto eth0
iface eth0 inet static
	address 192.217.0.22
	netmask 255.255.255.252
	gateway 192.217.0.21
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

## ROUTING
### Aura
```
route add -net 192.217.8.0 netmask 255.255.248.0 gw 192.217.0.2
route add -net 192.217.4.0 netmask 255.255.252.0 gw 192.217.0.2

route add -net 192.217.0.8 netmask 255.255.255.252 gw 192.217.0.6
route add -net 192.217.0.12 netmask 255.255.255.252 gw 192.217.0.6
route add -net 192.217.2.0 netmask 255.255.254.0 gw 192.217.0.6
route add -net 192.217.0.128 netmask 255.255.255.128 gw 192.217.0.6
route add -net 192.217.0.16 netmask 255.255.255.252 gw 192.217.0.6
route add -net 192.217.0.20 netmask 255.255.255.252 gw 192.217.0.6
```

### Heiter
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.1
```

### Frieren
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.5
route add -net 192.217.2.0 netmask 255.255.254.0 gw 192.217.0.14
route add -net 192.217.0.128 netmask 255.255.255.128 gw 192.217.0.14
route add -net 192.217.0.16 netmask 255.255.255.252 gw 192.217.0.14
route add -net 192.217.0.20 netmask 255.255.255.252 gw 192.217.0.14
```

### Himmel
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.13
route add -net 192.217.0.16 netmask 255.255.255.252 gw 192.217.0.130
route add -net 192.217.0.20 netmask 255.255.255.252 gw 192.217.0.130
```

### Fern
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.129
```

## DHCP
### DNS Server (Richter)
```
apt update
apt install bind9 -y
echo '
options {
        directory "/var/cache/bind";
        forwarders {
                192.168.122.1;	// IP NAT
        };
        allow-query { any; };
        auth-nxdomain no;    # conform to RFC1035
        listen-on-v6 { any; };
}; 
' > /etc/bind/named.conf.options
service bind9 restart
```

### DHCP Server (Revolte)
```
apt update
apt install isc-dhcp-server -y
echo '
INTERFACES="eth0"
' > /etc/default/isc-dhcp-server

echo '
# Revolte subnet A10
subnet 192.217.0.20 netmask 255.255.255.252 {
}

# TurkRegion subnet A2
subnet 192.217.8.0 netmask 255.255.248.0 {
range 192.217.8.2 192.217.15.254;
option routers 192.217.8.1;
option broadcast-address 192.217.15.255;
option domain-name-servers 192.217.0.18;
}

# GrobeForest subnet A3
subnet 192.217.4.0 netmask 255.255.252.0 {
range 192.217.4.3 192.217.7.254;
option routers 192.217.4.1;
option broadcast-address 192.217.7.255;
option domain-name-servers 192.217.0.18;
}

#  LaubHills subnet A7
subnet 192.217.2.0 netmask 255.255.254.0 {
range 192.217.2.2 192.217.3.254;
option routers 192.217.2.1;
option broadcast-address 192.217.3.255;
option domain-name-servers 192.217.0.18;
}

#  SchwerMountain subnet A8
subnet 192.217.0.128 netmask 255.255.255.128 {
range 192.217.0.131 192.217.0.254;
option routers 192.217.0.129;
option broadcast-address 192.217.0.255;
option domain-name-servers 192.217.0.18;
}
' > /etc/dhcp/dhcpd.conf

rm /var/run/dhcpd.pid
service isc-dhcp-server start
```

### DHCP Relay (Heiter, Frieren, Fern, Himmel)
```
apt update
apt install isc-dhcp-relay -y

echo '
SERVERS="192.217.0.22"
INTERFACES="eth0 eth1 eth2 eth3"
OPTIONS=""
' > /etc/default/isc-dhcp-relay

service isc-dhcp-relay restart
```

## Nomor 1
Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi Aura menggunakan iptables, tetapi tidak ingin menggunakan MASQUERADE.
* Aura
  
Ubah configuration Aura
```
auto eth0
iface eth0 inet static
        address 192.168.122.2
        netmask 255.255.255.252
        gateway 192.168.122.1
        up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
```
iptables -t nat -A POSTROUTING -o eth0 -j SNAT -s 192.217.0.0/20 --to-source 192.168.122.2
```

## Nomor 2
Kalian diminta untuk melakukan drop semua TCP dan UDP kecuali port 8080 pada TCP.
* Client (GrobeForest)
```
apt-get update
apt install netcat -y

iptables -A INPUT -p tcp --dport 8080 -j ACCEPT
iptables -A INPUT -p tcp -j DROP
iptables -A INPUT -p udp -j DROP
```
* Client (selain GrobeForest)
```
apt-get update
apt install netcat -y
```
#### Testing
Netcat ke GrobeForest
  * Receiver (
    ```
    nc -l -p 8081
    nc -u -l -p 8080
    nc -l -p 8080
    ```
  * Sender
    ```
    nc [IP Receiver] 8081
    nc -u [IP Receiver] 8080
    nc [IP Receiver] 8080
    ```
## Nomor 3
Kepala Suku North Area meminta kalian untuk membatasi DHCP dan DNS Server hanya dapat dilakukan ping oleh maksimal 3 device secara bersamaan, selebihnya akan di drop
* DNS Server (Richter),  DHCP Server (Revolte)
```
iptables -I INPUT -p icmp -m connlimit --connlimit-above 3 --connlimit-mask 0 -j DROP
iptables -I INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
```
#### Testing
Ping DNS Richter atau Revolte di empat client bersamaan
```
ping 192.217.0.18
ping 192.217.0.22
```
## Nomor 4
Lakukan pembatasan sehingga koneksi SSH pada Web Server hanya dapat dilakukan oleh masyarakat yang berada pada GrobeForest
* WebServer
```
apt install netcat -y

iptables -A INPUT -p tcp --dport 22 -s  192.217.4.4/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 22 -m iprange --src-range 192.217.4.3-192.217.7.254 -j ACCEPT
iptables -A INPUT -p tcp --dport 22 -j DROP
```
#### Testing
Netcat webserver di client GrobeForest dan selain GrobeForest
* Web Server
  ```
  nc -l -p 22
  ```
* Client
  ```
  nc 192.217.4.2
  nc 192.217.0.10
  ```
## Nomor 5
Selain itu, akses menuju WebServer hanya diperbolehkan saat jam kerja yaitu Senin-Jumat pada pukul 08.00-16.00.
* WebServer
```
iptables -A INPUT -m time --timestart 16:01 --timestop 23:59 --weekdays Mon,Tue,Wed,Thu,Fri -j REJECT
iptables -A INPUT -m time --timestart 00:00 --timestop 07:59 --weekdays Mon,Tue,Wed,Thu,Fri -j REJECT
iptables -A INPUT -m time --weekdays Sat,Sun -j REJECT
```
#### Testing
* Pada jam kerja
```
date --set="2023-12-19 09:00:00"
```
* Di luar jam kerja
```
date --set="2023-12-19 21:00:00"
```
* Di luar hari kerja
```
date --set="2023-12-16 09:00:00"
```
## Nomor 6
Lalu, karena ternyata terdapat beberapa waktu di mana network administrator dari WebServer tidak bisa stand by, sehingga perlu ditambahkan rule bahwa akses pada hari Senin - Kamis pada jam 12.00 - 13.00 dilarang (istirahat maksi cuy) dan akses di hari Jumat pada jam 11.00 - 13.00 juga dilarang (maklum, Jumatan rek).
* WebServer
```
iptables -A INPUT -m time --timestart 12:00 --timestop 13:00 --weekdays Mon,Tue,Wed,Thu -j REJECT
iptables -A INPUT -m time --timestart 11:00 --timestop 13:00 --weekdays Fri -j REJECT
```
#### Testing
* Pada jam istirahat
  ```
  date --set="2023-12-19 12:30:00"
  ```
* Pada jam istirahat hari Jumat
  ```
  date --set="2023-12-22 11:30:00"
  ```
## Nomor 7
Karena terdapat 2 WebServer, kalian diminta agar setiap client yang mengakses Sein dengan Port 80 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan dan request dari client yang mengakses Stark dengan port 443 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan.
## Nomor 8
Karena berbeda koalisi politik, maka subnet dengan masyarakat yang berada pada Revolte dilarang keras mengakses WebServer hingga masa pencoblosan pemilu kepala suku 2024 berakhir. Masa pemilu (hingga pemungutan dan penghitungan suara selesai) kepala suku bersamaan dengan masa pemilu Presiden dan Wakil Presiden Indonesia 2024.
* Webserver
```
iptables -A INPUT -s 192.217.0.22/30 -m time --datestart 2023-12-10 --datestop 2024-02-15 -j REJECT
```
* Revolte
```
apt install netcat -y
```
### Testing
* Revolte sebelum pemilu
  ```
  date --set="2023-12-19 10:00:00"
  ```
* Revolte setelah pemilu
  ```
  date --set="2024-2-15 10:00:00"
  ```
## Nomor 9
Sadar akan adanya potensial saling serang antar kubu politik, maka WebServer harus dapat secara otomatis memblokir  alamat IP yang melakukan scanning port dalam jumlah banyak (maksimal 20 scan port) di dalam selang waktu 10 menit. 
(clue: test dengan nmap)
### Webserver
```
iptables -N portscan

iptables -A INPUT -m recent --name portscan --update --seconds 600 --hitcount 20 -j DROP
iptables -A FORWARD -m recent --name portscan --update --seconds 600 --hitcount 20 -j DROP

iptables -A INPUT -m recent --name portscan --set -j ACCEPT
iptables -A FORWARD -m recent --name portscan --set -j ACCEPT
```
#### Testing
Ping Webserver lebih dari 20 kali
```
ping 192.217.4.2 -c 27
ping 192.217.0.10 -c 27
```

## Nomor 10
Karena kepala suku ingin tau paket apa saja yang di-drop, maka di setiap node server dan router ditambahkan logging paket yang di-drop dengan standard syslog level. 
