

1.Arsitektur Sistem  
Menggunakan arsitektur client-server berbasis web. Frontend berbasis React.js, backend menggunakan Node.js dan Express, database menggunakan MySQL.

2.Diagram Komponen  
- Frontend: UI untuk anggota dan staf (React.js)  
- Backend API: Endpoint untuk operasi CRUD dan autentikasi (Node.js/Express)  
- Database: MySQL untuk penyimpanan data buku, anggota, dan transaksi

3.Desain Database  
Tabel:  
- anggota (ID_Anggota PK, Nama, Email, No_Telp, Alamat, Tanggal_Daftar)  
- buku (ID_Buku PK, Judul, Pengarang, Penerbit, Tahun_Terbit, Kategori, Jumlah_Stok)  
- peminjaman (ID_Peminjaman PK, ID_Anggota FK, ID_Buku FK, Tanggal_Pinjam, Tanggal_Jatuh_Tempo, Tanggal_Kembali, Status)

4.Alur Proses  
1. Anggota login  
2. Cari buku  
3. Pilih buku dan lakukan peminjaman (jika stok tersedia)  
4. Sistem menyimpan transaksi peminjaman  
5. Anggota mengembalikan buku pada waktu yang ditentukan  
6. Sistem update status peminjaman menjadi "Dikembalikan"

5.Interface Pengguna  
- Form pendaftaran anggota  
- Dashboard pencarian dan daftar buku  
- Form peminjaman dan pengembalian buku  
- Panel manajemen data untuk staf  

6.Keamanan  
- Autentikasi pengguna menggunakan JWT  
- Validasi input di frontend dan backend  
- Backup data database secara berkala  

