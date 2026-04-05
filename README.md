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