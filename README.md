📌 Profil Kelompok - Web HTML & CSS
📖 Deskripsi Proyek

Proyek ini merupakan tugas pembuatan halaman web sederhana bertema Profil Kelompok menggunakan HTML dan CSS.
Halaman ini menampilkan informasi anggota kelompok dalam bentuk tabel yang telah dipercantik dengan berbagai teknik styling CSS.

🎯 Tujuan
Memahami struktur dasar HTML
Menggunakan tabel dalam HTML
Mengimplementasikan Inline CSS, Internal CSS, dan External CSS
Menerapkan styling seperti warna, font, dan background
🧩 Fitur Utama

✅ Menampilkan profil kelompok dalam bentuk tabel
✅ Berisi:

Nama Kelompok
Nama Anggota
NIM
Kata Motivasi

✅ Menggunakan:

🎨 Inline CSS (langsung pada elemen)
🎨 Internal CSS (di dalam <style>)
🎨 External CSS (file terpisah)
🛠️ Teknologi yang Digunakan
HTML5
CSS3
📂 Struktur Folder
profil-kelompok/
│── index.html
│── style.css
│── README.md
🎨 Implementasi Styling
1. Inline CSS

Digunakan langsung pada elemen HTML, contoh:

<td style="color: blue;">Nama Anggota</td>
2. Internal CSS

Digunakan untuk styling heading:

<style>
h1 {
    color: darkblue;
    text-align: center;
}
</style>
3. External CSS

Digunakan untuk styling paragraf:

p {
    font-family: Arial;
    color: gray;
    font-size: 14px;
}
✨ Tampilan yang Diharapkan
Tabel rapi dan berwarna
Font menarik dan mudah dibaca
Background tidak monoton
Heading menonjol
👥 Anggota Kelompok
Nama	NIM	Kelas
1.  Nama  : Zul Ikhwanul Anggara 
    NIM   : 255410043
    Kelas : IF1
2.  Nama  : Hendrik Firmansyah
    NIM   : 255410075
    Kelas : IF1
3.  Nama  : Odilia Valensia Pradevi Putri
    NIM   : 255410045
    Kelas : IF1

    
🚀 Cara Menjalankan
Download atau clone repository ini
Buka file index.html
Jalankan di browser
---

## 📚 Penjelasan Detail Kode

### Struktur HTML

#### Deklarasi Dokumen & Metadata
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Kelompok</title>
</head>
```

**Penjelasan:**
- **`<!DOCTYPE html>`**: Mendeklarasikan bahwa dokumen menggunakan standar HTML5
- **`lang="id"`**: Menetapkan bahasa dokumen ke Bahasa Indonesia, membantu aksesibilitas dan SEO
- **`<meta charset="UTF-8">`**: Mengatur encoding karakter untuk menampilkan karakter spesial dengan benar
- **`<meta name="viewport">`**: Memastikan halaman responsif di perangkat mobile dengan menyesuaikan skala otomatis

#### Struktur Tabel
```html
<table>
    <tr>
        <th>Nama Kelompok</th>
        <th>Nama Anggota</th>
        <th>NIM</th>
        <th>Kata Motivasi</th>
    </tr>
    <!-- Data rows dengan informasi anggota -->
</table>
```

**Fungsi:**
- **`<table>`**: Container untuk data terstruktur
- **`<tr>` (Table Row)**: Mendeklarasikan setiap baris dalam tabel
- **`<th>` (Table Header)**: Menentukan judul/header kolom
- **`<td>` (Table Data)**: Berisi data aktual dari setiap anggota

---

### CSS Internal (Inline Styling)

#### 1. Global Styling pada `<body>`
```css
body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #eef6fb;
}
```

**Penjelasan:**
- **`margin: 0`**: Menghilangkan margin default browser sehingga warna latar belakang mencakup seluruh halaman
- **`font-family`**: Mengatur urutan font fallback - jika Segoe UI tidak tersedia, gunakan alternatif lain
- **`background-color: #eef6fb`**: Warna latar belakang biru muda yang lembut dan menenangkan

#### 2. Styling Heading
```css
h1 {
    color: #0a3d62;
    text-align: center;
    margin-top: 30px;
}
```

