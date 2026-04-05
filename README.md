
# Latihan Membuat Device Tree (DTS)

Repositori sederhana ini berisi catatan dasar cara membuat, mengompilasi, dan membongkar file Device Tree untuk keperluan kernel Linux.

## Struktur File
- `belajar.dts`: Source code mentah yang kita tulis manual.
- `belajar.dtb`: Hasil kompilasi (binary) yang siap dibaca sistem.

## Alur Kerja (Workflow)

### 1. Install Compiler
Pastikan kamu sudah menginstal `device-tree-compiler`.
```bash
sudo apt install device-tree-compiler
```

### 2. Kompilasi (DTS ke DTB)
Gunakan perintah ini untuk mengubah file teks menjadi file biner:
```bash
dtc -I dts -O dtb -o belajar.dtb belajar.dts
```

### 3. Decompile (DTB ke DTS)
Gunakan perintah ini jika ingin melihat isi file biner atau belajar dari file `.dtb` milik perangkat lain:
```bash
dtc -I dtb -O dts -o hasil_bongkar.dts belajar.dtb
```

## Aturan Main Penulisan
- Selalu akhiri properti dan penutup kurung kurawal `};` dengan titik koma.
- Gunakan `/dts-v1/;` di baris paling atas.
- Root node selalu dimulai dengan `/ { ... };`.


*Selamat belajar oprek hardware!*


# Cara Simpan:
1. Buka Notepad atau VS Code.
2. Paste kode di atas.
3. Simpan dengan nama `README.md` (pastikan ekstensinya `.md`).

