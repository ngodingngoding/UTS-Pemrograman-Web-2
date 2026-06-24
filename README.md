|Nama|NIM|Kelas|Mata Kuliah|
|----|---|-----|------|
|**Arbi Bagaskara Putra**|**312310671**|**I241D**|**Pemrograman Web 2**|

# UAS Pemrograman Web 2

## Identitas Mahasiswa

| Nama                 | NIM       | Kelas | Mata Kuliah       |
| -------------------- | --------- | ----- | ----------------- |
| Arbi Bagaskara Putra | 312310671 | I241D | Pemrograman Web 2 |

---

# Sistem Manajemen Inventaris Barang (E-Inventory)

Aplikasi ini merupakan proyek Ujian Akhir Semester (UAS) Pemrograman Web 2 yang dibangun menggunakan arsitektur **Decoupled Architecture**, yaitu memisahkan Backend API dan Frontend SPA.

## Teknologi yang Digunakan

### Backend

* PHP CodeIgniter 4
* RESTful API
* MySQL / MariaDB
* Resource Controller
* Filter Token Authentication
* CORS Filter

### Frontend

* VueJS 3
* Vue Router
* Axios
* TailwindCSS
* LocalStorage Authentication

---

# Struktur Repository

```
UAS_Web2_312310671_ArbiBagaskaraPutra
│
├── backend-api/
│
├── frontend-spa/
│
├── Screenshots/
│
└── README.md
```

---

# Struktur Database

Database menggunakan relasi beberapa tabel:

* users
* kategori
* barang
* supplier

### Relasi Database

Tambahkan screenshot berikut:

```
Screenshots/database-relasi.png
```

![Relasi Database](Screenshots/database-relasi.png)

---

# REST API

Endpoint yang tersedia:

| Method | Endpoint     | Fungsi                  |
| ------ | ------------ | ----------------------- |
| GET    | /barang      | Menampilkan data barang |
| POST   | /barang      | Menambah data           |
| PUT    | /barang/{id} | Mengubah data           |
| DELETE | /barang/{id} | Menghapus data          |
| POST   | /login       | Login administrator     |

---

# Proteksi Token (401 Unauthorized)

API menggunakan Authorization Bearer Token.

Screenshot pengujian API gagal melalui Postman:

```
Screenshots/postman-401.png
```

![401 Unauthorized](Screenshots/postman-401.png)

---

# Tampilan Aplikasi

## Halaman Login

```
Screenshots/login.png
```

![Login](Screenshots/login.png)

---

## Dashboard Administrator

```
Screenshots/dashboard.png
```

![Dashboard](Screenshots/dashboard.png)

---

## Form Tambah/Edit Data

```
Screenshots/modal-tambah.png
```

![Form Tambah](Screenshots/modal-tambah.png)

---

## Tabel Data Barang

```
Screenshots/tabel-data.png
```

![Data Barang](Screenshots/tabel-data.png)

---

# Fitur Aplikasi

## Public User

* Melihat halaman beranda
* Melihat ringkasan data

## Administrator

* Login
* Dashboard
* Menambah data
* Mengedit data
* Menghapus data
* Logout

---

# Sistem Keamanan

### Backend

* Filter Authorization Bearer Token
* CORS Configuration

### Frontend

* Vue Router Navigation Guard
* LocalStorage Token
* Axios Request Interceptor
* Axios Response Interceptor (401 Unauthorized)

---

# Cara Menjalankan Backend

Masuk ke folder backend:

```bash
cd backend-api
```

Install dependency:

```bash
composer install
```

Konfigurasi database pada file:

```
.env
```

Jalankan server:

```bash
php spark serve
```

Server berjalan pada:

```
http://localhost:8080
```

---

# Cara Menjalankan Frontend

Masuk ke folder:

```bash
cd frontend-spa
```

Jalankan menggunakan XAMPP atau Live Server.

Frontend berjalan pada:

```
http://localhost
```

---

# Demo Proyek

Link Demo:

```
https://<isi-link-demo>
```

---

# Video Presentasi

Link YouTube:

```
https://youtube.com/<isi-link-video>
```

---

# Screenshot Tambahan

Folder Screenshots berisi:

* Relasi Database
* Error 401 Postman
* Halaman Login
* Dashboard Admin
* Form Tambah/Edit
* Tabel Data Barang

---

# Kesimpulan

Aplikasi E-Inventory berhasil dibangun menggunakan CodeIgniter 4 sebagai REST API dan VueJS 3 sebagai Single Page Application (SPA). Sistem telah menerapkan autentikasi token, routing, serta antarmuka modern menggunakan TailwindCSS sesuai dengan ketentuan UAS Pemrograman Web 2.


