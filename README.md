# Purwadhika-Capstone-2

## 🛒 Dekoruma CLI Furniture Store
Aplikasi belanja furnitur berbasis terminal (Command Line Interface) yang menyimulasikan proses belanja seperti toko online. Dibuat untuk latihan proyek Python dengan struktur modular dan interaktif.

## ✨ Fitur Utama

- Menyediakan **10 kategori produk** furnitur dan rumah tangga
- User dapat:
  - Melihat keranjang
  - Menambah produk
  - Menghapus item dari keranjang
  - Mengubah jumlah pembelian (qty)
  - Melakukan **checkout dan mencetak struk**
- Checkout menghasilkan **file struk `.txt` otomatis**

## 🚀 Cara Menjalankan

1. Clone repo ini
```
git clone
```
2. Install library yang dibutuhkan:
```
pip3 install tabulate, datetime, uuid
```
3. Jalankan program
```
python3 dekoruma.py
```

## ⚙️ Penjelasan Functions
menu_utama()
Fungsi utama program yang menampilkan menu:
1. Lihat Keranjang
2. Tambah Item
3. Hapus Item
4. Update Item
5. Checkout
6. Keluar program

### tampilkan_keranjang()
Menampilkan isi keranjang belanja

Jika kosong, tampilkan pesan peringatan

Menggunakan tabulate untuk menampilkan tabel rapi

## pilih_kategori()
Menampilkan semua kategori produk

User memilih salah satu kategori (0 untuk kembali)

Memanggil pilih_produk(kategori) berdasarkan pilihan

###pilih_produk(kategori)
Menampilkan daftar produk dalam suatu kategori

User memilih produk dan jumlah (qty) yang ingin dibeli

Produk akan ditambahkan ke dalam list keranjang

###hapus_item()
Menampilkan isi keranjang

Meminta user memilih nomor item untuk dihapus

Menghapus item dari list keranjang berdasarkan input

###update_item()
Menampilkan isi keranjang

Meminta user memilih item dan memasukkan qty baru

Memperbarui jumlah pembelian item yang dipilih

###checkout()
Menampilkan isi keranjang

Meminta konfirmasi user untuk lanjut checkout

Meminta input jumlah uang dari user

Mengecek apakah uang cukup

###Jika cukup:

Menampilkan dan menyimpan struk belanja ke .txt

Menghapus semua item di keranjang setelah checkout berhasil
