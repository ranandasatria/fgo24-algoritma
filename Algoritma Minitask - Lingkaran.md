# Algoritma - Minitask 
Membuat algoritma menghitung luas dan keliling lingkaran
1. Mulai
2. Masukkan nilai r
3. Jika r bisa dibagi 7, maka nilai phi 22/7
4. Jika tidak, maka nilai phi 3.14
5. Jika ingin mencari luas lingkaran, kalikan phi dengan  r kuadrat, lalu cetak hasilnya
6. Jika tidak, kalikan angka 2 dengan phi lalu kalikan dengan r, lalu cetak hasilnya untuk mengetahui keliling lingkaran
7. Selesai

## Flowchart
```mermaid
flowchart 
    A@{shape: circle, label: "Mulai"}
    B@{shape: lean-r, label: "Masukkan nilai r"}
    phi{"Apakah r bisa dibagi 7?"}
    phib@{shape: rect, label: "Phi = 22/7"}
    phic@{shape: rect, label: "Phi = 3.14"}
    C{"Ingin mencari luas?"}
    D@{shape: rect, label: "L = phi × r x r"}
    E@{shape: rect, label: "K = 2 × phi × r"}
    F@{shape: lean-r, label: "Cetak: Luas lingkaran adalah 'L'"}
    G@{shape: lean-r, label: "Cetak: Keliling lingkaran adalah 'K'"}
    H@{shape: dbl-circ, label: "Selesai"}

    A --> B
    B --> phi
    phi --YA--> phib
    phi --TIDAK--> phic
    phib --> C
    phic --> C
    C --YA--> D --> F --> H
    C --TIDAK--> E --> G --> H
```

## Pseudocode

```
DECLARE r: REAL
DECLARE phi: REAL
DECLARE L: REAL
DECLARE K: REAL
DECLARE pilihan: STRING

INPUT r

IF r MOD 7 = 0 THEN
    phi ← 22 / 7
ELSE
    phi ← 3.14
ENDIF

OUTPUT "Ingin mencari luas? (YA/TIDAK):"
INPUT pilihan

IF pilihan = "YA" THEN
    L ← phi * r * r
    OUTPUT "Luas lingkaran adalah ", L
ELSE
    K ← 2 * phi * r
    OUTPUT "Keliling lingkaran adalah ", K
ENDIF

```
