# 📚 Manga Translator

> Terjemahkan manga langsung di browser — tanpa install, tanpa server, 100% gratis.

![Version](https://img.shields.io/badge/version-v5-e63946?style=flat-square)
![Languages](https://img.shields.io/badge/languages-60%2B-ffd60a?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-2ec4b6?style=flat-square)
![No Server](https://img.shields.io/badge/server-none-brightgreen?style=flat-square)

**🌐 Live Demo:** [https://username.github.io/manga-translator](https://username.github.io/manga-translator)
> *(ganti `username` dengan username GitHub kamu)*

---

## ✨ Fitur

- 🎬 **Intro screen** animasi bergaya manga saat pertama buka
- 🌍 **Auto-detect bahasa** dari browser pengguna (11 bahasa UI tersedia)
- 📦 **Multi-format** — CBZ, ZIP, PDF, dan gambar langsung (JPG/PNG/WebP)
- 🔍 **OCR** menggunakan Tesseract.js — mendukung 15 bahasa sumber termasuk Jepang, Korea, Mandarin, Arab
- 🌐 **Terjemahan** via MyMemory API ke 21 bahasa target
- 📋 **Copy teks** per halaman (asli maupun terjemahan)
- 🔒 **100% lokal** — gambar tidak pernah dikirim ke server manapun
- 📱 **Responsive** — bisa dipakai di HP maupun desktop

---

## 🖥️ Tampilan

| Intro | Pilih Bahasa | App Utama |
|-------|-------------|-----------|
| Animasi manga-style saat buka | Splash pilihan bahasa dengan auto-detect | Dropzone + panel hasil OCR & terjemahan |

---

## 🚀 Cara Pakai

1. Buka link live demo (atau buka `index.html` langsung di browser)
2. Pilih bahasa UI saat splash screen muncul
3. Pilih format file: **CBZ/ZIP**, **PDF**, atau **Images**
4. Pilih bahasa sumber manga (misal: 🇯🇵 Japanese) dan bahasa tujuan (misal: 🇮🇩 Indonesian)
5. Drop file atau klik tombol pilih file
6. Tunggu proses OCR & terjemahan selesai per halaman
7. Baca hasilnya — atau klik **Copy** untuk salin teksnya

---

## 📂 Format yang Didukung

| Format | Ekstensi | Keterangan |
|--------|----------|------------|
| Comic Book ZIP | `.cbz` | Format standar manga digital |
| ZIP | `.zip` | Archive berisi gambar |
| PDF | `.pdf` | Render setiap halaman PDF sebagai gambar |
| Gambar | `.jpg` `.png` `.webp` `.gif` | Upload langsung, bisa multi-select |

> ⚠️ Format `.cbr` (RAR) belum didukung karena keterbatasan browser.

---

## 🌍 Bahasa yang Didukung

**Bahasa UI (tampilan aplikasi):**
`🇮🇩 Indonesia` `🇬🇧 English` `🇯🇵 日本語` `🇰🇷 한국어` `🇨🇳 中文` `🇪🇸 Español` `🇵🇹 Português` `🇫🇷 Français` `🇩🇪 Deutsch` `🇸🇦 العربية` `🇷🇺 Русский`

**Bahasa sumber OCR (15 bahasa):**
English, Japanese, Korean, Chinese (Simplified & Traditional), Arabic, French, German, Spanish, Portuguese, Italian, Russian, Thai, Vietnamese, Indonesian

**Bahasa tujuan terjemahan (21 bahasa):**
Indonesian, English, Japanese, Korean, Chinese, Arabic, French, German, Spanish, Portuguese, Italian, Russian, Thai, Vietnamese, Malay, Filipino, Turkish, Dutch, Polish, Swedish, Ukrainian, Hindi

---

## ⚙️ Teknologi

| Library | Versi | Fungsi |
|---------|-------|--------|
| [Tesseract.js](https://github.com/naptha/tesseract.js) | 5.0.4 | OCR — ekstrak teks dari gambar |
| [JSZip](https://stuk.github.io/jszip/) | 3.10.1 | Baca file CBZ/ZIP |
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | Render halaman PDF |
| [MyMemory API](https://mymemory.translated.net/) | — | Terjemahan teks (gratis) |

Semua library di-load via CDN — tidak perlu `npm install` apapun.

---

## ⚡ Tips

- OCR paling akurat untuk teks yang kontras tinggi (teks hitam di balon putih)
- Untuk manga Jepang/Korea/Mandarin, download data bahasa ~50MB dilakukan otomatis saat pertama dipakai
- MyMemory API gratis dengan limit ~5.000 karakter/hari per IP — untuk penggunaan kasual sudah cukup
- Gunakan tombol **⇄** untuk tukar bahasa sumber & tujuan dengan cepat
- Klik mana saja di intro screen untuk skip ke halaman utama

---

## 📁 Struktur Repo

```
manga-translator/
├── index.html          ← Aplikasi utama (v5)
├── README.md           ← File ini
└── versions/
    ├── v2.html         ← Bug fixes (worker lang, blob URL, Latin chars)
    ├── v3.html         ← Multi-format (PDF, ZIP, Images)
    └── v4.html         ← Splash bahasa dengan auto-detect
```

---

## 🔧 Deploy Sendiri

Cukup satu file:

```bash
git clone https://github.com/username/manga-translator
cd manga-translator
# Buka index.html di browser — selesai!
```

Untuk deploy ke GitHub Pages:
1. Fork atau upload repo ini
2. Pergi ke **Settings → Pages**
3. Source: **Deploy from branch → main → / (root)**
4. Akses di `https://username.github.io/manga-translator`

---

## 📄 Lisensi

MIT License — bebas digunakan, dimodifikasi, dan didistribusikan.

---

<div align="center">
  <sub>Dibuat dengan ❤️ • Berjalan 100% di browser • Tidak ada data yang dikirim ke server</sub>
</div>
