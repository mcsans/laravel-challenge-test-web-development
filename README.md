# 💻 Laravel Challenge Test – Web Development

## 🎯 Tujuan

Challenge ini bertujuan untuk menguji kemampuan peserta dalam membangun aplikasi web sederhana menggunakan **Laravel**, dengan implementasi dasar seperti **routing**, **controller**, **view**, serta fitur **CRUD (Create, Read, Update, Delete)** menggunakan modal.

---

## 📝 Deskripsi Tantangan

Silakan buat sebuah aplikasi web **Manajemen Stok Produk (Product Stock Management)** sederhana menggunakan **Laravel** dengan ketentuan berikut:

### 1. Authentication

- Menggunakan Laravel Breeze / Jetstream / atau implementasi manual.
- Seluruh fitur hanya dapat diakses oleh user yang telah login (gunakan middleware `auth`).

### 2. CRUD User

- **URL:** `/users`
- Menyediakan fitur **CRUD** (Create, Read, Update, Delete) untuk data user.
- Struktur data minimal:
  - `id` (auto increment)
  - `name` (string)
  - `email` (string, unique)
  - `password` (string)
  - `created_at` dan `updated_at` (timestamp)

### 3. CRUD Product

- **URL:** `/products`
- Menyediakan fitur **CRUD** untuk data produk.
- Struktur data minimal:
  - `id` (auto increment)
  - `name` (string)
  - `category` (string)
  - `price` (integer)
  - `stock` (integer) – total stok produk saat ini
  - `description` (text)
  - `created_at` dan `updated_at` (timestamp)

### 4. Manajemen Stock

- **URL:** `/stock`
- Menyediakan fitur **CRUD** untuk manajemen stok produk.
- Struktur data minimal:
  - `id` (auto increment)
  - `user_id` (foreignId) – user yang melakukan perubahan stok
  - `product_id` (foreignId)
  - `stock` (integer) – nilai bisa positif (penambahan) atau negatif (pengurangan)
  - `created_at` dan `updated_at` (timestamp)

#### Fitur halaman:
- Tampilkan data dalam bentuk **tabel**.
- Tambah dan edit dilakukan melalui **modal form (popup)**.
- Tampilkan notifikasi saat operasi berhasil (opsional: toastr, sweetalert, dsb).

---

## ⚙️ Ketentuan Teknis

- Gunakan **Laravel versi terbaru** yang stabil.
- Gunakan **Blade template engine**.
- Modal form dapat menggunakan **Bootstrap Modal** atau pustaka sejenis.
- Data disimpan di database (boleh menggunakan SQLite/MySQL).
- **Fork repository ini** lalu push semua hasil pengerjaan ke github anda.

---

## 📦 Bonus (Opsional)

- Validasi form saat menambah dan mengedit data.
- Gunakan **Laravel Resource Controller** untuk manajemen controller.
- Gunakan **pagination** jika data user lebih dari 10.