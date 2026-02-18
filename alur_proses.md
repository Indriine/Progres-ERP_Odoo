# Alur Proses #
# 1. MODUL PURCHASE
mengelola pembelian bahan baku dari vendor.
1. Create Vendor
   - Masuk ke menu "Purchase - Vendor - Create"
   - Isi nama, alamat, email, nomor telepon.
   - Save.
2. Buat PO
   - Purchase - Orders - Requests for Quotation - New
   - Tambahkan produk bahan baku (Tepung, Gula, dll)
   - Isi quantity dan harga
   - Klik "Confirm Order"
3. Buat Bill Vendor
   - Dari PO, klik "Create Bill"
   - Klik Confirm, lalu create payment
# 2. MODUL INVENTORY
mengelola stok dan pergerakan barang.
1. Cek Stok
   - Inventory - Reporting - Stok
   - Untuk melihat semua produk bahan baku dan produk jadi
2. Terima Barang
   - Inventory - Operations - Receipts
   - Akan muncul otomatis dari PO yang sudah dikonfirmasi
3. Kirim Barang
   - Inventory → Operations → Delivery Orders
   - Otomatis muncul dari Sales Order
4. Pindah Stok
   - Inventory → Operations → Internal Transfers
   - Digunakan jika perlu memindahkan barang antar gudang
# 3. MODUL MANUFACTURING

1. MODUL SALES
- Questions (Masih dalam bentuk draft, contohnya saat kita memasukan barang ke keranjang)
- Orders (Pesanan sudah tervalidasi dan siap dikirim/ditagih)
Alur pemesanan:
- Question New (masukan nama pembeli dan barang yang mau di beli(add product) - bar other info/warehouse (diubah ke - Gudang produk jadi)) lalu klik confirm.
- Klik delivery (gambar mobil) - semuanya di validate
- Setelah validate (klik order) dan lakukan pembayaran (create invoice) lalu payment.




