# Range Tipe Data (overflow, underflow)

## 📌 Apa itu Range Tipe Data di C?
- Setiap tipe data di C memiliki **jumlah bit tetap** → sehingga nilai yang bisa ditampung juga terbatas.
- Contoh:
    * `int` biasanya 32-bit → mampu menampung angka dari sekitar -2 milyar s/d +2 milyar.
    * `char` adalah 1 byte → mampu menampung -128 s/d 127.

## 📌 Tabel Range Standar Tipe Data C
> Catatan: *Angka ini berlaku pada arsitektur umum 32-bit/64-bit (compiler modern seperti GCC/Clang).* 
**A. Integer Types**
| Tipe Data            | Ukuran        | Range                                  |
| -------------------- | ------------- | -------------------------------------- |
| `char`               | 1 byte        | -128 to 127                            |
| `unsigned char`      | 1 byte        | 0 to 255                               |
| `short`              | 2 byte        | -32,768 to 32,767                      |
| `unsigned short`     | 2 byte        | 0 to 65,535                            |
| `int`                | 4 byte        | -2,147,483,648 to 2,147,483,647        |
| `unsigned int`       | 4 byte        | 0 to 4,294,967,295                     |
| `long`               | 4 atau 8 byte | (umumnya sama seperti int atau 64-bit) |
| `long long`          | 8 byte        | -9.22e18 to 9.22e18                    |
| `unsigned long long` | 8 byte        | 0 to 1.84e19                           |
**B. Floating Types**
| Tipe Data     | Ukuran     | Perkiraan Range  |
| ------------- | ---------- | ---------------- |
| `float`       | 4 byte     | ±3.4e38          |
| `double`      | 8 byte     | ±1.7e308         |
| `long double` | 10–16 byte | jauh lebih besar |

## 📌 Apa itu Overflow dan Underflow?
**1. Overflow**
Terjadi ketika nilai **lebih besar** dari yang bisa ditampung **tipe data**.
contoh:
    ```c
    unsigned char x = 255;
    x = x + 1;  // overflow
    printf("%d", x);
    ```
Hasilnya:
    ```C
    x = 0
    ```
Karena 255 + 1 → kembali ke 0 (wrap around).

## 🛠️ Contoh Penggunaan
- Skematik / diagram / alur program (opsional)
- Kode contoh

## 📑 Catatan Penting
- Tips
- Edge case
- Kesalahan umum

## 🧪 Percobaan Yang Saya Lakukan
- Arah belajar
- Hasil testing
- Foto (kalau ada)

## 🔗 Referensi
- Link tutorial
- Datasheet
- Repo orang lain
