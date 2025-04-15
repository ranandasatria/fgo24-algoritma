# Algoritma - Minitask 
Membuat algoritma untuk menentukan bilangan ganjil atau genap
1. Mulai
2. Masukkan bilangan yang ingin diperiksa
2. Bagi bilangan tersebut dengan 2
3. Jika tidak habis dibagi 2 atau hasilnya 1, maka bilangan tersebut bilangan ganjil
4. Jika habis dibagi 2 atau hasilnya 0, maka bilangan tersebut bilangan genap
5. Selesai

## Flowchart (Pakai sintaks semantik)
```mermaid
flowchart LR
a@{shape: circle, label: "Mulai"}
b@{shape: lean-r, label: "x"}
c{x % 2 == 0}
d@{shape: lean-r, label: '"Bilangan Genap"'}
e@{shape: lean-r, label: '"Bilangan Ganjil"'}
f@{shape: dbl-circ, label: "Selesai"}

a --> b
b --> c
c -- Ya --> d
c -- Tidak --> e
d --> f
e --> f 

```

## Flowchart (Langsung shape)

```mermaid
flowchart
A((Mulai)) --> B[/Masukkan bilangan/] 
B --> C{Bilangan dibagi 2 sama dengan 0?}
C -- Ya --> D[/"Bilangan Genap"/]
C -- Tidak --> E[/"Bilangan Ganjil"/]
D --> F(((Selesai)))
E --> F
```
## Pseudocode cara 1
```
DECLARE Ganjil: INTEGER
DECLARE Genap: INTEGER
DECLARE x: INTEGER

INPUT x

Ganjil <- x % 2 != 0
Genap <- x % 2 == 0

OUTPUT Ganjil, "adalah Bilangan Ganjil"
OUTPUT Genap, "adalah Bilangan Genap"
```

## Pseudocode cara 2
```
DECLARE Bilangan : INTEGER

INPUT Bilangan

IF Bilangan MOD 2 = 0 THEN
    OUTPUT "Bilangan Genap"
ELSE
    OUTPUT "Bilangan Ganjil"
ENDIF
```