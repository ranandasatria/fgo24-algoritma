# Algoritma - Minitask 
Membuat algoritma untuk menentukan bilangan ganjil atau genap
1. Mulai
2. Masukkan bilangan x yang ingin diperiksa
3. Bagi bilangan x tersebut dengan 2
4. Jika habis dibagi 2, maka bilangan x tersebut bilangan genap
5. Jika tidak habis dibagi 2, maka bilangan x tersebut bilangan ganjil
6. Selesai

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
A((Mulai)) --> B[/x/] 
B --> C{X dibagi 2 sama dengan 0}
C -- Ya --> D[/'"Bilangan Genap"'/]
C -- Tidak --> E[/'"Bilangan Ganjil"'/]
D --> F(((Selesai)))
E --> F
```

## Pseudocode
```
DECLARE x: INTEGER

INPUT x

IF x MOD 2 = 0 THEN
    OUTPUT "Bilangan Genap"
ELSE
    OUTPUT "Bilangan Ganjil"
ENDIF
```