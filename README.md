# Sistem Manajemen Nilai Siswa

## 📋 Deskripsi
Program C++ untuk mengelola data nilai siswa dengan fitur input, tampilkan, simpan ke file, dan baca dari file. Program ini dibuat sebagai tugas Live Coding 01 menggunakan konsep struct, array, file handling, dan fungsi.

## 👤 Informasi Pengembang
- **Nama**: M. KRISNA. Y. P
- **Kelas**: Malam Karyawan TI C
- **Tugas**: Live Coding 01

## ✨ Fitur Utama

### 1. Input Data Siswa
- Memasukkan data siswa baru (nama, NIM, dan 3 nilai mata pelajaran)
- Validasi kapasitas maksimal 100 siswa
- Otomatis menghitung jumlah siswa yang telah diinput

### 2. Tampilkan Data Siswa
- Menampilkan daftar seluruh siswa dalam format tabel
- Menampilkan nama, NIM, 3 nilai, dan rata-rata nilai
- Format output yang rapi dengan lebar kolom tetap
- Presisi 2 digit untuk nilai desimal

### 3. Simpan Data ke File
- Menyimpan seluruh data siswa ke file `data_siswa.txt`
- Format penyimpanan: `Nama;NIM;Nilai1;Nilai2;Nilai3`
- Konfirmasi jumlah siswa yang berhasil disimpan

### 4. Baca Data dari File
- Membaca data siswa dari file `data_siswa.txt`
- Parsing data dengan delimiter semicolon (;)
- Memuat data ke dalam array untuk diproses lebih lanjut
- Konfirmasi jumlah siswa yang berhasil dibaca

### 5. Keluar Program
- Menutup aplikasi dengan pesan perpisahan

## 🛠️ Teknologi yang Digunakan
- **Bahasa**: C++
- **Library**: 
  - `iostream` - Input/output stream
  - `fstream` - File handling
  - `iomanip` - Formatting output
  - `string` - String manipulation
  - `cstring` - C-style string operations

## 📊 Struktur Data

```cpp
struct Siswa {
    string nama;      // Nama siswa
    int nim;          // Nomor Induk Mahasiswa
    float nilai[3];   // Array untuk 3 nilai mata pelajaran
};
```

## 🚀 Cara Menggunakan

### Kompilasi Program
```bash
g++ LiveCoding.cpp -o SistemNilai
```

### Menjalankan Program
```bash
./SistemNilai
```

### Menu Interaktif
```
=== SISTEM MANAJEMEN NILAI SISWA ===
1. Input Data Siswa
2. Tampilkan Data Siswa
3. Simpan Data ke File
4. Baca Data dari File
5. Keluar
Pilihan: 
```

## 📝 Contoh Penggunaan

### Input Data
1. Pilih menu `1`
2. Masukkan nama siswa
3. Masukkan NIM
4. Masukkan 3 nilai mata pelajaran

### Tampilkan Data
```
=== DAFTAR SISWA ===
                Nama            NIM     Nilai 1     Nilai 2     Nilai 3  Rata-rata
=====================================================================
        Ahmad Rizki         123456       85.00       90.00       88.00      87.67
     Siti Nurhaliza         123457       92.00       88.00       95.00      91.67
```

### Format File `data_siswa.txt`
```
Ahmad Rizki;123456;85.0;90.0;88.0
Siti Nurhaliza;123457;92.0;88.0;95.0
```

## 🎯 Fungsi-Fungsi Utama

| Fungsi | Tipe Return | Deskripsi |
|--------|-------------|-----------|
| `tampilkanMenu()` | void | Menampilkan menu utama |
| `hitungRataRata()` | float | Menghitung rata-rata 3 nilai |
| `inputData()` | void | Input data siswa baru |
| `tampilkanDaftar()` | void | Tampilkan daftar siswa |
| `simpanKeFile()` | void | Simpan data ke file txt |
| `bacaFromFile()` | void | Baca data dari file txt |

## ⚙️ Spesifikasi Teknis
- **Kapasitas maksimal**: 100 siswa
- **Jumlah nilai per siswa**: 3 mata pelajaran
- **Format file**: Text file dengan delimiter semicolon (;)
- **Nama file**: `data_siswa.txt`

## 🔍 Validasi & Error Handling
- Cek kapasitas array penuh
- Validasi pembukaan file
- Notifikasi jika tidak ada data
- Pesan error yang informatif

## 📌 Catatan
- Data akan hilang jika tidak disimpan ke file sebelum keluar program
- File `data_siswa.txt` akan dibuat otomatis saat menyimpan data
- Pastikan file `data_siswa.txt` berada di direktori yang sama dengan executable

## 📄 Lisensi
Program ini dibuat untuk keperluan edukasi dan pembelajaran.

---
⭐ **Selamat Mengerjakan!** ⭐
