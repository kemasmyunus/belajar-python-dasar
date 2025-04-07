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

## 5. Fungsi dan Return Value

Fungsi adalah blok kode yang dapat digunakan kembali. Digunakan untuk mengorganisasi program agar lebih modular.

```python
def sapa(nama):
    return f"Halo {nama}"

print(sapa("Kema"))
```

Fungsi bisa memiliki parameter default, menerima beberapa parameter, dan mengembalikan nilai (`return`). Fungsi juga mendukung *scope* variabel lokal dan global.

## 6. List, Tuple, dan Set

- **List** adalah kumpulan data yang dapat diubah (mutable):
  ```python
  buah = ["apel", "jeruk"]
  buah.append("mangga")
  ```
- **Tuple** adalah versi list yang tidak dapat diubah (immutable):
  ```python
  angka = (1, 2, 3)
  ```
- **Set** adalah kumpulan unik tanpa urutan:
  ```python
  angka_set = {1, 2, 2, 3}  # hasil: {1, 2, 3}
  ```
Set berguna untuk operasi himpunan seperti gabungan, irisan, dan perbedaan.

## 7. Dictionary (Kamus)

Dictionary menyimpan data dalam format key-value. Cocok untuk data yang saling berpasangan seperti nama dan umur.

```python
siswa = {"nama": "Kema", "umur": 23}
print(siswa["nama"])
siswa["umur"] = 24
```

Method umum:
- `.keys()` untuk mengambil semua key
- `.values()` untuk mengambil semua nilai
- `.items()` untuk pasangan key dan value

## 8. Exception Handling

Error bisa menyebabkan program berhenti. Python menyediakan blok `try-except` untuk menangani error agar program tetap berjalan.

```python
try:
    hasil = 10 / 0
except ZeroDivisionError:
    print("Tidak bisa bagi nol!")
finally:
    print("Selesai mencoba.")
```

Kita juga bisa membuat pengecualian untuk beberapa jenis error sekaligus.

## 9. File Handling

Membaca dan menulis file adalah kemampuan penting dalam pemrograman. Python memudahkan manipulasi file teks:

- **Membaca file:**
  ```python
  with open("data.txt", "r") as file:
      isi = file.read()
  ```
- **Menulis file:**
  ```python
  with open("data.txt", "w") as file:
      file.write("Halo dunia!")
  ```
- `"a"` digunakan untuk menambahkan data tanpa menghapus isi lama.

## 10. Object Oriented Programming (OOP)

OOP memungkinkan kita membuat class untuk merepresentasikan objek nyata dengan atribut dan perilaku.

```python
class Siswa:
    def __init__(self, nama, umur):
        self.nama = nama
        self.umur = umur

murid = Siswa("Kema", 23)
print(murid.nama)
```

Konsep penting:
- **Encapsulation:** menyembunyikan data internal
- **Inheritance:** pewarisan class induk ke class anak
- **Polymorphism:** metode dengan nama sama berperilaku berbeda

## 11. Modul dan Package

Modul adalah file Python yang bisa digunakan ulang.

- Modul built-in:
  ```python
  import math
  print(math.sqrt(16))
  ```

- Modul buatan sendiri:
  Buat file `hello.py`:
  ```python
  def sapa():
      print("Halo dunia!")
  ```
  Kemudian import di file utama:
  ```python
  import hello
  hello.sapa()
  ```

Packages adalah folder berisi banyak modul, biasanya digunakan dalam proyek besar.