**Penjelasan:**
- **`color: #0a3d62`**: Warna teks biru gelap yang professional
- **`text-align: center`**: Memusatkan judul di halaman
- **`margin-top: 30px`**: Memberikan jarak dari atas halaman (padding visual)

#### 3. Container Layout
```css
.container {
    width: 85%;
    margin: 30px auto;
    text-align: center;
}
```

**Penjelasan:**
- **`width: 85%`**: Lebar relatif (responsive) - menyesuaikan dengan ukuran layar
- **`margin: 30px auto`**: 
  - `30px` untuk atas-bawah
  - `auto` untuk kiri-kanan (memusatkan container secara horizontal)
- **`text-align: center`**: Memusatkan semua konten teks di dalam container

#### 4. Styling Tabel (Kunci Desain)
```css
table {
    width: 100%;
    border-collapse: collapse;
    background-color: #ffffff;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}
```

**Penjelasan Detail:**
- **`border-collapse: collapse`**: Menghilangkan jarak antar sel untuk tampilan rapi dan profesional
- **`border-radius: 10px`**: Membuat sudut tabel melengkung untuk desain modern
- **`overflow: hidden`**: Memotong konten agar mengikuti sudut melengkung
- **`box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1)`**: 
  - Membuat bayangan di bawah tabel untuk efek 3D/elevation
  - `0` = tidak ada pergeseran horizontal
  - `4px` = pergeseran bayangan ke bawah
  - `10px` = tingkat blur (kehalusan bayangan)
  - `rgba(0, 0, 0, 0.1)` = hitam dengan transparansi 10%

#### 5. Styling Cell (Sel Tabel)
```css
th, td {
    padding: 12px;
    text-align: center;
}

th {
    background-color: #3498db;
    color: white;
    font-size: 16px;
}
```

**Penjelasan:**
- **`padding: 12px`**: Memberikan ruang kosong di sekitar teks dalam sel untuk keterbacaan
- **`th`** (header cell):
  - **`background-color: #3498db`**: Warna biru terang membedakan header dari data
  - **`color: white`**: Teks putih untuk kontras maksimal
  - **`font-size: 16px`**: Ukuran font yang jelas dan mudah dibaca

#### 6. Alternating Row Colors (Zebra Striping)
```css
tr:nth-child(even) {
    background-color: #f2f9ff;
}
```

**Penjelasan:**
- **`nth-child(even)`**: Selector CSS yang menargetkan baris genap (ke-2, ke-4, ke-6, dst.)
- **Efek Zebra Striping**: Warna bergantian pada setiap baris untuk mengurangi kelelahan mata saat membaca data panjang
- Meningkatkan komfortabilitas visual dan scannability (kemudahan pemindaian)

#### 7. Hover Effect (Interaktivitas)
```css
tr:hover {
    background-color: #d6ecff;
    transition: 0.3s;
}
```

**Penjelasan:**
- **`:hover`**: Pseudo-class yang merespons ketika user mengarahkan mouse ke baris
- **`background-color: #d6ecff`**: Warna berubah menjadi biru sedikit lebih gelap
- **`transition: 0.3s`**: Animasi perubahan warna selama 0.3 detik untuk efek smooth (halus) alih-alih perubahan langsung
- **Manfaat UX**: Memberikan feedback visual bahwa baris interaktif/dapat dipilih

#### 8. Footer Styling
```css
footer {
    margin-top: 30px;
    padding: 10px;
    text-align: center;
    font-size: 14px;
    color: #555;
}
```

**Penjelasan:**
- **`margin-top: 30px`**: Jarak antara tabel dan footer
- **`color: #555`**: Warna abu-abu gelap untuk de-emphasize (mengurangi penekanan) informasi footer
- **`font-size: 14px`**: Ukuran lebih kecil untuk menunjukkan bahwa ini bukan informasi utama
- **`text-align: center`**: Konsistensi visual dengan elemen lain

---

### CSS External (style.css)

```css
p {
    color: #333;
    font-family: Verdana;
    font-size: 16px;
    text-align: center;
}
```

