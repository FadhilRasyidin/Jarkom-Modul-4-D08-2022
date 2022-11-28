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
  ![Topologi VLSM](https://user-images.githubusercontent.com/90826711/204242054-e4c7c6ea-171c-461c-9a29-73fffb249afa.png)
  
  ### Perhitungan subnet
  ![Subnet](https://user-images.githubusercontent.com/90826711/204242306-cb4a6edd-79bf-437a-b69d-a3c4cf340073.jpg)

  ### VLSM Tree
  ![VLSM Tree](https://user-images.githubusercontent.com/90826711/204242329-36e55674-628e-44ef-b7f9-fd36ea3c6c4d.png)

  ### Pembagian IP
  ![VLSM Table](https://user-images.githubusercontent.com/90826711/204242388-a4584695-0be5-493e-82df-259683a3a41d.jpg)

  ### Routing
  #### Subnet
  Setelah dilakukan subnetting maka satu node dengan node lainnya akan terhubung seperti gambar
  ![CPT](https://user-images.githubusercontent.com/90826711/204238402-aea1c30c-54b4-4db5-bc22-718f68389557.png)

# GNS3 - CIDR

- **Langkah 1** Menentukan subnet yang ada dalam topologi dan lakukan labelling netmask.

![A](https://user-images.githubusercontent.com/81240334/204345658-26d781d2-675d-4773-801e-d53f97bfd57b.jpg)

- **Langkah 2** Menggabungkan subnet paling bawah di dalam topologi. Pada teknik CIDR subnet gabungan akan memiliki netmask yang 1 tingkat di atas subnet terbesar yang digabungkan.

![B](https://user-images.githubusercontent.com/81240334/204345665-58073dec-1e78-4613-9831-5554cabf6b06.jpg)
> - B1 adalah penggabungan subnet A3 dengan A4 dengan netmask /23
> - B2 adalah penggabungan subnet A8 dengan A18 dengan netmask /23

![C](https://user-images.githubusercontent.com/81240334/204345669-42c3bca5-835b-4ad5-ae13-ea6d8eba673d.jpg)
> - C1 adalah penggabungan subnet A1 dengan B1 dengan netmask /21
> - C2 adalah penggabungan subnet A9 dengan B2 dengan netmask /22
> - C3 adalah penggabungan subnet A15 dengan A16 dengan netmask /23

![D](https://user-images.githubusercontent.com/81240334/204345675-a3ef35e3-1f8c-46a3-8f60-1c82ed9edd2f.jpg)
> - D1 adalah penggabungan subnet A2 dengan C1 dengan netmask /20
> - D2 adalah penggabungan subnet A10 dengan C2 dengan netmask /21
> - D3 adalah penggabungan subnet A12 dengan C3 dengan netmask /23

![E](https://user-images.githubusercontent.com/81240334/204345676-f225edb8-80a9-4154-a2c3-71424aaa3a12.jpg)
> - E1 adalah penggabungan subnet A5 dengan D1 dengan netmask /19
> - E2 adalah penggabungan subnet A7 dengan D2 dengan netmask /20

![F](https://user-images.githubusercontent.com/81240334/204347884-431b9e4b-46ac-483a-b547-db5ffea5b109.jpg)
> - F1 adalah penggabungan subnet D3 dengan E2 dengan netmask /19

![G](https://user-images.githubusercontent.com/81240334/204345691-f46a3187-0d84-4b36-b613-9a8ffea282fd.jpg)
> - G1 adalah penggabungan subnet A6 dengan E1 dengan netmask /18
> - G2 adalah penggabungan subnet A11 dengan F1 dengan netmask /18
> - G3 adalah penggabungan subnet A13 dengan A14 dengan netmask /22

![H](https://user-images.githubusercontent.com/81240334/204345693-7f9983e8-a0bc-43d6-b3ec-fe1f18538cbd.jpg)
> - H1 adalah penggabungan subnet A17 dengan G3 dengan netmask /21

![I](https://user-images.githubusercontent.com/81240334/204345696-ba5cbf89-f605-4d50-a207-18cb8cd211f2.jpg)
> - I1 adalah penggabungan subnet H1 dengan G1 dengan netmask /17

![J](https://user-images.githubusercontent.com/81240334/204345703-82f6fd70-9397-43b6-9a4a-e4b42ea390a2.jpg)
> - J1 adalah penggabungan subnet I1 dengan G2 dengan netmask /16

Dari proses penggabungan yang telah dilakukan, didapatkan sebuah subnet besar dengan netmask /16 dan NID 10.19.0.0. Selanjutnya menghitung pembagian IP dengan pohon berdasarkan penggabungan subnet.

xxx

Berdasarkan penghitungan, maka didapatkan pembagian IP sebagai berikut.


## Konfigurasi Node di GNS3
