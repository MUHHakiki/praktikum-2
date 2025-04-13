# Aplikasi Catatan Harian & Ramalan Cuaca

## Deskripsi Aplikasi
Aplikasi ini terdiri dari dua fitur utama, yaitu **Catatan Harian** dan **Ramalan Cuaca**. Pengguna dapat mencatat kegiatan atau pemikiran mereka setiap hari dengan menyimpan catatan dan menampilkannya di layar. Selain itu, pengguna juga dapat melihat ramalan cuaca berdasarkan nama kota yang dimasukkan, memanfaatkan API cuaca untuk mendapatkan informasi suhu dan kondisi cuaca terkini.

## Fitur-Fitur Aplikasi
1. **Catatan Harian**:
   - Menyediakan area untuk menulis catatan harian.
   - Menyimpan catatan yang dimasukkan ke dalam **localStorage** agar dapat diakses kembali setelah aplikasi dimuat ulang.
   - Fitur untuk menghapus catatan yang sudah ada.

2. **Ramalan Cuaca**:
   - Mengambil data cuaca secara langsung melalui **OpenWeather API** berdasarkan nama kota yang dimasukkan.
   - Menampilkan suhu dan kondisi cuaca kota yang dimasukkan oleh pengguna.
   - Menangani kesalahan jika kota tidak ditemukan atau API gagal merespon.

## Screenshot Aplikasi
![Screenshot Aplikasi](https://github.com/MUHHakiki/praktikum-2/blob/main/Screenshot%202025-04-13%20221141.png)

*Gambar ini menunjukkan antarmuka aplikasi yang sudah jadi, dengan fitur Catatan Harian di atas dan Ramalan Cuaca di bawah.*

## Daftar Fitur ES6+ yang Diimplementasikan
Aplikasi ini menggunakan berbagai fitur modern JavaScript (ES6+) untuk meningkatkan efisiensi dan kemudahan pengembangan. Berikut adalah fitur-fitur utama yang digunakan:

1. **Class ES6**:
   - Penggunaan **Class** untuk objek **Catatan Harian** yang memudahkan pengelolaan catatan dan interaksi dengan DOM.
   - Fungsi dan properti dalam class diimplementasikan menggunakan sintaks **arrow function** (`() => {}`) untuk menjaga konteks `this` yang konsisten.

2. **Fetch API**:
   - Digunakan untuk mengambil data dari **OpenWeather API** secara asinkron menggunakan metode **`fetch`** dan menangani **Promise** dengan **`async/await`**.
   - Menangani error dengan **`try...catch`** untuk memastikan aplikasi tetap responsif meskipun terjadi kesalahan saat mengambil data dari API.

3. **LocalStorage**:
   - Catatan harian disimpan menggunakan **`localStorage`**, sehingga data dapat dipertahankan bahkan setelah halaman direfresh.
   - Data diserialisasi dan dide-serialisasi menggunakan **`JSON.parse()`** dan **`JSON.stringify()`**.

4. **Template Literals**:
   - Penggunaan **template literals** (`` `${variable}` ``) untuk membuat string dinamis, terutama untuk menampilkan teks yang menggabungkan variabel dan HTML, seperti menampilkan data cuaca.

5. **Arrow Functions**:
   - Fungsi ditulis dengan menggunakan sintaks **arrow function** untuk meningkatkan kebersihan kode dan menghindari masalah dengan `this`.

6. **Destructuring**:
   - Penggunaan **destructuring** pada objek, khususnya saat mengambil data dari response API cuaca (misalnya, `const { main, weather } = data;`).

7. **Event Listeners**:
   - Penggunaan **`addEventListener`** untuk menangani interaksi pengguna (klik tombol, input teks, dll) secara asinkron dan terpisah dari DOM, meningkatkan pemeliharaan kode.

8. **CSS Animations**:
   - Implementasi **CSS animations** dengan **keyframes** untuk membuat efek berkedip pada elemen seperti judul halaman.

## Instruksi Penggunaan
1. **Clone repository** ini ke dalam folder proyek Anda.
2. Pastikan Anda memiliki file `index.html`, `app.js`, dan `styles.css` yang terhubung dengan benar.
3. Buka file `index.html` di browser untuk menjalankan aplikasi.
4. Gunakan fitur **Catatan Harian** untuk menulis dan menyimpan catatan.
5. Gunakan fitur **Ramalan Cuaca** dengan memasukkan nama kota dan menampilkan informasi cuaca terkini.

## Lisensi
Aplikasi ini dibuat untuk tujuan edukasi dan pengembangan pribadi. Dapat digunakan, diubah, dan dibagikan sesuai dengan ketentuan yang berlaku.

---

Terima kasih telah menggunakan aplikasi ini!
