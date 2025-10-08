# Chat_Analyzer_MAN_13_Jakarta_Selatan
ini adalah hasil riset opsi siswa man13 jakarta yaitu Ihsan Akmal Arrazi Kelas XI-7 dan juga Nabiel Ahmad Zakky Kelas XI-7

# WhatsApp Chat Analyzer - Panduan Lengkap untuk Pemula

## 📋 Daftar Isi
- [Apa itu WhatsApp Chat Analyzer?](#apa-itu-whatsapp-chat-analyzer)
- [Fitur Utama](#fitur-utama)
- [Persyaratan Sistem](#persyaratan-sistem)
- [Panduan Instalasi Lengkap](#panduan-instalasi-lengkap)
- [Cara Menggunakan](#cara-menggunakan)
- [Troubleshooting](#troubleshooting)

---

## 🤔 Apa itu WhatsApp Chat Analyzer?

WhatsApp Chat Analyzer adalah program untuk menganalisis percakapan WhatsApp dan mendeteksi kata-kata kasar atau bullying. Program ini akan membaca file chat WhatsApp Anda dan memberikan laporan lengkap tentang:
- Siapa yang paling banyak menggunakan kata kasar
- Kata-kata apa saja yang terdeteksi
- Grafik visualisasi data
- Analisis sentimen percakapan

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|-------|-----------|
| 🔍 **Deteksi Kata Kasar** | Mendeteksi lebih dari 400+ kata kasar dalam bahasa Indonesia, Inggris, dan lainnya |
| 📊 **Grafik Visual** | Menampilkan diagram batang dan statistik yang mudah dipahami |
| 😊 **Analisis Sentimen** | Menganalisis apakah percakapan positif, negatif, atau netral |
| 🎭 **Anonimisasi** | Menyembunyikan nama asli pengguna untuk privasi |
| 💾 **Export Laporan** | Simpan hasil analisis ke TXT, DOCX, Excel, PDF, atau CSV |
| ⏰ **Filter Waktu** | Analisis berdasarkan periode waktu tertentu |
| 🔔 **Monitoring Real-time** | Peringatan langsung saat kata kasar terdeteksi |

---

## 💻 Persyaratan Sistem

| Komponen | Minimum | Rekomendasi |
|----------|---------|-------------|
| **Sistem Operasi** | Windows 7/8/10/11, macOS 10.12+, Linux | Windows 10/11, macOS 11+ |
| **Processor** | Intel Core i3 atau setara | Intel Core i5 atau lebih tinggi |
| **RAM** | 4 GB | 8 GB atau lebih |
| **Ruang Disk** | 500 MB | 1 GB |
| **Koneksi Internet** | Diperlukan untuk instalasi | - |

---

## 📥 Panduan Instalasi Lengkap

### Langkah 1: Install Python

#### Untuk Windows:

1. **Download Python:**
   - Buka browser, kunjungi: https://www.python.org/downloads/
   - Klik tombol kuning "Download Python 3.12.x" (atau versi terbaru)

2. **Install Python:**
   - Buka file yang sudah didownload (misalnya: `python-3.12.x.exe`)
   - ⚠️ **PENTING:** Centang kotak "Add Python to PATH" di bagian bawah
   - Klik "Install Now"
   - Tunggu hingga selesai (sekitar 5-10 menit)
   - Klik "Close"

3. **Verifikasi Instalasi:**
   - Tekan tombol `Windows + R`
   - Ketik `cmd` lalu tekan Enter
   - Ketik: `python --version`
   - Tekan Enter
   - Jika muncul versi Python (contoh: `Python 3.12.0`), berarti berhasil!

#### Untuk macOS:

1. **Download Python:**
   - Buka browser, kunjungi: https://www.python.org/downloads/
   - Klik "Download Python 3.12.x"

2. **Install Python:**
   - Buka file `.pkg` yang sudah didownload
   - Ikuti wizard instalasi (klik "Continue" → "Agree" → "Install")
   - Masukkan password Mac Anda jika diminta
   - Klik "Close"

3. **Verifikasi Instalasi:**
   - Buka "Terminal" (cari di Spotlight atau buka dari Applications → Utilities)
   - Ketik: `python3 --version`
   - Jika muncul versi Python, berarti berhasil!

---

### Langkah 2: Download File Program

1. **Simpan File:**
   - Copy semua kode program dari file `ChatAnalyzer`
   - Buka Notepad atau VScode
   - Paste kode tersebut
   - Klik "File" → "Save As"
   - Beri nama: `whatsapp_analyzer.py`
   - **Penting:** Pastikan ekstensinya `.py` bukan `.txt`
   - Simpan di folder yang mudah diakses, misalnya: `C:\Users\NamaAnda\Documents\`

---

### Langkah 3: Install Dependensi (Library yang Dibutuhkan)

Ini adalah library-library yang dibutuhkan program untuk bekerja:

| Library | Fungsi | Ukuran (perkiraan) |
|---------|--------|-------------------|
| **tkinter** | Membuat tampilan window program | Sudah termasuk di Python |
| **matplotlib** | Membuat grafik dan diagram | ~100 MB |
| **python-docx** | Export ke format Word | ~5 MB |
| **pandas** | Mengolah data | ~50 MB |
| **openpyxl** | Export ke Excel | ~10 MB |
| **fpdf** | Export ke PDF | ~5 MB |
| **textblob** | Analisis sentimen | ~50 MB |
| **vaderSentiment** | Analisis sentimen lanjutan | ~2 MB |
| **pycryptodome** | Enkripsi data | ~10 MB |
| **numpy** | Perhitungan matematis | ~50 MB |
| **mplcursors** | Interaksi dengan grafik | ~2 MB |

#### Untuk Windows:

1. **Buka Command Prompt:**
   - Tekan `Windows + R`
   - Ketik `cmd`
   - Tekan Enter

2. **Install Semua Library Sekaligus:**
   ```bash
   pip install matplotlib python-docx pandas openpyxl fpdf textblob vaderSentiment pycryptodome numpy mplcursors
   ```

3. **Tunggu Proses Instalasi:**
   - Proses ini akan memakan waktu 5-15 menit tergantung kecepatan internet
   - Anda akan melihat progress bar dan teks yang berjalan
   - Tunggu hingga muncul kembali tulisan `C:\Users\...>`

4. **Instalasi Tambahan untuk TextBlob:**
   ```bash
   python -m textblob.download_corpora
   ```

#### Untuk macOS/Linux:

1. **Buka Terminal**

2. **Install pip (jika belum ada):**
   ```bash
   python3 -m ensurepip --upgrade
   ```

3. **Install Semua Library:**
   ```bash
   pip3 install matplotlib python-docx pandas openpyxl fpdf textblob vaderSentiment pycryptodome numpy mplcursors
   ```

4. **Instalasi Tambahan untuk TextBlob:**
   ```bash
   python3 -m textblob.download_corpora
   ```

---

### Langkah 4: Export Chat WhatsApp

#### Di Android:

1. Buka aplikasi WhatsApp
2. Buka grup atau chat yang ingin dianalisis
3. Tap titik tiga (⋮) di pojok kanan atas
4. Pilih "Lainnya" → "Ekspor chat"
5. Pilih "Tanpa Media"
6. Pilih lokasi penyimpanan (misalnya Google Drive atau Email ke diri sendiri)
7. Download file `.txt` tersebut ke komputer

#### Di iPhone:

1. Buka aplikasi WhatsApp
2. Buka grup atau chat yang ingin dianalisis
3. Tap nama grup/kontak di atas
4. Scroll ke bawah, tap "Ekspor Chat"
5. Pilih "Tanpa Media"
6. Pilih cara mengirim (misalnya Email atau save ke Files)
7. Transfer file ke komputer

---

## 🚀 Cara Menggunakan

### Menjalankan Program

#### Windows:

1. **Cara 1 - Double Click:**
   - Cari file `whatsapp_analyzer.py`
   - Double click file tersebut
   - Program akan terbuka

2. **Cara 2 - Command Prompt:**
   - Buka Command Prompt
   - Ketik: `cd C:\Users\NamaAnda\Documents\` (sesuaikan dengan lokasi file)
   - Ketik: `python whatsapp_analyzer.py`
   - Tekan Enter

#### macOS/Linux:

1. **Buka Terminal**
2. Ketik: `cd ~/Documents/` (sesuaikan dengan lokasi file)
3. Ketik: `python3 whatsapp_analyzer.py`
4. Tekan Enter

---

### Menggunakan Fitur-Fitur Program

| No | Langkah | Deskripsi | Screenshot Area |
|----|---------|-----------|-----------------|
| 1 | **Buka File Chat** | Klik tombol "Buka File Chat" (hijau) → Pilih file `.txt` hasil export WhatsApp | Bagian atas |
| 2 | **Pilih Periode** | Di dropdown "Periode Waktu", pilih rentang waktu yang ingin dianalisis | Bagian atas kiri |
| 3 | **Lihat Laporan** | Laporan otomatis muncul di area teks besar di tengah layar | Area tengah |
| 4 | **Cari Pengguna** | Ketik nama pengguna di kotak "Cari Pengguna" → Klik "Cari" | Bagian atas tengah |
| 5 | **Anonimkan** | Klik "Anonimkan" untuk menyembunyikan nama asli (jadi User1, User2, dst) | Bagian atas |
| 6 | **Lihat Grafik** | Klik tombol diagram yang diinginkan (biru/ungu/merah/orange) | Baris kedua dari atas |
| 7 | **Export Laporan** | Klik salah satu tombol simpan (TXT/DOCX/Excel/PDF/CSV) | Baris ketiga dari atas |

---

### Penjelasan Tombol

| Tombol | Warna | Fungsi |
|--------|-------|--------|
| **Buka File Chat** | 🟢 Hijau | Membuka dan menganalisis file chat WhatsApp |
| **Diagram Pengirim** | 🔵 Biru | Menampilkan grafik jumlah pesan per pengirim |
| **Diagram Metrik Evaluasi** | 🟣 Ungu | Menampilkan akurasi deteksi bullying |
| **Diagram Frekuensi Kata** | 🔴 Merah | Menampilkan kata kasar yang paling sering muncul |
| **Diagram Sentimen** | 🟠 Orange | Menampilkan analisis positif/negatif per pengguna |
| **Anonimkan** | 🟣 Ungu | Menyembunyikan nama asli pengguna |
| **Batal Anonim** | 🟣 Ungu Tua | Mengembalikan nama asli (muncul setelah anonimkan) |
| **Cari** | 🟠 Orange | Mencari statistik pengguna tertentu |
| **Simpan ke TXT** | ⚫ Abu-abu | Menyimpan laporan sebagai file teks biasa |
| **Simpan ke DOCX** | 🔵 Biru Tua | Menyimpan laporan sebagai file Word |
| **Simpan ke Excel** | 🔴 Merah | Menyimpan laporan sebagai spreadsheet Excel |
| **Simpan ke PDF** | 🔴 Pink | Menyimpan laporan sebagai PDF |
| **Simpan ke CSV** | 🟡 Kuning | Menyimpan data sebagai CSV (untuk diolah lagi) |

---

## 📊 Memahami Hasil Analisis

### Bagian Laporan

| Bagian | Penjelasan | Contoh |
|--------|------------|--------|
| **Total pesan bermasalah** | Jumlah pesan yang mengandung kata kasar | 150 dari 5000 pesan |
| **Total kata kasar terdeteksi** | Total kemunculan kata kasar | 200 (bisa lebih dari jumlah pesan karena 1 pesan bisa punya banyak kata kasar) |
| **Total peserta** | Jumlah orang dalam chat | 25 orang |
| **Analisis Sentimen** | Menunjukkan apakah percakapan cenderung positif/negatif | Negatif (-0.45) |
| **Precision** | Seberapa akurat program mendeteksi (0.00 - 1.00) | 0.85 = 85% akurat |
| **Recall** | Seberapa banyak kasus yang berhasil ditemukan | 0.90 = menemukan 90% dari semua bullying |
| **F1 Score** | Keseimbangan antara Precision dan Recall | 0.87 = performa baik |

### Memahami Statistik Per Pengguna

```
User1:
- Total pesan: 500
- Pesan kasar: 50 (10.0%)
- Sentimen rata-rata: Negatif (-0.30)
```

**Artinya:**
- User1 mengirim 500 pesan total
- Dari 500 pesan, 50 (10%) mengandung kata kasar
- Sentimen negatif -0.30 menunjukkan cenderung negatif (skala: -1 sampai +1)

---

## ❗ Troubleshooting (Mengatasi Masalah)

### Masalah Umum dan Solusinya

| Masalah | Penyebab | Solusi |
|---------|----------|--------|
| **Program tidak mau dibuka** | Python belum terinstall dengan benar | Install ulang Python, pastikan centang "Add to PATH" |
| **Error: ModuleNotFoundError** | Library belum terinstall | Jalankan lagi perintah `pip install ...` di Command Prompt/Terminal |
| **File chat tidak terbaca** | Format file tidak sesuai | Pastikan file dari export WhatsApp asli (format `.txt`) |
| **Tidak ada data terdeteksi** | Chat tidak mengandung kata kasar atau format tidak dikenali | Coba chat lain atau cek format timestamp |
| **Program lemot/hang** | File chat terlalu besar | Bagi chat menjadi beberapa periode lebih kecil saat export |
| **Grafik tidak muncul** | matplotlib bermasalah | Tutup program, jalankan: `pip install --upgrade matplotlib` |
| **Error saat save PDF** | Font tidak ditemukan | Install ulang fpdf: `pip install --upgrade fpdf` |

### Error Spesifik

#### Error: "tkinter not found"
**Windows:**
- Reinstall Python, pastikan centang "tcl/tk and IDLE" saat instalasi

**Linux:**
```bash
sudo apt-get install python3-tk
```

**macOS:**
- tkinter seharusnya sudah include, jika error coba:
```bash
brew install python-tk
```

#### Error: "Permission Denied" saat save file
- Tutup file Excel/Word/PDF yang sedang terbuka
- Coba save dengan nama file berbeda
- Pastikan folder tujuan tidak read-only

#### Program tiba-tiba close
- Cek apakah ada file yang corrupt
- Coba jalankan dari Command Prompt/Terminal untuk melihat error message
- Update semua library: `pip install --upgrade matplotlib pandas openpyxl`

---

## 🎓 Tips Penggunaan

| Tips | Penjelasan |
|------|------------|
| **Export tanpa media** | Selalu export WhatsApp tanpa media untuk file lebih kecil dan cepat |
| **Backup file chat** | Simpan file `.txt` asli untuk berjaga-jaga |
| **Gunakan filter waktu** | Untuk grup besar, analisis per periode (misalnya per bulan) |
| **Anonimkan untuk privasi** | Gunakan fitur anonimkan sebelum share laporan ke orang lain |
| **Simpan ke Excel** | Format Excel paling fleksibel untuk analisis lanjutan |
| **Cek grafik sentimen** | Grafik sentimen membantu melihat trend positif/negatif percakapan |

---

## 📞 Bantuan Lebih Lanjut

Jika masih ada masalah setelah mengikuti panduan ini:

1. **Screenshot error message** yang muncul
2. **Catat langkah-langkah** yang sudah dilakukan
3. **Cek versi Python**: Buka Command Prompt/Terminal, ketik `python --version`
4. **Cek versi library**: Ketik `pip list` untuk melihat semua library terinstall

---

## ⚠️ Catatan Penting

- ✅ Program ini GRATIS dan open-source
- ✅ Semua analisis dilakukan di komputer Anda (offline setelah install)
- ✅ Data chat tidak dikirim ke server manapun
- ⚠️ Gunakan secara etis dan bertanggung jawab
- ⚠️ Hormati privasi pengguna lain
- ⚠️ Deteksi tidak 100% akurat, butuh verifikasi manual

---

## 📝 Checklist Instalasi

Centang setiap langkah yang sudah berhasil:

- [ ] Python sudah terinstall (cek dengan `python --version`)
- [ ] File `whatsapp_analyzer.py` sudah disimpan
- [ ] Semua library sudah terinstall (tidak ada error)
- [ ] TextBlob corpora sudah didownload
- [ ] File chat WhatsApp sudah di-export
- [ ] Program berhasil dibuka
- [ ] Berhasil membuka dan menganalisis file chat

---

**Selamat menggunakan WhatsApp Chat Analyzer! 🎉**

*Panduan ini dibuat untuk membantu pengguna non-teknikal. Jika ada bagian yang kurang jelas, jangan ragu untuk bertanya.*
