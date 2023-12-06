# Jarkom-Modul-4-D13-2023
<table>
<tbody>
  <thead>
    <tr>
      <th>Name</th>
      <th>NRP</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Thalent Athalla Razzaq</td>
      <td>5025211101</td>
    </tr>
    <tr>
      <td> Jawahirul Wildan </td>
      <td> 5025211150 </td>
  </tbody>
</table>
Soal Dapat diakses pada [disini](https://docs.google.com/document/d/1PFDIgt5fC4PMmUaDKxw9ZEgwzpzgFv0xvo3K7PRkj10/edit?usp=sharing)

## Topologi
![topologi](images/topologi_modul4.png)

### Perhitunngan IP
[!subnet_ip](images/subnet-ip.jpg)
Setelah dihitung jumlah IP dari subnet-subnet di atas, didapat tabel berikut
Subnet | Jumlah IP | Netmask
:---: | :---: | :---:
A1|2|/30
A2|25|/27
A3|2|/30
A4|2|/30
A5|1023|/21
A6|1001|/22
A7|2|/30
A8|6|/29
A9|2|/30
A10|3|/29
A11|2|/30
A12|2|/30
A13|1001|/22
A14|251|/24
A15|2|/30
A16|255|/23
A17|2|/30
A18|31|/26
A19|512|/22
A20|2|/30
A21|127|/24
Total|4255|/19

## VLSM - GNS
### Penentuan Network ID, Netmask dan Broadcast Address
Berikut pohon subnet yang dibentuk sesuai dengan penggabungan subnet sebelumnya
![vlsm-tree](images/vlsm-tree.png)

Didapat tabel data setiap subnet, yakni NID dan Netmask. Lalu Broadcast address dapat dicari dengan menggunakan operasi OR pada IP dan Inverted Netmask
Subnet | Network ID | Netmask | Broadcast
:---: | :---: | :---: | :---:
A1|10.28.7.8|255.255.255.252|10.28.7.11 
A2|10.28.7.160|255.255.255.224|10.28.7.191 
A3|10.28.7.12|255.255.255.252|10.28.7.15
A4|10.28.7.16|255.255.255.252|10.28.7.19 
A5|10.28.24.0|255.255.248.0|10.28.31.255 
A6|10.28.12.0|255.255.252.0|10.28.15.255
A7|10.28.7.20|255.255.255.252|10.28.7.23
A8|10.28.7.144|255.255.255.248|10.28.7.151 
A9|10.28.7.24|255.255.255.252|10.28.7.27
A10|10.28.7.152|255.255.255.248|10.28.7.159
A11|10.28.7.28|255.255.255.252|10.28.7.31
A12|10.28.7.128|255.255.255.252|10.28.7.131
A13|10.28.16.0|255.255.252.0|10.28.19.255 
A14|10.28.8.0|255.255.255.0|10.28.8.255
A15|10.28.7.132|255.255.255.252|10.28.7.135
A16|10.28.10.0|255.255.254.0|10.28.11.255 
A17|10.28.7.136|255.255.255.252|10.28.7.139
A18|10.28.7.192|255.255.255.192|10.28.7.255
A19|10.28.20.0|255.255.252.0|10.28.23.255
A20|10.28.7.140|255.255.255.252|10.28.7.143
A21|10.28.9.0|255.255.255.0|10.28.9.255 
### Subnetting

### Routing

## CIDR - CPT
### Penggabungan Subnet
Berikut penggabungan subnet dengan metode CIDR
![cidr-subnet](images/cidr-b.jpg)
![cidr-subnet](images/cidr-c.jpg)
![cidr-subnet](images/cidr-d.jpg)
![cidr-subnet](images/cidr-e.jpg)
![cidr-subnet](images/cidr-f.jpg)
![cidr-subnet](images/cidr-g.jpg)
![cidr-subnet](images/cidr-h.jpg)
![cidr-subnet](images/cidr-i.jpg)


### Penentuan Network ID, Netmask dan Broadcast Address
Berikut pohon subnet yang dibentuk sesuai dengan penggabungan subnet sebelumnya
![cidr-tree](images/cidr-tree.jpg)

Didapat tabel data setiap subnet, yakni NID dan Netmask. Lalu Broadcast address dapat dicari dengan menggunakan operasi OR pada IP dan Inverted Netmask

Subnet | Network ID | Netmask | Broadcast
:---: | :---: | :---: | :---:
A1|10.28.192.0|255.255.255.252|10.28.192.3
A2|10.28.160.0|255.255.255.224|10.28.160.31
A3|10.28.136.0|255.255.255.252|10.28.136.3
A4|10.28.152.0|255.255.255.252|10.28.152.3
A5|10.28.144.0|255.255.248.0|10.28.151.255
A6|10.28.132.0|255.255.252.0|10.28.135.255
A7|10.28.128.8|255.255.255.252|10.28.128.11
A8|10.28.128.0|255.255.255.248|10.28.128.7
A9|10.28.32.0|255.255.255.252|10.28.32.3
A10|10.28.24.0|255.255.255.248|10.28.24.7
A11|10.28.24.8|255.255.255.252|10.28.24.11
A12|10.28.21.0|255.255.255.252|10.28.21.3
A13|10.28.16.0|255.255.252.0|10.28.19.255
A14|10.28.20.0|255.255.255.0|10.28.20.255
A15|10.28.8.0|255.255.255.252|10.28.8.3
A16|10.28.2.0|255.255.254.0|10.28.3.255
A17|10.28.0.64|255.255.255.252|10.28.0.67
A18|10.28.0.0|255.255.255.192|10.28.0.63
A19|10.28.4.0|255.255.252.0|10.28.7.255
A20|10.28.65.0|255.255.255.252|10.28.65.3
A21|10.28.64.0|255.255.255.0|10.28.64.255

### Topologi CPT

![cidr-cpt](images/topologi-cpt.png)

### Subnetting
Setelah dihitung ip untuk tiap subnet, maka sekarang saatnya mengatur ip pada tiap router, client dan server. Setiap interface node diatur sesuai ip yang telah dihitung melalui GUI aplikasi.

#### Aura
```
FastEthernet0/0
FastEthernet0/1
FastEthernet1/0
FastEthernet1/1
```
### Routing
Setelah pengaturan IP selesai, dilanjutkan dengan routing pada router-router seperti berikut.
