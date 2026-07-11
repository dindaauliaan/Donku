Product Requirement Design

Donku (LadyBakeshop Finance)

- Product Overview

Donku adalah aplikasi berbasis web yang membantu pemilik usaha donat dalam mencatat pemasukan dan pengeluaran secara digital, menghitung saldo secara otomatis, serta memberikan informasi laba/rugi dan laporan keuangan agar pemilik usaha dapat mengambil keputusan berdasarkan data.

- Problem Statement

- Pembelian bahan secara mendadak sering tidak tercatat
- Perhitungan masih manual menggunakan kalkulator sehingga ada kemungkinan salah hitung
- Owner kesulitan mengetahui laba sebenarnya karna :

Gaji setiap lapak berbeda tanggal, Pembelian bahan tidak terjadwal sehingga menyebabkan muncul perasaan banyak pengeluaran besar muncul di hari yg berbeda

- Tidak ada dashboard kondisi usaha. Owner harus membuka buku catatan satu per satu.

- Goals & Succeess Metrics

- Membantu owner mengetahui kondisi keuangan usaha secara real-time.
- Mengurangi pencatatan manual.
- Menghitung saldo dan laba otomatis.

- Target Users
- User Persona
- Functional Requirements
- \[FR-01\] Login

**Deskripsi**

Sistem menyediakan halaman login untuk mengautentikasi pengguna sebelum mengakses aplikasi.

**Tujuan**

Menjaga keamanan data keuangan agar hanya dapat diakses oleh pengguna yang memiliki akun.

**Acceptance Criteria**

- Pengguna dapat login menggunakan email dan password.
- Jika data benar, pengguna diarahkan ke halaman Dashboard.
- Jika data salah, sistem menampilkan pesan kesalahan.
- Pengguna dapat logout dari aplikasi.

- \[FR-02\] Tambah pemasukan.

### Deskripsi

Pengguna dapat mencatat setiap transaksi pemasukan yang berasal dari hasil penjualan donat.

### Tujuan

Mencatat seluruh pemasukan agar sistem dapat menghitung saldo dan laba secara otomatis.

### Data yang Diinput

- Tanggal transaksi
- Nominal pemasukan
- Keterangan (opsional)
- Outlet/Lapak (opsional untuk pengembangan multi-lapak)

### Acceptance Criteria

- Data pemasukan berhasil disimpan.
- Saldo bertambah secara otomatis.
- Dashboard langsung memperbarui total pemasukan.
- Transaksi muncul pada riwayat transaksi.

- \[FR-03\] Tambah pengeluaran.

### Deskripsi

Pengguna dapat mencatat setiap pengeluaran usaha seperti pembelian bahan baku, pembayaran gaji, operasional, maupun pengeluaran lainnya.

### Tujuan

Mengurangi kemungkinan lupa mencatat pengeluaran serta membantu mengetahui arus kas usaha secara akurat.

### Data yang Diinput

- Tanggal
- Kategori pengeluaran
- Nominal
- Keterangan
- Foto struk (opsional pada MVP, bisa dikembangkan nanti)

### Acceptance Criteria

- Pengeluaran berhasil disimpan.
- Saldo otomatis berkurang.
- Dashboard memperbarui total pengeluaran.
- Riwayat transaksi menampilkan data yang baru ditambahkan.

- \[FR-04\] Kategori transaksi.

### Deskripsi

Setiap transaksi pengeluaran dikelompokkan berdasarkan kategori tertentu agar memudahkan analisis keuangan.

### Tujuan

Membantu owner mengetahui sumber pengeluaran terbesar setiap periode.

### Contoh Kategori

- Bahan Baku
- Gaji Karyawan
- Operasional
- Peralatan
- Transportasi
- Lain-lain

### Acceptance Criteria

- Pengguna wajib memilih kategori saat menambah pengeluaran.
- Sistem dapat mengelompokkan transaksi berdasarkan kategori.
- Data kategori digunakan pada laporan dan dashboard.

- \[FR-05\] Perhitungan saldo otomatis.

### Deskripsi

Sistem menghitung saldo usaha secara otomatis berdasarkan seluruh transaksi pemasukan dan pengeluaran yang telah dicatat.

### Tujuan

Menghilangkan proses perhitungan manual menggunakan kalkulator.

### Acceptance Criteria

- Saldo berubah setiap terdapat transaksi baru.
- Tidak diperlukan perhitungan manual.
- Saldo selalu sesuai dengan data transaksi.

- \[FR-06\] Perhitungan laba/rugi otomatis.

### Deskripsi

Sistem menghitung laba atau rugi berdasarkan selisih antara total pemasukan dan total pengeluaran dalam periode tertentu.

### Tujuan

Membantu owner mengetahui kondisi usaha secara cepat tanpa harus menghitung sendiri.

### Tampilan

- Hijau apabila laba positif.
- Merah apabila mengalami kerugian.

### Acceptance Criteria

- Laba diperbarui secara otomatis setiap ada transaksi.
- Pengguna dapat melihat laba harian maupun bulanan.
- Dashboard menampilkan status Untung atau Rugi.

- \[FR-07\] Dashboard

### Deskripsi

Dashboard merupakan halaman utama yang menampilkan ringkasan kondisi keuangan usaha secara real-time.

### Tujuan

Memberikan informasi penting yang dapat dipahami hanya dengan sekali melihat.

### Informasi yang Ditampilkan

- Total pemasukan hari ini
- Total pengeluaran hari ini
- Saldo saat ini
- Laba/Rugi hari ini
- Ringkasan pengeluaran berdasarkan kategori
- Riwayat transaksi terbaru

### Acceptance Criteria

- Data diperbarui secara otomatis setelah transaksi disimpan.
- Informasi mudah dipahami.
- Tampilan responsif di desktop maupun mobile.

- \[FR-08\] Laporan harian.

### Deskripsi

Sistem menyediakan laporan transaksi harian yang berisi seluruh pemasukan dan pengeluaran pada tanggal tertentu.

### Tujuan

Memudahkan owner melakukan evaluasi kondisi usaha setiap hari.

### Informasi

- Total pemasukan
- Total pengeluaran
- Laba/Rugi
- Daftar transaksi

### Acceptance Criteria

- Pengguna dapat memilih tanggal.
- Sistem menampilkan seluruh transaksi pada tanggal tersebut.
- Total dihitung otomatis.

- \[FR-09\] Laporan bulanan.

### Deskripsi

Sistem menyediakan rekapitulasi transaksi selama satu bulan.

### Tujuan

Membantu owner mengetahui perkembangan usaha dari bulan ke bulan.

### Informasi

- Total pemasukan
- Total pengeluaran
- Total laba/rugi
- Pengeluaran berdasarkan kategori
- Grafik sederhana (opsional MVP)

### Acceptance Criteria

- Pengguna dapat memilih bulan dan tahun.
- Data dihitung otomatis.
- Informasi ditampilkan dalam bentuk tabel.

- \[FR-10\] Export PDF.

### Deskripsi

Pengguna dapat mengunduh laporan keuangan dalam format PDF.

### Tujuan

Memudahkan penyimpanan, pencetakan, atau pembagian laporan kepada pihak lain.

### Acceptance Criteria

- Pengguna memilih periode laporan.
- Sistem menghasilkan file PDF.
- PDF berisi ringkasan keuangan beserta daftar transaksi.
- File dapat diunduh dan dicetak.

- Non Functional Requirements

- Responsive
- Data aman
- UX mudah dipahami pengguna

- User Flow
- Feature List (MVP)
- Future Features
- Data Requirements
- Technical Stack
- Timeline