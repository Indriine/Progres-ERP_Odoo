# Alur Proses #
# 1. MODUL PURCHASE
mengelola pembelian bahan baku dari vendor.
1. Create Vendor
   - Masuk ke menu "Purchase - Vendor - Create"
   - Isi nama, email, nomor telepon.
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
mengelola proses produksi roti
1. Buat Bill of Materials (BoM)
   - Manufacturing - Products - Bill of Materials - New
   - Pilih produk jadi (Roti Tawar)
   - Tambahkan bahan baku (Tepung 1kg, Ragi 10g, dll)
   - Centang BoM Type: Manufacture this product
   - Save
2. Manufacturing Order (MO)
   - Manufacturing - Operations - Manufacturing Orders - Create
   - Pilih produk jadi
   - Isi quantity (misal: 10 roti)
   - Sistem otomatis hitung bahan baku yang dibutuhkan dari BoM
   - Klik "Confirm"
3. Proses Produksi
   - Klik "Produce All" untuk mulai
   - Sistem otomatis:
     - Kurangi stok bahan baku (modul Inventory)
     - Tambah stok produk jadi (modul Inventory)
# 4. MODUL SALES
mengelola pesanan dan penjualan ke pelanggan.
1. Buat Customer
   - Sales - Customers - Create
   - Isi nama pelanggan
   - Save
2. Buat Sales Order (SO)
   - Sales - Orders - Quotations - New
   - Pilih customer
   - Tambahkan produk (Roti Tawar, Roti Manis)
   - Isi quantity
   - Klik "Confirm"
3. Proses Pengiriman
   - Setelah SO confirm, Delivery Order otomatis dibuat
   - Setelah barang dikirim klik "Validate"
4. Buat Invoice
   - Di SO klik "Create Invoice"
   - Pilih "Regular Invoice", lalu klik "Create Draft"
   - Klik "Confirm" dan "Pay", setelah itu klik "Create Payment"
   - Klik "Send" untuk otomatis terkirim ke email customer atau klik "Print" untuk mengunduh PDF.
# 5. MODUL INVOICING
membuat dan mengelola faktur penjualan/pembelian
A. Customer Invoice (Piutang)
1. Lihat Semua Invoice
   - Invoicing - Customers - Invoices
   - Untuk melihat daftar invoice yang sudah dibuat dari Sales
2. Validasi Invoice
   - Buka invoice yang status "Draft"
   - Klik "Confirm
   - Klik "Validate"
   - Status berubah jadi "Posted"
3. Terima Pembayaran
   - Buka invoice yang sudah "Posted"
   - Klik "Pay"
   - Pilih metode pembayaran (Tunai/Transfer)
   - Klik "Create Payment"
   - Status invoice jadi "Paid"
B. Vendor Bill
1. Lihat Vendor Bills
   - Invoicing - Vendors - Bills
   - Untuk melihat tagihan yang dibuat dari Purchase
2. Bayar ke Vendor
   - Buka Vendor Bill yang sudah "Posted"
   - Klik "Pay" lalu klik "Create Payment"
   - Status invoice jadi "Paid"
