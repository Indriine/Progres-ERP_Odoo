Pada project ini saya melakukan implementasi sistem ERP Odoo untuk operasional toko roti.
# 1. Modul yang digunakan
- Sales
- Invoicing
- Purchase
- Inventory
- Manufacturing
# 2. Alur Operasional Toko Roti
- Pengadaan
  - Vendor --> PO -> Receipt -> Vendor Bill -> Payment
- Produksi
  - Manufacturing Order -> Produk Jadi
- Penjualan
  - Sales Order -> Kirim -> Customer Invoice -> Payment
# 3. Struktur Gudang
Gudang dibagi menjadi dua lokasi utama, yaitu:
1. Gudang Bahan Baku (Untuk menyimpan stok bahan baku)
2. Gudang Produk Jadi (Untuk menyimpan semua produk jadi (roti))
Struktur ini dibuat untuk memisahkan pergerakan bahan baku dan produk jadi agar tidak saling tercampur.




