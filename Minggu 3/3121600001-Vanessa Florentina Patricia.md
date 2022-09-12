# DOCUMENTATION PACKET TRACER
## Topologi
![topologi](assets/topologi.JPG)

Pada gambar di atas, terdapat 3 buah PC yang tersambung pada 1 Hub. Setiap PCnya mempunyai IP yang akan di set seperti di bawah ini.

![config pc0](assets/config-pc0.JPG)
![config pc1](assets/config-pc1.JPG)
![config pc2](assets/config-pc2.JPG)

Setelah disetting seperti di atas, lanjut ke skenario yang akan ditest.

## Scenario 1: PC0 -> PC1
Langkah pertama adalah check ARP pada PC0.

![check ARP PC 0](assets/check-arp0.JPG)

Kemudian ping IP PC1 melalui CMD PC0.

![ping](assets/ping%20pc0-1.JPG)

Maka pada simulasinya, awal pesan terbentuk berada pada layer 2.

![step 1](assets/step1.JPG)

Karena MAC IP Address Destinationnya belum ditemukan maka PC0 mengirim broadcast dengan broadcast address FFFF.FFFF.FFFF.

![arp 1](assets/arp1.JPG)![step 2](assets/step2.JPG)

Setelah mendapatkan PC dengan IP 192.168.1.2 yaitu PC1, maka isi MAC Destination yang awalnya FFFF.FFFF.FFFF diubah dengan MAC dari PC1 yang dikembalikan sebagai pesan ke PC0.

![send MAC](assets/send-MAC.JPG)

![finish](assets/finish.JPG)

## Skenario 2: PC0 -> PC1
Seperti biasa, di sini akan dicek ARP nya terlebih dahulu.

![check ARP 2](assets/check-arp1.JPG)

Karena di sini ARPnya sudah ada, maka PC0 tidak akan melakukan broadcast seperti saat pertama kali mencari MAC Destination.
Berikut isi dari paket ARP pada skenario ke-2 ini.

![arp 2](assets/arp2.JPG)

## Skenario 3: PC1 -> PC0
Sama seperti skenario di atas, hal pertama yang akan dicek adalah ARPnya.

![check ARP 3](assets/check-arp2.JPG)

Karena di sini ARPnya sudah ada, maka PC1 tidak akan melakukan broadcast seperti saat pertama kali mencari MAC Destination.
Berikut isi dari paket ARP pada skenario ke-3 ini.

![arp 3](assets/arp3.JPG)