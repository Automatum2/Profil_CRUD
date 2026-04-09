# Profil_CRUD
Membuat Halaman Profil yang menggunakan CRUD(Create Read Update Delete) 
Cara menjalankan : 
1.open terminal jalankan php artisan serve
2.buka localhost dan tambahkan /profiles di url 

struktur file yang terlibat: 
coba/
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── ProfileController.php      <-- (Logika Controller CRUD)
│   └── Models/
│       └── Profile.php                    <-- (Model Data)
│
├── database/
│   └── migrations/
│       └── ..._create_profiles_table.php  <-- (Struktur Tabel Database)
│
├── resources/
│   └── views/
│       ├── layouts/
│       │   └── app.blade.php              <-- (Kerangka Desain UI Utama)
│       └── profiles/
│           ├── index.blade.php            <-- (Halaman Tabel Data)
│           ├── create.blade.php           <-- (Halaman Form Tambah)
│           ├── edit.blade.php             <-- (Halaman Form Edit)
│           └── show.blade.php             <-- (Halaman Detail Profil)
│
└── routes/
    └── web.php                            <-- (Modifikasi Jalur/Rute URL)
