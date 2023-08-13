# SAP-Technology
Business of SAP Technology

1.	Bisnis Proses serta point utama :
Flowchart Proses Pembelian Material PT PMI ke PT Radial melalui Tokopedia sesuai SAP:
	[Start] Memulai proses.
	[Proses] Permintaan Pembelian:
	Departemen yang membutuhkan barang mengajukan permintaan pembelian melalui sistem SAP
	[Proses] Pengadaan Penyedia (TOKOPEDIA) sesuai SAP
	[Proses] Pesanan Pembelian:
	Pesanan pembelian seperti item no, nama, quantity, unit price, uom
	[Proses] Konfirmasi Pengiriman melalui ekspedisi TIKI/JNE:
	[Proses] Konfirmasi Pembayaran melalui Bank Transfer atau GOPAY
	[Proses] Pengiriman barang ke PT PMI
	[Proses] Barang diterima oleh PT PMI ada proses cheking ke MM dan WM di SAP dan di catat dalam system SAP PT PMI melaui Barcode TIKI / JNE yang dapat merekap raws material yang sudah diterima sesuai lokasi gudang, item number, Qty, unit price dan UOM
	[End] Proses berakhir.
Flow Chart Bisniss :
 

2.	Test Scenario
a.	Skenario: Permintaan Pembelian
Deskripsi: Menguji apakah sistem mampu menerima dan memproses permintaan pembelian yang diajukan oleh PT PMI.
Langkah-langkah:
-	Ajukan permintaan pembelian dengan detail barang dan kuantitas melalui sistem SAP.
-	Periksa apakah sistem berhasil menerima permintaan dengan benar.
b.	Skenario: Pembelian dari e-commers Tokopedia
Deskripsi: Menguji alur pembelian raws materials sesuai SAP di Tokopedia
Langkah-langkah:
-	Melakukan order permintaan pembelian raws material sesuai SAP
-	Pilih ekspedisi TIKI/SAP
-	Pilih metode pembayaran GOPAY/Bank Transfer
Periksa apakah sistem mengirim notifikasi dan memproses persetujuan dengan benar.
c.	Skenario: Konfirmasi Pengiriman dan Penerimaan Barang
Deskripsi: Menguji alur konfirmasi pengiriman dari Tokopedia dan penerimaan barang oleh PT PMI.
Langkah-langkah:
-	Pesanan sampai dan dapat dicek detail pesanan memalalui barcode yang tertera di TIKI/JNE
-	Cek apakah pesanan yang diterima sama mengirimkan konfirmasi pengiriman melalui sistem SAP.
PT PMI menerima barang dan mencatat penerimaan melalui sistem.
Periksa apakah sistem berhasil mencatat konfirmasi dan penerimaan dengan benar.
d.	Skenario: Pemeriksaan Kualitas
Deskripsi: Menguji apakah sistem mampu mengintegrasikan pemeriksaan kualitas barang yang diterima melalui Module MM dan VM di SAP
Langkah-langkah:
-	PT PMI melakukan pemeriksaan kualitas terhadap barang yang diterima.
-	PT PMI melakukan pemeriksaan terhadap kwitansi

3.	Scripts Test
https://docs.google.com/spreadsheets/d/1jAcljkCOqkTbrgCLl4qQh39lgbOp34oWpJA9Epd_3p4/edit?usp=sharing

4.	Model – model test case yang dapat dilakukan
a.	Pengujian Fungsional:
Pengujian fungsional adalah pengujian yang dilakukan untuk memverifikasi apakah setiap fungsi dalam sistem SAP berjalan sesuai dengan spesifikasi dan kebutuhan bisnis. Ini mencakup pengujian berdasarkan skenario penggunaan, alur kerja, dan kebijakan bisnis.
b.	Pengujian Integrasi:
Pengujian integrasi melibatkan pengujian interoperabilitas dan integrasi antara berbagai modul atau komponen dalam sistem SAP. Ini memastikan bahwa data dan proses dapat berjalan dengan benar di seluruh modul yang terkait.
c.	Pengujian End-to-End:
Pengujian end-to-end adalah pengujian yang melibatkan seluruh alur kerja proses bisnis dari awal hingga akhir. Tujuannya adalah memverifikasi apakah semua komponen dan sistem terintegrasi dengan baik dan berfungsi sesuai harapan.
d.	Pengujian Performa:
Pengujian performa bertujuan untuk mengukur kinerja dan respons sistem SAP dalam situasi beban yang berbeda. Ini melibatkan pengujian beban (load testing), pengujian kecepatan (stress testing), dan pengujian stabilitas (stability testing) untuk memahami sejauh mana sistem dapat menangani beban kerja yang berbeda.
e.	Pengujian Keamanan:
Pengujian keamanan dilakukan untuk memastikan bahwa sistem SAP memiliki langkah-langkah keamanan yang memadai dan melindungi data serta proses bisnis dari ancaman. Ini melibatkan pengujian penetrasi, pengujian kerentanan, dan pengujian otorisasi.
f.	Pengujian Regresi:
Pengujian regresi dilakukan setelah perubahan atau pembaruan sistem SAP. Tujuannya adalah memastikan bahwa perubahan tersebut tidak mempengaruhi fungsi-fungsi yang sudah ada sebelumnya. Ini melibatkan pengujian skenario sebelumnya setelah ada perubahan.
g.	Pengujian Penerimaan Pengguna (UAT):
Pengujian penerimaan pengguna melibatkan pengguna akhir atau pihak yang terlibat dalam bisnis untuk menguji sistem SAP dengan skenario kasus nyata. Ini memastikan bahwa sistem sesuai dengan harapan pengguna dan kebutuhan bisnis.

