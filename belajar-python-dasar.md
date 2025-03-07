# Belajar Python Dasar

## 1. Pendahuluan
Python adalah bahasa pemrograman yang mudah dipelajari dan digunakan. Python sering digunakan untuk pengembangan web, analisis data, kecerdasan buatan, dan berbagai aplikasi lainnya.

## 2. Instalasi Python
Unduh dan instal Python dari [python.org](https://www.python.org/downloads/). Setelah instalasi, pastikan Python sudah terinstal dengan menjalankan perintah berikut di terminal atau command prompt:

```sh
python --version
```

## 3. Hello World
Kode Python pertama yang mencetak teks ke layar:

```python
print("Hello, World!")
```

## 4. Variabel dan Tipe Data
### 4.1 Deklarasi Variabel
Variabel digunakan untuk menyimpan data.
```python
nama = "John"
umur = 25
is_student = True
```

### 4.2 Tipe Data
Python memiliki berbagai tipe data:

| Tipe Data  | Deskripsi | Contoh        |
|------------|-----------|--------------|
| String     | Teks | "Hello" |
| Integer    | Bilangan bulat | 10 |
| Float      | Bilangan desimal | 3.14 |
| Boolean    | Nilai benar atau salah | True / False |
| List       | Kumpulan data yang dapat diubah | [1, 2, 3] |
| Tuple      | Kumpulan data yang tidak dapat diubah | (1, 2, 3) |
| Dictionary | Koleksi pasangan kunci-nilai | {"nama": "John", "umur": 20} |

## 5. Struktur Kontrol
### 5.1 Percabangan (if-elif-else)
Digunakan untuk menjalankan kode berdasarkan kondisi tertentu.
```python
x = 10
if x > 5:
    print("x lebih besar dari 5")
elif x == 5:
    print("x sama dengan 5")
else:
    print("x kurang dari 5")
```

### 5.2 Perulangan
#### 5.2.1 For Loop
Digunakan untuk mengulang kode dalam jumlah tertentu.
```python
for i in range(5):
    print(i)
```

#### 5.2.2 While Loop
Digunakan untuk mengulang kode selama kondisi masih benar.
```python
x = 0
while x < 5:
    print(x)
    x += 1
```

## 6. Fungsi
Fungsi digunakan untuk mengelompokkan kode agar lebih modular.
```python
def sapa(nama):
    return "Halo, " + nama

print(sapa("John"))
```

## 7. List dan Dictionary
### 7.1 List
Struktur data untuk menyimpan banyak nilai.
```python
angka = [1, 2, 3, 4, 5]
print(angka[0])  # Akses elemen pertama
angka.append(6)  # Tambah elemen
```

### 7.2 Dictionary
Struktur data yang menggunakan pasangan kunci-nilai.
```python
mahasiswa = {"nama": "John", "umur": 20}
print(mahasiswa["nama"])  # Akses nilai
mahasiswa["jurusan"] = "Informatika"  # Tambah elemen
```

## 8. Exception Handling
Digunakan untuk menangani kesalahan dalam program.
```python
try:
    angka = int("abc")
except ValueError:
    print("Terjadi kesalahan konversi")
```
