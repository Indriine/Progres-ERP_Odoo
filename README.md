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

**Penjelasan:**
1. Bahan baku (tepung, gula, dll) dibeli melalui modul Purchase.
2. Barang diterima dan masuk ke stok gudang (Inventory).
3. Produksi roti dilakukan melalui Manufacturing Order berdasarkan Bill of Materials.
4. Produk jadi masuk ke stok barang jadi.
5. Penjualan dilakukan melalui Sales Order.
6. Sistem menghasilkan Delivery Order dan mengurangi stok barang jadi.
# 3. Struktur Gudang
Gudang dibagi menjadi dua lokasi utama, yaitu:
1. Gudang Bahan Baku (Untuk menyimpan stok bahan baku pembuatan roti)
   - Tepung terigu
   - Ragi
   - Gula
   - Mentega
2. Gudang Produk Jadi (Untuk menyimpan semua produk roti yang sudah di produksi)
   - Roti tawar
   - Roti manis
Struktur ini dibuat untuk memisahkan pergerakan bahan baku dan produk jadi agar tidak saling tercampur.






