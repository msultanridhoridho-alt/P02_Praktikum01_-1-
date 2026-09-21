## Bagian F — Checkpoint proyek

**1. Dimensi dan Satuan Data**
- Dataset ini memiliki **1.212 baris** dan **11 kolom**.
- **Satuan baris:** Satu baris merepresentasikan satu riwayat transaksi penjualan.

**2. Pengelompokan Tipe Kolom**
- **Tanggal:** `tanggal`
- **Numerik:** `jumlah`, `harga_satuan`, `diskon_persen`, `rating_pelanggan`, `total_bayar`
- **Kategorikal:** `id_transaksi`, `kota`, `kategori`, `produk`, `metode_bayar`

**3. Masalah pada Data**
- **Data Kosong:** Terdapat data yang hilang (null) pada kolom `rating_pelanggan` dan `metode_bayar`.
- **Tipe Data Salah:** Kolom `tanggal` masih dibaca sebagai teks, seharusnya diubah ke format waktu (datetime).
- **Nilai Tidak Konsisten:** Penulisan nama kota berantakan karena perbedaan huruf besar/kecil (contoh: "Depok" dan "DEPOK"), serta ada salah ketik tahun pada awalan `id_transaksi`.

**4. Kecukupan Data**
- **Sudah cukup** jika analisis tim berfokus pada tren penjualan produk, kategori terlaris, atau efektivitas metode pembayaran.
- **Belum cukup** jika tim ingin menghitung profit/keuntungan bersih (karena tidak ada data Harga Pokok Penjualan/modal) atau menganalisis loyalitas pembeli (karena tidak ada ID Pelanggan).
