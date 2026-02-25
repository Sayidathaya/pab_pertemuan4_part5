# 🛒 Mini E-Commerce Shopping Cart (Flutter + Provider) 🚀

## 🎯 Gambaran Project

Project ini adalah implementasi aplikasi **Mini E-Commerce Shopping Cart** menggunakan **Flutter** dengan state management **Provider** 💙

Tujuan utama project ini adalah memahami bagaimana cara mengelola **state global** menggunakan `ChangeNotifier`, serta membangun fitur dasar keranjang belanja pada aplikasi mobile 📱

Pengguna dapat:

* 👀 Melihat daftar produk
* ➕ Menambahkan produk ke keranjang
* 🔢 Mengatur jumlah item
* ❌ Menghapus item
* 💰 Melihat total harga otomatis
* 🧾 Melakukan checkout sederhana

---

## ✨ Fitur Unggulan

Berikut fitur yang tersedia dalam aplikasi ini:

🧱 Model Product
🛍️ Model CartItem
🧠 CartModel dengan ChangeNotifier
📦 Halaman daftar produk
➕ Tombol Add to Cart
🔔 Badge jumlah item pada ikon cart
🛒 Halaman keranjang belanja
🔼🔽 Tambah & kurangi jumlah produk
🗑️ Hapus item dari keranjang
💵 Perhitungan total harga otomatis
📭 Pesan ketika keranjang kosong
✅ Simulasi checkout sederhana

---

## TAMPILAN

---

## 📁 Struktur Folder Project

```
lib/
│
├── models/
│   ├── product.dart
│   ├── cart_item.dart
│   └── cart_model.dart
│
├── pages/
│   ├── product_list_page.dart
│   └── cart_page.dart
│
└── main.dart
```

Struktur ini dibuat agar kode lebih rapi, modular, dan mudah dikembangkan ke depannya 🧩✨

---

## 🏗️ Penjelasan Arsitektur

### 🛍️ Product Model

Digunakan untuk merepresentasikan data produk seperti:

* ID
* Nama
* Harga
* Gambar
* Kategori

Model ini menjadi blueprint dari setiap produk yang ditampilkan 📦

---

### 🧾 CartItem Model

Berfungsi untuk menyimpan:

* Data produk yang dipilih
* Jumlah item

Selain itu, model ini juga memiliki properti untuk menghitung **total harga per item secara otomatis** 💰

---

### 🧠 CartModel (ChangeNotifier)

Ini adalah pusat pengelolaan state aplikasi 🔥

Tanggung jawabnya meliputi:

✔️ Menyimpan daftar item dalam cart
✔️ Menambahkan produk
✔️ Menghapus produk
✔️ Mengubah jumlah item
✔️ Menghitung total harga keseluruhan
✔️ Memberi notifikasi ke UI menggunakan `notifyListeners()`

Menggunakan struktur **Map** agar akses berdasarkan product ID lebih cepat dan efisien ⚡

---

## 🌍 State Management dengan Provider

`ChangeNotifierProvider` diletakkan di root aplikasi 🏠

Dengan cara ini:

* Semua halaman bisa mengakses state cart
* Tidak perlu kirim data manual antar widget (no prop drilling 😎)
* UI otomatis rebuild saat data berubah

State jadi lebih bersih, terstruktur, dan scalable 🚀

---

## ▶️ Cara Menjalankan Aplikasi

1️⃣ Clone repository atau copy source code
2️⃣ Jalankan perintah berikut:

```
flutter pub get
```

3️⃣ Jalankan aplikasi:

```
flutter run
```

Pastikan:

* Flutter SDK sudah terinstall ✅
* Emulator atau device sudah aktif 📱

---

## 📲 Cara Menggunakan Aplikasi

1️⃣ Buka aplikasi
2️⃣ Pilih produk di halaman utama
3️⃣ Tekan tombol **Add** untuk memasukkan ke cart
4️⃣ Tekan ikon 🛒 untuk membuka keranjang
5️⃣ Gunakan tombol ➕ atau ➖ untuk mengatur jumlah
6️⃣ Hapus item jika tidak diperlukan 🗑️
7️⃣ Tekan **Checkout** untuk simulasi pembelian 🎉

---

## 🧪 Pengujian Fungsional

Pengujian dilakukan secara manual dengan skenario berikut:

🔹 Menambahkan produk berulang kali
🔹 Menambahkan produk berbeda
🔹 Mengubah jumlah item
🔹 Menghapus item
🔹 Mengosongkan cart
🔹 Navigasi antar halaman

Hasilnya ✅
Semua fitur berjalan dengan baik dan state tetap sinkron di seluruh halaman 🎯

---

## 🎓 Kesimpulan

Project ini membuktikan bahwa **Provider + ChangeNotifier** adalah solusi yang sederhana namun powerful untuk mengelola state global pada Flutter 💪

Keunggulan yang didapat:

✨ UI otomatis update
✨ Struktur kode lebih terorganisir
✨ Mudah dikembangkan lebih lanjut (database, API, dll)
✨ Arsitektur lebih bersih dan scalable
