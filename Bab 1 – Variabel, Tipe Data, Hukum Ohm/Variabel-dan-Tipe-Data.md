# Variabel, Tipe Data dan Hukum Ohm

## 📌 Apa itu Variabel di Bahasa C?
- Variabel adalah "tempat penyimpanan" di memori komputer yang digunakan untuk menyimpan data sementara.
- Ibarat **kotak** yang punya:
    * **Name** (misal `umur`)
    * **Tipe data** (misalnya `int`)
    * **Nilai** (misalnya `25`)

## 🛠️ Cara Mendeklarasikan Variabel
- Format dasarnya:
    ```c
    tipe nama_variabel = nilai_awal;
    ```
- Contoh:
    ```c
    int umur = 20;
    float suhu = 28.5;
    char huruf = 'A';
    ```

## 🎯 Tipe Data Utama di C

| Tipe Data       | Penjelasan                 | Contoh              |
|-----------------|----------------------------|---------------------|
| int             | bilangan bulat             | 10, -3              |
| float           | bilangan pecahan           | 3.14                |
| double          | pecahan presisi tinggi     | 3.1415926535        |
| char            | 1 karakter                 | 'A', '9'            |
| long            | bilangan bulat besar       | 123456789           |
| unsigned int    | bilangan bulat tanpa minus | 0–4294967295        |


## 📑 Aturan Penamaan Variabel 
- Variabel harus:
    * dimulai huruf atau underscore
    * hanya boleh berisi huruf, angka, underscore
    * tidak boleh pakai spasi
    * tidak boleh sama dengan keyword C (misal `int`, `while`, dll.)
- Contoh benar:
    ```c
    int nilaiUjian;
    float suhu_ruangan;
    char _kode;
    ```
- Contoh salah:
    ```c
    int 1data;          // tidak boleh diawal angka
    float suhu ruang;   // tidak boleh ada spasi
    chat int;           // tidak boleh pakai keyword
    ```

## 🧪 Inisialisasi vs. Deklarasi
- Deklarasi = menyebutkan tipe + nama variabel
    ```c
    int a
    ```
- Inisialisasi = memberi nilai
    ```c
    a = 10
    ```
- Gabungan (deklarasi + inisialisasi):
    ```c
    int a = 10;
    ```

## 🧪 Mengubah Nilai Variabel
- Nilai bisa diganti kapan saja:
    ```c
    int x = 5;
    x = 12;
    printf("%d",x); // output: 12
    ```

## 🧪 Penggunaan di Program 
- Contoh Program Lengkap
    ```c
    #include <stdio.h>

    int main() {
        int umur = 20;
        float suhu = 32.5;
        char grade = 'A';

        printf("Umur: %d\n", umur);
        printf("Suhu: %.1f\n", suhu);
        printf("Grade: %c\n", grade);

        return 0;
    }
    ```

## 🧪 Multiple Variabel
- Bisa dideklarasi sekaligus:
    ```c
    int a, b, c;
    float x = 1.5, y = 2.7;

    ```

## 🔗 Referensi
- [chatgpt](https://chatgpt.com/c/69309531-0170-8321-83ce-9e6cf872802a)
