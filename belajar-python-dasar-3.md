# Belajar Python Dasar

## 1. Dasar-dasar Python

- **Variabel** digunakan untuk menyimpan data, contohnya:
  ```python
  nama = "Kema"
  umur = 23
  ```
- Python memiliki **tipe data** utama seperti:
  - `str` untuk teks
  - `int` untuk angka bulat
  - `float` untuk angka desimal
  - `bool` untuk nilai logika `True` atau `False`
- Komentar dalam Python diawali dengan `#`, berguna untuk memberikan catatan pada kode agar lebih mudah dipahami.

## 2. Operasi Matematika & String

Python mendukung berbagai operasi aritmatika seperti penjumlahan, pengurangan, perkalian, pembagian, modulus (`%`), pembagian bulat (`//`), dan pangkat (`**`).

String juga sangat fleksibel dan dapat dimanipulasi:
- Gabungkan string menggunakan `+`
- Ubah huruf menjadi besar atau kecil dengan `.upper()`, `.lower()`
- Ambil sebagian string (slicing): `kalimat[0:4]`

Contoh:
```python
kalimat = "Halo Dunia"
print(kalimat.upper())      # HALO DUNIA
print(kalimat[0:4])         # Halo
```

## 3. Pengkondisian (if, elif, else)

Pengkondisian digunakan untuk membuat logika program:
```python
usia = 20
if usia >= 18:
    print("Dewasa")
elif usia >= 13:
    print("Remaja")
else:
    print("Anak-anak")
```

Python juga mengenal **operator logika** seperti `and`, `or`, dan `not` untuk membuat kondisi yang kompleks. Misalnya:
```python
if usia > 18 and status == "pelajar":
    print("Pelajar dewasa")
```

## 4. Looping (for dan while)

Loop atau perulangan digunakan untuk mengeksekusi kode berulang kali.

- `for` digunakan untuk iterasi terstruktur, contohnya:
  ```python
  for i in range(5):
      print(i)  # mencetak angka 0 sampai 4
  ```

- `while` digunakan ketika kondisi masih terpenuhi:
  ```python
  x = 0
  while x < 5:
      print(x)
      x += 1
  ```

- Gunakan `break` untuk keluar dari loop, `continue` untuk melewati satu iterasi.
