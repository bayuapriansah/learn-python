
**Materi Belajar Python Dasar untuk Calon Data Analyst**

---

### 1. Instalasi Python dan IDE

**a. Instalasi Python:**
- Kunjungi situs resmi Python di https://www.python.org/downloads/.
- Pilih versi Python terbaru (disarankan versi 3.11 ke atas).
- Jalankan installer dan pastikan mencentang opsi "Add Python to PATH" agar Python bisa diakses dari command prompt.
- Setelah instalasi, cek instalasi dengan perintah `python --version` di terminal.

**b. Instalasi IDE (Integrated Development Environment):**
- **Visual Studio Code (VS Code):**
  - Kunjungi https://code.visualstudio.com dan download untuk sistem operasi yang kamu gunakan.
  - Setelah instalasi, buka VS Code dan pasang ekstensi "Python" dari Microsoft agar mendukung penulisan kode Python dengan fitur seperti auto-completion dan debugging.
- **Jupyter Notebook (melalui Anaconda):**
  - Anaconda merupakan distribusi Python yang cocok untuk analisis data.
  - Unduh dari https://www.anaconda.com/ dan ikuti proses instalasi.
  - Buka "Anaconda Navigator", lalu klik "Launch" pada Jupyter Notebook.
  - Jupyter sangat cocok untuk analisis data karena mendukung kombinasi teks dan kode dalam satu dokumen interaktif.

---

### 2. Variabel dan Tipe Data

Python memiliki tipe data dasar seperti:
- `str` (string)
- `int` (bilangan bulat)
- `float` (bilangan desimal)
- `bool` (boolean: True/False)

Contoh penggunaan:
```python
# Contoh variabel dan tipe data
nama = "Patrick Star"           # string
umur = 25                # integer
berat = 68.5             # float
aktif = True             # boolean
```

Gunakan fungsi `type()` untuk mengetahui tipe data:
```python
print(type(nama))  # <class 'str'>
print(type(umur))  # <class 'int'>
```

Variabel bisa dinamai bebas (asal tidak pakai spasi atau simbol khusus), dan tidak perlu deklarasi tipe secara eksplisit.

---

### 3. Operasi Dasar

**a. Operasi Aritmatika:**
Python mendukung semua operasi matematika dasar:
```python
x = 10
y = 3
print(x + y)   # Penjumlahan
print(x - y)   # Pengurangan
print(x * y)   # Perkalian
print(x / y)   # Pembagian (hasil float)
print(x // y)  # Pembagian bulat (floor division)
print(x % y)   # Modulus (sisa bagi)
print(x ** y)  # Pangkat
```

**b. Operasi Logika dan Perbandingan:**
Operator logika dan perbandingan digunakan dalam pengambilan keputusan:
```python
print(x > y)    # True
print(x == y)   # False
print(x != y)   # True
print(x >= y)   # True
```
Boolean (`True` / `False`) bisa digunakan dalam kondisi dan perulangan.

---

### 4. Struktur Kontrol

**a. If, Elif, Else:**
Struktur kontrol digunakan untuk pengambilan keputusan:
```python
nilai = 85
if nilai >= 90:
    print("A")
elif nilai >= 80:
    print("B")
else:
    print("C")
```

Indentasi (spasi di awal baris) sangat penting di Python!

**b. Looping - For dan While:**
Gunakan `for` untuk iterasi berdasarkan urutan, dan `while` untuk kondisi logika:
```python
# For loop dengan range
for i in range(5):
    print(i)

# While loop
count = 0
while count < 5:
    print(count)
    count += 1
```

---

### 5. Fungsi
Fungsi digunakan untuk membuat blok kode yang dapat digunakan ulang:
```python
def sapa(nama):
    return f"Halo, {nama}!"

print(sapa("Patrick Star"))
```
Fungsi bisa memiliki parameter dan nilai balik (`return`).
Fungsi membantu mengorganisasi kode dan menghindari pengulangan.

---

### 6. Struktur Data

**a. List (daftar):**
Digunakan untuk menyimpan kumpulan nilai:
```python
buah = ["apel", "jeruk", "pisang"]
buah.append("anggur")
print(buah[0])  # apel
```
List bersifat mutable (bisa diubah).

**b. Tuple:**
Mirip list tapi immutable (tidak bisa diubah):
```python
angka = (1, 2, 3)
print(angka[1])
```

**c. Set:**
Digunakan untuk menyimpan elemen unik (tanpa duplikat):
```python
unik = {1, 2, 2, 3}
print(unik)  # {1, 2, 3}
```

**d. Dictionary (kamus):**
Menyimpan pasangan kunci-nilai:
```python
mahasiswa = {"nama": "Patrick Star", "umur": 25}
print(mahasiswa["nama"])
```
Dictionary sangat berguna untuk data terstruktur.

---

### 7. Error Handling
Untuk menangani error agar program tidak berhenti secara tiba-tiba:
```python
try:
    hasil = 10 / 0
except ZeroDivisionError:
    print("Tidak bisa membagi dengan nol.")
```
Selain `ZeroDivisionError`, ada juga error seperti `ValueError`, `TypeError`, dll.
Error handling penting saat bekerja dengan data real yang tidak selalu bersih.

---

### Penutup

Materi ini adalah dasar penting sebelum masuk ke dunia data analysis yang lebih kompleks. Penguasaan Python dari sisi sintaks, struktur data, fungsi, dan kontrol logika akan sangat membantu dalam mengolah dan menganalisis data nantinya. Setelah bagian ini, kamu bisa lanjut ke tahap berikutnya seperti penggunaan Pandas untuk manipulasi data, visualisasi dengan Matplotlib dan Seaborn, serta statistik dasar.

Teruslah berlatih dan eksplorasi berbagai contoh kode serta buatlah mini project kecil agar skill kamu makin matang!
