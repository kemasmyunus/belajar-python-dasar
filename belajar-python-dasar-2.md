# Belajar Python Lanjutan

## 13. File Handling
File handling digunakan untuk membaca dan menulis file dalam Python.

### 13.1 Membaca File
```python
with open("data.txt", "r") as file:
    isi = file.read()
    print(isi)
```

### 13.2 Menulis File
```python
with open("data.txt", "w") as file:
    file.write("Halo, ini adalah contoh penulisan file!")
```

### 13.3 Menambah Isi File
```python
with open("data.txt", "a") as file:
    file.write("Tambahan teks ke dalam file.\n")
```

## 14. Database dengan SQLite
SQLite adalah database ringan yang dapat digunakan dalam Python menggunakan modul `sqlite3`.

### 14.1 Membuat dan Menghubungkan Database
```python
import sqlite3

conn = sqlite3.connect("database.db")
cursor = conn.cursor()
```

### 14.2 Membuat Tabel
```python
cursor.execute("""
CREATE TABLE IF NOT EXISTS mahasiswa (
    id INTEGER PRIMARY KEY,
    nama TEXT,
    umur INTEGER
)
""")
conn.commit()
```

### 14.3 Menambah Data
```python
cursor.execute("INSERT INTO mahasiswa (nama, umur) VALUES (?, ?)", ("John", 20))
conn.commit()
```

### 14.4 Membaca Data
```python
cursor.execute("SELECT * FROM mahasiswa")
print(cursor.fetchall())
```

### 14.5 Menutup Koneksi
```python
conn.close()
```

## 15. Pemrograman Asinkron dengan `asyncio`
Python mendukung pemrograman asinkron untuk meningkatkan kinerja program yang menangani banyak tugas secara bersamaan.

### 15.1 Contoh Program Asinkron
```python
import asyncio

async def sapa():
    await asyncio.sleep(1)
    print("Halo, Dunia!")

asyncio.run(sapa())
```

