# 📌 Dokumentasi Logo PT Kedap Sayaaq Dua

## ✅ Status Logo - OFFLINE

Semua logo di website ini **sudah diubah menjadi format DATA URI (Base64)**, sehingga:
- ✅ **Tidak memerlukan koneksi internet** untuk ditampilkan
- ✅ **Tersimpan langsung di dalam file HTML** 
- ✅ **Tidak bergantung pada server eksternal**
- ✅ **Bisa digunakan kapan saja, di mana saja**

---

## 🎨 Lokasi Logo yang Sudah Diganti

### 1. **FAVICON** (Tab Browser)
- **File:** `dashboard.html`
- **Baris:** 8
- **Fungsi:** Logo yang muncul di tab browser
- **Format:** SVG dengan gradasi hijau (Base64)

### 2. **NAVBAR LOGO** (Header Navigasi)
- **File:** `dashboard.html`
- **Baris:** 227
- **Fungsi:** Logo di bagian atas kiri saat navigasi
- **Format:** SVG dengan gradasi hijau (Base64)

### 3. **MODAL LOGIN LOGO** (Portal Karyawan)
- **File:** `dashboard.html`
- **Baris:** 775
- **Fungsi:** Logo yang muncul di modal login
- **Format:** SVG dengan gradasi hijau (Base64)

### 4. **FOOTER LOGO** (Bagian Bawah)
- **File:** `dashboard.html`
- **Baris:** 709
- **Fungsi:** Logo di footer bersama informasi perusahaan
- **Format:** SVG dengan gradasi hijau (Base64)

---

## 📝 Informasi Data URI

### Format SVG Base64 yang Digunakan:
```
data:image/svg+xml;base64,[STRING BASE64 PANJANG]
```

### Deskripsi Logo:
- **Tipe:** SVG (Vector - Scalable)
- **Warna:** Gradasi Hijau (#6ba547 → #2d7a4a)
- **Desain:** Leaf/Palm dengan relief 3D
- **Kompatibilitas:** Semua browser modern ✓

---

## 🔧 Cara Mengganti Logo dengan Gambar Custom

Jika Anda ingin mengganti logo dengan gambar sendiri, ikuti langkah berikut:

### Opsi 1: Konversi Gambar ke Base64
1. Upload gambar Anda ke website converter (contoh: https://www.base64-image.de/)
2. Convert gambar ke format Base64
3. Copy kode Base64 yang dihasilkan
4. Ganti seluruh kode `data:image/svg+xml;base64,...` dengan:
   ```
   data:image/png;base64,[KODE BASE64 ANDA]
   ```
   atau
   ```
   data:image/jpeg;base64,[KODE BASE64 ANDA]
   ```

### Opsi 2: Menggunakan File Lokal
Jika ingin menggunakan file lokal (disimpan di folder yang sama):
1. Buat folder `assets` atau `images` di folder project
2. Simpan logo Anda di folder tersebut (misal: `assets/logo.png`)
3. Ganti URL dari:
   ```html
   <img src="data:image/svg+xml;base64,..." />
   ```
   Menjadi:
   ```html
   <img src="./assets/logo.png" />
   ```

---

## 📊 Keuntungan Menggunakan Data URI

| Fitur | Data URI | File Lokal | URL Internet |
|-------|----------|-----------|-------------|
| **Offline** | ✅ | ✅ | ❌ |
| **Tidak butuh file terpisah** | ✅ | ❌ | ❌ |
| **Ukuran file** | Sedang | Kecil | Tidak ada |
| **Kecepatan loading** | Cepat | Sangat cepat | Tergantung internet |
| **Portabilitas** | Mudah | Mudah | Bergantung server |

---

## 🎯 Rekomendasi

### Gunakan Data URI jika:
- Ingin website berfungsi offline ✓
- Logo simple/sedang (ukuran < 100KB) ✓
- Tidak perlu update logo sering ✓

### Gunakan File Lokal jika:
- Logo kompleks dengan banyak detail
- Perlu update logo sering
- Ingin file HTML tetap ringkas

---

## 📝 Contoh Kode

**Saat ini (Data URI SVG):**
```html
<img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgdmlld0JveD0iMCAwIDIwMCAyMDAiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+..." class="h-12 w-12 rounded-lg" />
```

**Jika ingin pakai file lokal:**
```html
<img src="./assets/logo.png" class="h-12 w-12 rounded-lg" />
```

---

## ⚠️ Catatan Penting

1. **Ukuran File HTML**: Data URI akan membuat file HTML lebih besar (~10-15KB untuk logo SVG)
2. **Browser Support**: Semua browser modern mendukung Data URI ✓
3. **SEO**: Tidak ada pengaruh terhadap SEO
4. **Performance**: Loading time hampir sama dengan URL internet

---

## 📞 Support

Jika ada pertanyaan atau ingin customize logo lebih lanjut, silakan hubungi tim IT.

**Dibuat:** 20 Januari 2026  
**Status:** ✅ Offline Ready