**Penjelasan:**
- **`color: #333`**: Warna abu-abu gelap untuk kontras tinggi dan keterbacaan
- **`font-family: Verdana`**: Font fallback jika sistem tidak memiliki Segoe UI
- **`font-size: 16px`**: Ukuran standar untuk teks body
- **`text-align: center`**: Memusatkan paragraf deskripsi

**Mengapa Dipisah?**
File CSS eksternal memudahkan:
- Pemeliharaan kode (modular)
- Reusability di halaman lain
- Kecepatan loading (caching browser)

---

### Skema Warna & Desain

| Elemen | Warna | Hex | Fungsi |
|--------|-------|-----|--------|
| Background | Biru Muda | #eef6fb | Latar belakang lembut, menyenangkan |
| Heading | Biru Gelap | #0a3d62 | Warna profesional, kontras tinggi |
| Table Header | Biru Terang | #3498db | Pembeda jelas antara header dan data |
| Striped Rows | Biru Sangat Muda | #f2f9ff | Alternasi halus untuk keterbacaan |
| Hover State | Biru Medium | #d6ecff | Feedback interaktif |

**Prinsip Desain:** Penggunaan palet biru monokromatik menciptakan tampilan yang kohesif dan profesional. Biru adalah warna yang menyampaikan kepercayaan dan stabilitas—tepat untuk profil akademik.

---

### Konsep CSS yang Digunakan

#### 1. **Responsive Design**
```css
.container {
    width: 85%;  
}
```
- Desain beradaptasi dengan ukuran layar berbeda (mobile, tablet, desktop)

#### 2. **Box Model**
```css
padding: 12px;   
margin: 30px;    
border-radius: 10px;  
```

#### 3. **Pseudo-Classes**
```css
tr:nth-child(even) { }   
tr:hover { }              
```
- Memberikan styling berdasarkan state/kondisi elemen

#### 4. **Transitions**
```css
transition: 0.3s;  
```
- Membuat perubahan visual lebih mulus dan engaging

#### 5. **Shadows & Depth**
```css
box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
```
- Menciptakan kedalaman visual (elevation) tanpa menggunakan border tebal

---

### Responsive Behavior

**Viewport Meta Tag:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- `width=device-width`: Halaman menyesuaikan dengan lebar perangkat
- `initial-scale=1.0`: Dimulai pada zoom 100% (bukan zoom out)

**Keuntungan:** Halaman terlihat baik di smartphone tanpa user perlu zoom manual.

**Catatan:** Untuk layar sangat kecil (< 320px), tabel mungkin memerlukan horizontal scroll. Ini dapat ditingkatkan dengan media queries untuk stacking kolom pada mobile.

---

### Aksesibilitas & Best Practices

✅ **Semantic HTML**: Penggunaan `<h1>`, `<table>`, `<footer>` yang benar
✅ **Color Contrast**: Teks gelap pada latar terang memenuhi standar WCAG
✅ **Font Readability**: Font sans-serif modern (Segoe UI) optimal untuk layar
✅ **Responsive Meta Tag**: Mendukung tampilan yang baik di mobile
✅ **Meaningful Markup**: Struktur tabel yang jelas dengan `<th>` untuk header

**Saran Peningkatan:**
- Tambahkan `<thead>`, `<tbody>` untuk semantik tabel yang lebih baik
- Implementasi media queries untuk responsive design yang lebih lengkap
- Gunakan `aria-labels` untuk aksesibilitas screen reader

---

💡 Catatan

Proyek ini dibuat sebagai latihan dasar dalam memahami HTML dan CSS sebelum masuk ke tahap pengembangan web yang lebih kompleks.
Dengan proyek ini, diharapkan mahasiswa mampu memahami dasar pembuatan tampilan web serta penggabungan berbagai jenis CSS dalam satu halaman.

Penjelasan detail di atas mencakup:
- 🔍 Analisis setiap elemen HTML dan fungsinya
- 🎨 Teknik CSS yang digunakan dan alasan penggunaan
- 📐 Prinsip desain dan responsivitas
- ♿ Best practices aksesibilitas
- 💡 Tips cara kerja browser dan optimasi
