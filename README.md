Pada project ini saya melakukan implementasi sistem ERP Odoo untuk operasional toko roti. Tujuan implementasi ini adalah untuk mengintegrasikan proses pembelian bahan baku, produksi roti, manajemen stok, hingga penjualan dalam satu sistem yang terstruktur dan terdokumentasi.
Implementasinya meliputi:
- Pembelian bahan baku
- Produksi roti
- Manajemen stok
- Penjualan produk
# 1. Modul yang digunakan
- Sales: Untuk mengelola pesanan dan penjualan ke pelanggan. 
- Invoicing: Untuk membuat dan mengelola faktur penjualan/pembelian.
- Purchase: Untuk mengelola pembelian bahan baku dari vendor.
- Inventory: Untuk mengelola stok dan pergerakan barang.
- Manufacturing: Untuk mengelola proses produksi roti.
# 2. Alur Operasional Toko Roti
- Pengadaan
  - Vendor --> PO -> Receipt -> Vendor Bill -> Payment
- Produksi
  - Manufacturing Order -> Produk Jadi
- Penjualan
  - Sales Order -> Kirim -> Customer Invoice -> Payment

**Penjelasan:**
1. Bahan baku (tepung, gula, dll) dibeli ke vendor melalui modul purchase.
2. Barang diterima dan masuk ke stok gudang (Inventory).
3. Produksi roti dilakukan melalui manufacturing order berdasarkan Bill of Materials yang sudah dibuat.
4. Produk jadi masuk ke stok barang jadi.
5. Penjualan dilakukan melalui sales order.
6. Sistem menghasilkan delivery order dan mengurangi stok barang jadi.
7. Sistem menghasilkan invoice yang harus divalidasi dan juga dicatat sebagai piutang.
8. Pelanggan melakukan pembayaran untuk menutup piutang.
# 3. Struktur Gudang
Gudang dibagi menjadi dua lokasi utama untuk memisahkan pergerakan bahan baku dan produk jadi agar tidak saling tercampur.
1. Gudang Bahan Baku (Untuk menyimpan stok bahan baku pembuatan roti)
   - Tepung terigu - satuan: kg
   - Ragi - satuan: g
   - Gula - satuan: kg
   - Mentega - satuan: kg
2. Gudang Produk Jadi (Untuk menyimpan semua produk roti yang sudah di produksi)
   - Roti tawar - satuan: unit
   - Roti manis - satuan: unit
# 4. Berikut beberapa fitur yang telah diimplementasikan
1. Pembuatan Bill of Materials untuk Roti Tawar dan Roti Manis
2. Sinkronisasi Server Email (SMTP Gmail) 
3. Replenishment rule pada produk jadi untuk otomatis membuat Manufacturing Order (produksi) saat stok menipis
4. Proses pembelian bahan baku
5. Proses penerimaan barang (Receipt)
6. Proses produksi menggunakan Manufacturing Order
7. Proses penjualan dan delivery












