# Algoritma - Minitask 
Membuat algoritma konversi dari Celcius ke Fahrenheit, Kelvin, dan Reamur
1. Mulai
2. Tentukan variabel: C = Celcius, F = Fahrenheit, K = Kelvin, R = Reamur
3. Masukkan suhu dalam C
4. Pilih konversi
5. Jika konversi ke F = (9/5 × C) + 32
6. Jika konversi ke K = C + 273.15
7. Jika konversi ke R = 4/5 x C
8. Cetak hasil F, K, atau R
9. Selesai

## Flowchart
```mermaid
flowchart
a@{shape: circle, label: "Mulai"}
b@{shape: lean-r, label: "C"}
c{Pilih konversi}
d@{shape: rect, label: F = (9/5 × C) + 32}
e@{shape: rect, label: K = C + 273.15}
f@{shape: rect, label: R = 4/5 x C}
g@{shape: lean-r, label: '"F"'}
h@{shape: lean-r, label: '"K"'}
i@{shape: lean-r, label: '"R"'}
j@{shape: dbl-circ, label: "Selesai"}

a --> b
b --> c
c -- Fahrenheit --> d
c -- Kelvin --> e
c -- Reamur--> f
d --> g
e --> h
f --> i
g --> j
h --> j
i --> j