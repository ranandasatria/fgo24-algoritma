# Algoritma - Minitask 
Membuat algoritma konversi dari Celcius ke Fahrenheit, Kelvin, dan Reamur
1. Mulai
2. Tentukan variabel: C = Celcius, F = Fahrenheit, K = Kelvin, R = Reamur
3. Masukkan suhu dalam C
5. Jika konversi ke F = (9/5 × C) + 32
6. Jika konversi ke K = C + 273.15
7. Jika konversi ke R = 4/5 x C
8. Cetak hasil F, K, atau R sebagai result
9. Selesai

## Flowchart
```mermaid
flowchart
a@{shape: circle, label: "Mulai"}
b@{shape: lean-r, label: "C"}
d@{shape: rect, label: F = (9/5 × C) + 32}
e@{shape: rect, label: K = C + 273.15}
f@{shape: rect, label: R = 4/5 x C}
output@{shape: lean-r, label: '"result"'}
j@{shape: dbl-circ, label: "Selesai"}

a --> b
b --> d
d --True--> output
d --False--> e
e --True--> output
e --False--> f
f --True--> output
output --> j
f --False --> j
