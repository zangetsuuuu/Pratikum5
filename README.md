Nama: Rafif Isdarufa Athallah

NIM: 312210299

Kelas: TI.22.A3

---

## Latihan

- Buat sebuah list yang berisi 5 elemen

```python
warna = ["Merah", "Hijau", "Hitam", "Abu-abu", "Biru"]
```

- Untuk menampilkan semua elemen didalam list, gunakan fungsi `print(warna)`
- Untuk menampilkan elemen ke-3, gunakan fungsi `print(warna[2])` *( index dimulai dari 0 )*
- Untuk menampilkan elemen ke 2 sampai elemen ke-4, gunakan fungsi `print(warna[1:4])`
- Untuk menampilkan elemen terakhir, gunakan fungsi `print(warna[-1])`

```python
print(warna)
print(warna[2])
print(warna[1:4])
print(warna[-1])
```

Output:

```
["Merah", "Hijau", "Hitam", "Abu-abu", "Biru"]
Hitam
["Hijau", "Hitam", "Abu-abu"]
Biru
```

---

- Untuk mengubah elemen ke-4 dengan nilai lainnya, `warna[3] = "nilai baru"`
- Untuk mengubah elemen ke-4 sampai elemen terakhir, `warna[3:] = "nilai baru", "nilai baru", ...`

```python
warna[3] = "Ungu"

# Isi list menjadi: ["Merah", "Hijau", "Hitam", "Ungu", "Biru"]

warna[3:] = "Putih", "Kuning"

# Isi list menjadi: ["Merah", "Hijau", "Hitam", "Putih", "Kuning"]
```

---

- Untuk mengambil 2 bagian dari **list A** ke **list B**

```python
warna2 = [warna[0], warna[1]]

# Isi list menjadi: ["Merah", "Hijau"]
```

- Untuk menambah elemen list, gunakan `append()` untuk menambahkan elemen ke akhir daftar

```python
warna2.append("Coklat")

# Isi list menjadi: ["Merah", "Hijau", "Coklat"]
```

- Untuk menambah lebih banyak elemen list, gunakan `extend()`

```python
warna2.extend(["Biru Muda", "Violet", "Oren"])

# Isi list menjadi: ["Merah", "Hijau", "Coklat", "Biru Muda", "Violet", "Oren"]
```

- Untuk menggabungkan **list A** dan **list B**, gunakan operasi pertambahan (+)

```python
warna3 = warna + warna2
```

- Jika ditampilkan, maka outputnya:

```
['Merah', 'Hijau', 'Hitam', 'Abu-abu', 'Biru', 'Merah', 'Hijau', 'Biru Muda', 'Violet', 'Oren']
```

## Tugas Pratikum

### Flowchart

![Flowchart.jpg](https://github.com/zangetsuuuu/Pratikum-5/blob/d29830ceee25dc67bdda71cd4cc15e714b770244/gambar/Flowchart.jpg)

---

- Buat sebuah list kosong yang akan digunakan untuk menampung data-data

```python
dataList = []
```

- Gunakan statement `while` untuk melakukan perulangan
- Buat variabel untuk menginput data
- Hitung total sebagai nilai akhir

```python
while True:
    nama = str(input("Nama: "))
    nim = int(input("NIM: "))
    tugas = int(input("Nilai tugas: "))
    uts = int(input("Nilai UTS: "))
    uas = int(input("Nilai UAS: "))
    total = (tugas * 0.30) + (uts * 0.35) + (uas * 0.35)
```

- Gunakan `append()` untuk menambah data ke dalam list

```python
    dataList.append([nama, nim, tugas, uts, uas, total])
```

- Buat pilihan apakah ingin menambah data atau tidak, jika *user* menjawab "t" (tidak) maka program akan berhenti

```python
    pilihan = str(input("Tambah data (y/t)? "))
    print()

    if pilihan == "t":
        break
```

- Tampilkan hasil dengan metode perulangan `for`

```python
print("===================================================================================================")
print("| No |          Nama          |       NIM       |   Tugas   |   UTS   |   UAS   |   Nilai Akhir   |")
print("===================================================================================================")

i = 0
for j in dataList:
    i += 1
    print("| {no:2d} | {nama:22s} | {nim:15d} | {tugas:9d} | {uts:7d} | {uas:7d} | {total:15f} |".format(no=i, nama=j[0], nim=j[1], tugas=j[2], uts=j[3], uas=j[4], total=j[5]))

print("===================================================================================================")
```

### Hasil program

![Hasil Program.jpg](https://github.com/zangetsuuuu/Pratikum-5/blob/d29830ceee25dc67bdda71cd4cc15e714b770244/gambar/Hasil%20Program.jpg)

### Sekian, terimakasih.
