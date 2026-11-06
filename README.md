# RACIK_AFL2-AI

Racik adalah program manajemen bumbu dapur instan yang membantu pengguna
mengurangi sampah makanan. Program mencatat stok bumbu beserta tanggal
kedaluwarsanya, lalu menentukan bumbu mana yang harus dipakai lebih dulu
menggunakan algoritma **Greedy Best-First Search (GBFS)**, dengan sisa hari
sebelum kedaluwarsa sebagai nilai heuristik.

Anggota
- Arsya Aulia Amira     (0806022410012)
- Cherryl Callista	    (0806022410023)
- Dhiva Kesuma Pertiwi	(0806022410025)
- St Mutmainnah         (0806022410027)


## Library yang Digunakan

**Library standar Python** (sudah bawaan, tidak perlu diinstall):
- `heapq` untuk priority queue pada GBFS
- `dataclasses` untuk struktur data `FoodNode`
- `datetime` untuk penanganan tanggal
- `itertools` untuk penomoran urutan antrean
- `threading` untuk menghapus pesan error secara otomatis

**Library eksternal** (perlu diinstall):
- `ipywidgets` untuk tampilan UI (form, tombol, dropdown)
- `ipykernel` agar notebook bisa berjalan di VS Code
- `IPython` untuk fungsi `display` dan `clear_output` (terpasang otomatis bersama `ipykernel`)

## IDE dan Versi

- **Google Colab**, digunakan pada tahap uji coba awal.
- **Visual Studio Code** versi `isi versi Anda` (cek di *Help → About*), digunakan sebagai lingkungan akhir.
  - Ekstensi **Python** (Microsoft) versi `isi versi`
  - Ekstensi **Jupyter** (Microsoft) versi `isi versi`
- **Python** versi 3.10 atau lebih baru (kode memakai sintaks `date | None`).

Program ini memakai `ipywidgets`, sehingga **harus dijalankan sebagai notebook (`.ipynb`)**, bukan lewat `python racik.py` di terminal.

## Langkah Menjalankan Program

1. **Pasang Python 3.10+** dari https://www.python.org/downloads/ lalu cek dengan `python --version`.
2. **Pasang Visual Studio Code** dari https://code.visualstudio.com/.
3. **Pasang ekstensi** *Python* dan *Jupyter* (keduanya dari Microsoft) lewat menu Extensions (Ctrl+Shift+X).
4. **Unduh atau clone** repository ini, lalu buka foldernya di VS Code (*File → Open Folder*).
5. **Pasang library** lewat terminal VS Code (Ctrl+`):
   ```
   pip install -r requirements.txt
   ```
6. **Buka file `racik.ipynb`**, klik **Select Kernel** di kanan atas, lalu pilih Python environment tempat library tadi dipasang.
7. **Jalankan cell** dengan Shift+Enter atau tombol ▶. Dashboard Racik akan muncul di bawah cell.

### Note

- Disarankan menggunakan Light Mode di VS Code (*Preferences: Color Theme → Light Modern*) untuk tampilan yangl ebih baik.
- Jika widget tidak muncul, pastikan `ipywidgets` terpasang di environment yang sama dengan kernel yang dipilih.