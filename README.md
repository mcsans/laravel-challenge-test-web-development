# 💻 Laravel Challenge Test – Web Development

## 🎯 Tujuan

Challenge ini bertujuan untuk menguji kemampuan peserta dalam membangun aplikasi web sederhana menggunakan **Laravel**, dengan implementasi dasar seperti **routing**, **controller**, **view**, serta fitur **CRUD (Create, Read, Update, Delete)** menggunakan modal.

---

## 📝 Deskripsi Tantangan

Silakan buat sebuah aplikasi web sederhana menggunakan **Laravel** dengan ketentuan berikut:

### 1. Halaman Home

- **URL**: `/`
- Menampilkan teks **"Hello World"**.

### 2. Halaman User

- **URL**: `/users`
- Menyediakan fitur **CRUD** (Create, Read, Update, Delete) untuk data user.
- Struktur data user minimal terdiri dari:
  - `id` (auto increment)
  - `name` (string)
  - `email` (string, unique)
  - `password` (string)
  - `created_at` dan `updated_at` (timestamp)

#### Fitur halaman:
- Tampilkan data user dalam bentuk **tabel**.
- Tambah dan edit user dilakukan melalui **modal form (popup)**.
- Tampilkan notifikasi saat operasi berhasil (opsional: toastr, sweetalert, dsb).

---

## ⚙️ Ketentuan Teknis

- Gunakan **Laravel versi terbaru** yang stabil.
- Gunakan **Blade template engine**.
- Modal form dapat menggunakan **Bootstrap Modal** atau pustaka sejenis.
- Data disimpan di database (boleh menggunakan SQLite/MySQL).
- **Buat branch baru dari repository ini dengan nama sesuai nama Anda** (contoh: `johndoe`) lalu push semua hasil pengerjaan ke branch tersebut.

---

## 📦 Bonus (Opsional)

- Validasi form saat menambah dan mengedit user.
- Gunakan **Laravel Resource Controller** untuk manajemen user.
- Gunakan **pagination** jika data user lebih dari 10.