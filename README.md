Nama: Rafif Isdarufa Athallah

NIM: 312210299

Kelas: TI.22.A3

## Latihan

```python
warna = ["Merah", "Hijau", "Hitam", "Abu-abu", "Biru"]
print(warna)
print(warna[2])
print(warna[1:4])
```

Output:

```
["Merah", "Hijau", "Hitam", "Abu-abu", "Biru"]
Hitam
["Hijau", "Hitam", "Abu-abu"]
```

## Tugas Pratikum

### Flowchart

![Flowchart.jpg](https://github.com/zangetsuuuu/Pratikum-5/blob/d29830ceee25dc67bdda71cd4cc15e714b770244/gambar/Flowchart.jpg)

```python
dataList = []

while True:
    nama = str(input("Nama: "))
    nim = int(input("NIM: "))
    tugas = int(input("Nilai tugas: "))
    uts = int(input("Nilai UTS: "))
    uas = int(input("Nilai UAS: "))
    total = (tugas * 0.30) + (uts * 0.35) + (uas * 0.35)
```

```python
dataList.append([nama, nim, tugas, uts, uas, total])
```

```python
pilihan = str(input("Tambah data (y/t)? "))
print()

if pilihan == "t":
    break
```

```python
print("===================================================================================================")
print("| No |          Nama          |       NIM       |   Tugas   |   UTS   |   UAS   |   Nilai Akhir   |")
print("===================================================================================================")

i = 0
for j in dataList:
    i += 1
    print("| {no:2d} | {nama:22s} | {nim:15d} | {tugas:9d} | {uts:7d} | {uas:7d} | {akhir:15f} |".format(no=i, nama=j[0], nim=j[1], tugas=j[2], uts=j[3], uas=j[4], akhir=j[5]))

print("===================================================================================================")
```

### Hasil program

![Hasil Program.jpg](https://github.com/zangetsuuuu/Pratikum-5/blob/d29830ceee25dc67bdda71cd4cc15e714b770244/gambar/Hasil%20Program.jpg)

### Sekian, terimakasih.
