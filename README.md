Praktikum 3 — CSS Dasar

## Identitas Praktikum

- **Nama:** Mu’ammar Kadafi
- **NIM:** 312510192
- **Program Studi/Semester:** Teknik Informatika / 3
- **Mata Kuliah:** Pemrograman Web
- **Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom.
- **Kelas:** I253C
- **Hari/Tanggal:** Sabtu, 10 Oktober 2026
- **Pertemuan:** 4 (Offline)

## Tujuan Praktikum

Praktikum ini bertujuan untuk mempelajari penerapan CSS dasar pada dokumen HTML, termasuk CSS internal, inline, dan eksternal. Praktikum juga mengenalkan penggunaan selector elemen, ID, dan class serta memahami bagaimana aturan CSS diterapkan pada elemen HTML.

## Langkah-Langkah Praktikum

1. Mempersiapkan text editor, misalnya Visual Studio Code.
2. Membuat folder kerja dengan nama `praktikum-3-css-dasar`.
3. Membuat file HTML dengan nama `lab2_css_dasar.html`.
4. Menyusun struktur HTML untuk menampilkan data mahasiswa dan membuka file tersebut di browser untuk melihat hasilnya.
5. Menambahkan deklarasi CSS internal di dalam elemen `<style>` pada bagian `<head>`. Pada tahap ini, CSS digunakan untuk mengatur jenis huruf pada halaman, tinggi minimum header, garis bawah header, ukuran dan warna judul, perataan teks, serta jarak di sekitar judul.
6. Menambahkan CSS inline pada elemen paragraf menggunakan atribut `style`. Deklarasi tersebut digunakan untuk mengatur perataan dan warna teks paragraf secara langsung pada elemen HTML.
7. Membuat file CSS eksternal bernama `style_eksternal.css`.
8. Menuliskan deklarasi CSS eksternal untuk mengatur tampilan navigasi, termasuk warna latar belakang, warna teks, jarak bagian dalam, tampilan tautan, dan perubahan tampilan ketika kursor diarahkan ke tautan.
9. Menghubungkan file `style_eksternal.css` ke dokumen HTML dengan elemen `<link>` pada bagian `<head>`.
10. Menambahkan ID selector dan class selector pada file CSS eksternal. ID selector digunakan untuk mengatur tampilan bagian dengan ID `intro`, termasuk latar belakang, garis tepi, tinggi minimum, dan jarak bagian dalam. Selector `#intro h1` digunakan untuk mengatur judul yang berada di dalam bagian tersebut.
11. Menambahkan class selector `.button` untuk mengatur tampilan tautan agar menyerupai tombol, lalu menggunakan `.btn-primary` untuk memberikan tampilan khusus pada tombol utama.
12. Menyimpan perubahan dan membuka atau memuat ulang dokumen HTML di browser untuk memeriksa hasil penerapan CSS internal, inline, dan eksternal.

## Eksperimen CSS

Eksperimen dilakukan dengan mengubah dan menambahkan properti serta nilai CSS pada file `style_eksternal.css`. Properti yang dapat dicoba meliputi warna latar belakang (`background`), warna teks (`color`), jarak dalam (`padding`), jarak luar (`margin`), garis tepi (`border`), ukuran teks (`font-size`), perataan teks (`text-align`), sudut membulat (`border-radius`), bayangan (`box-shadow`), serta efek ketika kursor diarahkan ke tautan (`:hover`). Setelah perubahan disimpan, hasilnya diamati melalui browser untuk membandingkan tampilan sebelum dan sesudah eksperimen.

## Jawaban Pertanyaan Praktikum

### 1. Apa perbedaan deklarasi CSS `h1 { ... }` dengan `#intro h1 { ... }`?

Deklarasi CSS `h1 { ... }` digunakan untuk memberikan gaya pada semua elemen HTML `<h1>` yang terdapat dalam halaman web. Sementara itu, deklarasi CSS `#intro h1 { ... }` digunakan untuk memberikan gaya hanya pada elemen `<h1>` yang berada di dalam elemen HTML dengan atribut `id="intro"`. Perbedaannya terletak pada cakupan penerapan gaya. Selector `h1` berlaku untuk seluruh elemen `<h1>`, sedangkan selector `#intro h1` lebih spesifik karena hanya menargetkan elemen `<h1>` di dalam elemen dengan ID `intro`. Dengan demikian, tampilan judul pada bagian tertentu dapat diatur tanpa memengaruhi judul lainnya di halaman web.

### 2. Jika CSS internal, eksternal, dan inline diterapkan pada elemen yang sama, deklarasi manakah yang ditampilkan?

Deklarasi CSS yang diterapkan pada browser ditentukan oleh prioritas, spesifisitas, dan urutan aturan CSS. Pada contoh sederhana ketika ketiga deklarasi mengatur properti yang sama dan tidak ada aturan khusus seperti `!important`, CSS inline umumnya memiliki prioritas lebih tinggi daripada CSS internal dan eksternal.

Sebagai contoh, CSS eksternal mengatur warna paragraf menjadi biru, CSS internal mengatur warna menjadi hijau, dan CSS inline mengatur warna menjadi merah. Hasilnya, teks paragraf ditampilkan dengan warna merah karena nilai warna ditentukan langsung pada atribut `style` elemen tersebut. Namun, aturan `!important`, spesifisitas, dan mekanisme cascade juga dapat memengaruhi hasil akhirnya.

### 3. Jika sebuah elemen memiliki ID dan class, selector manakah yang diprioritaskan?

Jika ID selector dan class selector mengatur properti yang sama pada elemen yang sama, ID selector umumnya diprioritaskan karena memiliki tingkat spesifisitas lebih tinggi daripada class selector.

Contohnya, sebuah paragraf memiliki `id="paragraf-1"` dan `class="text-paragraf"`. Jika selector `#paragraf-1` menetapkan warna biru dan ukuran teks 20 piksel, sedangkan selector `.text-paragraf` menetapkan warna merah dan ukuran teks 16 piksel, paragraf akan berwarna biru dengan ukuran teks 20 piksel. Hal tersebut terjadi karena spesifisitas ID selector lebih tinggi daripada class selector, selama tidak ada aturan lain yang mengubah hasil cascade.

## Struktur Berkas

Struktur berkas praktikum yang digunakan adalah sebagai berikut:

- `praktikum-3-css-dasar/`
  - `lab2_css_dasar.html` — dokumen HTML untuk menampilkan konten praktikum.
  - `style_eksternal.css` — stylesheet eksternal untuk mengatur tampilan navigasi, bagian pengenalan, dan tombol.

## Hasil Praktikum

Praktikum menghasilkan halaman web sederhana yang menerapkan CSS internal, inline, dan eksternal. Tampilan halaman dapat diatur melalui selector elemen, ID, dan class. Perubahan properti CSS dapat diamati melalui browser setelah berkas disimpan.
