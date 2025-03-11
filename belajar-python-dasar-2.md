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
