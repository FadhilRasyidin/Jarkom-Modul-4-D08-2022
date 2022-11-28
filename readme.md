## Anggota Kelompok

- Mohammad Fadhil Rasyidin Parinduri // 5025201131
- Marcelino Salim // 5025201026
- Aisyah Nurhalimah // 5025201081 

### Soal Shift

- [link](https://docs.google.com/document/d/1a_ITp6WYIqoJFXA2oL1jkox9AzqYGxicjr2LGPBsqBE/edit?usp=sharing)

Kendala:

1. banyak tugas sedikit waktu (butuh introspeksi diri untuk memperbaiki manajemen waktu)
2. hehe

 ## Topologi
 ![soal shift 4 1](https://user-images.githubusercontent.com/73109893/203557069-d6c56215-1f3e-4103-8b24-a9934e1fbcb8.png)

 # CPT - VLSM
  ### Pembagian Subnet
  ![jarkom modul 4 vlsm](https://user-images.githubusercontent.com/73109893/203556279-84193c96-a612-477b-938c-e48f6bae89af.png)

  ### Perhitungan subnet
  <img width="183" alt="image" src="https://user-images.githubusercontent.com/73109893/203556405-eb786e6a-7510-49f2-b771-49eecad16077.png">

  ### VLSM Tree
  ![VLSM Tree](https://user-images.githubusercontent.com/73109893/203556653-f56c19d3-b2c9-4077-9a4d-6714488d0301.png)

  ### Pembagian IP
  ![messageImage_1669205970740](https://user-images.githubusercontent.com/73109893/203556754-e23763d2-ccb3-42a9-ab54-a65fecb3814a.jpg)

  ### Routing
  #### Subnet

# GNS3 - CIDR
## Konfigurasi Node di GNS3
- **The Minister**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.136.2
    netmask 255.255.255.252
    gateway 10.19.136.1

    auto eth1
    iface eth1 inet static
    address 10.19.133.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 10.19.128.1
    netmask 255.255.252.0
    ```

- **The Dauntless**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.133.2
    netmask 255.255.255.252
    gateway 10.19.133.1

    auto eth1
    iface eth1 inet static
    address 10.19.132.1
    netmask 255.255.255.0
    ``` 

- **The Order**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.160.2
    netmask 255.255.255.252
    gateway 10.19.160.1

    auto eth1
    iface eth1 inet static
    address 10.19.136.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 10.19.144.1
    netmask 255.255.255.192
    ``` 

- **The Instrument**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.32.2
    netmask 255.255.255.252
    gateway 10.19.32.1

    auto eth1
    iface eth1 inet static
    address 10.19.17.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 10.19.4.1
    netmask 255.255.255.252

    auto eth3
    iface eth3 inet static
    address 10.19.8.1
    netmask 255.255.255.128
    ``` 

- **The Perfomance**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet dhcp

    auto eth1
    iface eth1 inet static
    address 10.19.68.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 10.19.66.1
    netmask 255.255.255.252

    auto eth3
    iface eth3 inet static
    address 10.19.32.1
    netmask 255.255.255.252

    auto eth4
    iface eth4 inet static
    address 10.19.160.1
    netmask 255.255.255.252
    ``` 

- **The Firefist**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.4.2
    netmask 255.255.255.252
    gateway 10.19.4.1

    auto eth1
    iface eth1 inet static
    address 10.19.2.1
    netmask 255.255.254.0

    auto eth2
    iface eth2 inet static
    address 10.19.0.1
    netmask 255.255.255.0
    ```

- **The Queen**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.0.2
    netmask 255.255.255.0
    gateway 10.19.0.1

    auto eth1
    iface eth1 inet static
    address 10.19.1.1
    netmask 255.255.255.252
    ```

- **The Magical**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.66.2
    netmask 255.255.255.252
    gateway 10.19.66.1

    auto eth1
    iface eth1 inet static
    address 10.19.64.1
    netmask 255.255.254.0
    ```

- **The Profound**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 10.19.17.2
    netmask 255.255.255.252
    gateway 10.19.17.1

    auto eth1
    iface eth1 inet static
    address 10.19.16.1
    netmask 255.255.255.128

    auto eth2
    iface eth2 inet static
    address 10.19.16.129
    netmask 255.255.255.128
    ```

- **Haines**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.64.2
    netmask 255.255.254.0
    gateway 10.19.64.1
    ```

- **Corveks**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.64.3
    netmask 255.255.254.0
    gateway 10.19.64.1
    ```

- **The Beast**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.68.2
    netmask 255.255.255.252
    gateway 10.19.68.1
    ```

- **Ashaf**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.144.2
    netmask 255.255.255.192
    gateway 10.19.144.1
    ```

- **Guidessau**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.128.2
    netmask 255.255.252.0
    gateway 10.19.128.1
    ```

- **Johan**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.132.3
    netmask 255.255.255.0
    gateway 10.19.132.1
    ```

- **Phanora**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.132.2
    netmask 255.255.255.0
    gateway 10.19.132.1
    ```

- **Matt Cugat**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.8.2
    netmask 255.255.255.128
    gateway 10.19.8.1
    ```

- **Helga**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.16.130
    netmask 255.255.255.128
    gateway 10.19.16.129
    ```

- **Spendrow**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.16.2
    netmask 255.255.255.128
    gateway 10.19.16.1
    ```

- **Oakleave**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.2.2
    netmask 255.255.254.0
    gateway 10.19.2.1
    ```

- **Keith**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.0.3
    netmask 255.255.255.0
    gateway 10.19.0.1
    ```

- **The Witch**
    ```
    auto eth0
    iface eth0 inet static
    address 10.19.1.2
    netmask 255.255.255.252
    gateway 10.19.1.1
    ```







## Routing pada GNS3   
- **The Minister**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.136.1

    route add -net 10.19.132.0 netmask 255.255.255.0 gw 10.19.133.2
    ```

- **The Dauntless**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.133.1
    ``` 

- **The Order**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.160.1

    route add -net 10.19.128.0 netmask 255.255.252.0 gw 10.19.136.2
    route add -net 10.19.133.0 netmask 255.255.255.252 gw 10.19.136.2
    route add -net 10.19.132.0 netmask 255.255.255.0 gw 10.19.136.2
    ``` 

- **The Instrument**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.32.1

    route add -net 10.19.16.0 netmask 255.255.255.128 gw 10.19.17.2
    route add -net 10.19.16.128 netmask 255.255.255.128 gw 10.19.17.2

    route add -net 10.19.2.0 netmask 255.255.254.0 gw 10.19.4.2
    route add -net 10.19.0.0 netmask 255.255.255.0 gw 10.19.4.2
    route add -net 10.19.1.0 netmask 255.255.255.252 gw 10.19.4.2
    ``` 

- **The Perfomance**
    ```
    route add -net 10.19.144.0 netmask 255.255.255.192 gw 10.19.160.2
    route add -net 10.19.136.0 netmask 255.255.255.252 gw 192.178.160.2
    route add -net 10.19.128.0 netmask 255.255.252.0 gw 192.178.160.2
    route add -net 10.19.133.0 netmask 255.255.255.252 gw 192.178.160.2
    route add -net 10.19.132.0 netmask 255.255.255.0 gw 192.178.160.2

    route add -net 10.19.64.0 netmask 255.255.254.0 gw 192.178.66.2

    route add -net 10.19.8.0 netmask 255.255.255.128 gw 10.19.32.2
    route add -net 10.19.17.0 netmask 255.255.255.252 gw 10.19.32.2
    route add -net 10.19.16.0 netmask 255.255.255.128 gw 10.19.32.2
    route add -net 10.19.16.128 netmask 255.255.255.128 gw 10.19.32.2
    route add -net 10.19.4.0 netmask 255.255.255.252 gw 10.19.32.2
    route add -net 10.19.2.0 netmask 255.255.254.0 gw 10.19.32.2
    route add -net 10.19.0.0 netmask 255.255.255.0 gw 10.19.32.2
    route add -net 10.19.1.0 netmask 255.255.255.252 gw 10.19.32.2
    ``` 

- **The Firefist**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.4.1

    route add -net 10.19.1.0 netmask 255.255.255.252 gw 10.19.0.2
    ```

- **The Queen**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.0.1
    ```

- **The Magical**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.66.1
    ```

- **The Profound**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.19.17.1
    ```

