# Laporan Praktikum Konsep Jaringan (Intervlan)

## Apa itu Intervlan?
Intervlan adalah proses meneruskan lalu lintas jaringan dari satu VLAN ke VLAN yang lain menggunakan router.

## Jenis Intervlan
Intervlan terbagi menjadi beberapa jenis, yaitu:
1. Traditional Intervlan
![traditional intervlan](assets/traditional.JPG)
2. Router-On-Stick (sering digunakan)
![router-on-stick](assets/router%20on%20stick.JPG)

## Konfigurasi dengan Metode Router-on-stick
### Konfigurasi IP
![config pc0](assets/config%20pc0.JPG)
![config pc1](assets/config%20pc1.JPG)
![config router](assets/config%20router.JPG)

### Konfigurasi Switch
Tambahkan vlan database (10->admin, 30->user)
![vlan database](assets/vlan%20database.JPG)

Kemudian config interfacenya
![interface](assets/config%20interface.JPG)

### Konfigurasi Router (2)
![config](assets/config%20router%202.JPG)
![config terminal](assets/config%20terminal.JPG)
