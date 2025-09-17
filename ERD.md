+----------------+           +----------------+           +------------------+
|    Anggota     |           |   Peminjaman   |           |       Buku       |
+----------------+           +----------------+           +------------------+
| PK ID_Anggota  |1         N| PK ID_Peminjaman|N        1| PK ID_Buku       |
|    Nama        |-----------| FK ID_Anggota  |-----------|    Judul         |
|    Email       |           | FK ID_Buku     |           |    Pengarang     |
|    No_Telp     |           | Tgl_Pinjam     |           |    Penerbit      |
|    Alamat      |           | Tgl_Jatuh_Tempo|           |    Tahun_Terbit  |
| Tanggal_Daftar |           | Tgl_Kembali    |           |    Kategori      |
+----------------+           | Status        |           |    Jumlah_Stok   |
                             +----------------+           +------------------+
