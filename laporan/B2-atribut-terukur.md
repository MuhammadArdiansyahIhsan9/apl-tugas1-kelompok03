# B2. Atribut Kualitas yang Terukur
## 1. Definisi Atribut Kualitas

Atribut kualitas adalah ukuran suatu karakteristik yang menunjukkan kemampuan sistem dalam memenuhi kebutuhan pengguna. Setiap atribut memiliki indikator ukur yang objektif untuk menilai kualitas Layanan Nilai di SIAKAD.

## 2. Individu Atribut (Indikator Ukur)

| Individu Atribut | Definisi | Indikator Ukur | Target |
|---|---|---|---|
| Time Response | Kecepatan sistem dalam merespons permintaan pengguna. | Waktu membuka halaman nilai, KHS, dan transkrip. | < 2 detik |
| Turnaround Time | Waktu yang dibutuhkan sampai suatu proses selesai. | Waktu dari input nilai hingga tersimpan. | < 5 detik |
| Throughput | Jumlah transaksi yang dapat diproses dalam satu waktu. | Jumlah transaksi penyimpanan nilai per detik. | > 10 transaksi/detik |
| Availability | Persentase waktu sistem tersedia untuk digunakan. | Uptime dibandingkan total waktu operasional. | >= 99% |
| Data Integrity | Kemampuan menjaga keutuhan dan konsistensi data. | Persentase data nilai yang tersimpan sesuai input. | 100% |
| Resource Utilization | Penggunaan sumber daya sistem. | Penggunaan CPU dan memori saat pengujian. | < 70% rata-rata |
| Interoperability | Kemampuan sistem berkomunikasi dengan sistem lain. | Keberhasilan pertukaran data melalui API. | 100% pengujian integrasi berhasil |
| Portability | Kemampuan sistem digunakan pada berbagai platform. | Keberhasilan akses melalui browser dan perangkat berbeda. | 100% platform uji dapat mengakses sistem |

## 3. Dua Kategori Perilaku dan Empat Kategori Produk

### 3.1 Dua Kategori Perilaku

| Kategori | Definisi | Contoh Layanan Nilai di SIAKAD |
|---|---|---|
| Perilaku yang Dibatasi | Tingkat perilaku sistem yang memiliki batas atau standar tertentu. | Waktu membuka KHS maksimal 2 detik dan ketersediaan sistem minimal 99%. |
| Perilaku yang Diminta | Tingkat perilaku yang diharapkan oleh pengguna. | Nilai tersimpan secara akurat, pengesahan berjalan lancar, dan notifikasi sanggahan dapat diterima mahasiswa. |

### 3.2 Empat Kategori Produk

| Kategori | Definisi | Contoh Layanan Nilai di SIAKAD |
|---|---|---|
| Functional Suitability | Kemampuan fitur dalam memenuhi fungsi yang dibutuhkan. | Input nilai, pengesahan, KHS, transkrip, dan sanggahan nilai. |
| Performance Efficiency | Kinerja sistem dalam menggunakan sumber daya. | Waktu respons membuka nilai dan KHS kurang dari 2 detik. |
| Compatibility | Kemampuan sistem bekerja dengan teknologi lain. | Integrasi REST API dengan layanan akademik lainnya. |
| Usability | Kemudahan sistem digunakan oleh pengguna. | Tampilan mudah dipahami oleh dosen, admin, dan mahasiswa. |
| Reliability | Kemampuan sistem bekerja secara konsisten. | Data nilai tetap konsisten dan tidak hilang saat proses penyimpanan. |
| Security | Kemampuan melindungi data dari akses tidak sah. | Login, enkripsi HTTPS, dan pembatasan hak akses menggunakan RBAC. |
| Maintainability | Kemudahan sistem diperbaiki dan dikembangkan. | Pemisahan modul input nilai, pengesahan, KHS, transkrip, dan sanggahan. |
| Portability | Kemampuan sistem digunakan pada berbagai lingkungan. | Dapat diakses melalui komputer, laptop, dan smartphone. |

## 4. Tiga Atribut Kualitas Pendorong

| Atribut Kualitas | Angka Target | Kondisi Pengukuran | Cara Mengukur |
|---|---|---|---|
| Performance | Waktu respons maksimal 2 detik. | Ketika dosen dan mahasiswa mengakses layanan secara bersamaan. | Mengukur waktu yang dibutuhkan sistem untuk membuka halaman nilai, KHS, dan transkrip. |
| Security | 100% pengujian hak akses berhasil sesuai peran. | Ketika dosen, admin, dan mahasiswa mencoba mengakses fitur masing-masing. | Menguji login dan memastikan pengguna tidak dapat mengakses fitur di luar kewenangannya. |
| Reliability | 100% data nilai yang berhasil disimpan tetap konsisten. | Ketika proses input, pengesahan, koreksi, dan penampilan nilai dilakukan. | Membandingkan data sebelum dan sesudah proses serta memeriksa riwayat perubahan nilai. |



