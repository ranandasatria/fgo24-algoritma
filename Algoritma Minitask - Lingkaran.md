# Algoritma - Minitask 
Membuat algoritma menghitung luas dan keliling lingkaran
1. Mulai
2. Tentukan variabel: phi = 3,14, r = jari-jari, L = luas, K = keliling
3. Masukkan nilai r
4. Pilih operasi
5. Untuk mencari luas, kalikan phi dengan  r kuadrat, lalu cetak hasilnya
6. Untuk mencari keliling, kalikan angka 2 dengan phi lalu kalikan dengan r, lalu cetak hasilnya
7. Selesai


```mermaid
flowchart LR
    A@{shape: circle, label: "Mulai"}
    B@{shape: lean-r, label: "Masukkan r"}
    C{"Pilih operasi"}
    D@{shape: rect, label: "L = phi × r kuadrat"}
    E@{shape: rect, label: "K = 2 × phi × r"}
    F@{shape: lean-r, label: '"Hasil luas"'}
    G@{shape: lean-r, label: '"Hasil keliling"'}
    H@{shape: dbl-circ, label: "Selesai"}

    A --> B
    B --> C
    C -->|Luas| D --> F --> H
    C -->|Keliling| E --> G --> H
```