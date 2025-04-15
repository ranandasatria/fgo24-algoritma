# Algoritma - Minitask 
Membuat algoritma konversi dari Celcius ke Fahrenheit, Kelvin, dan Reamur
1. Mulai
2. Tentukan variabel: C = Celcius, F = Fahrenheit, K = Kelvin, R = Reamur
3. Masukkan suhu dalam C
4. Pilih tipe konversi
5. Jika konversi ke F = (9/5 × C) + 32
6. Jika konversi ke K = C + 273.15
7. Jika konversi ke R = 4/5 x C
8. Cetak hasil F, K, atau R sebagai Result
9. Selesai

## Flowchart
```mermaid
flowchart
a@{shape: circle, label: "Mulai"}
b@{shape: lean-r, label: "Input:C"}
type@{shape: lean-r, label: "Input:Type"}
selector1{"Type == F"}
selector2{"Type == K"}
selector3{"Type == R"}
d@{shape: rect, label: Result = (9/5 × C) + 32}
e@{shape: rect, label: Result = C + 273.15}
f@{shape: rect, label: Result = 4/5 x C}
output@{shape: lean-r, label: '"Output:Result"'}
j@{shape: dbl-circ, label: "Selesai"}

a --> b
b --> type
type --> selector1
selector1 --True--> d
selector1 --False--> selector2
selector2 --True--> e
selector2 --False--> selector3
selector3 --True--> f
d --> output
e --> output
f --> output
output --> j
f --False --> j

```

## Pseudocode
```
// Program Konversi Suhu

DECLARE Celcius: REAL
DECLARE Result: REAL
DECLARE Type: CHAR

INPUT Celcius
INPUT Type

IF Type == "K"
    Result <- Celcius + 273
ENDIF
IF Type == "F"
    Result <- (9/5 x Celcius) + 32
ENDIF
IF Type == "R"
    Result <- 4/5 x Celcius
ENDIF

OUTPUT "Hasil konversi suhu adalah:", Result

