# B1. Identifikasi dan Klasifikasi Karakteristik

Karakteristik arsitektur menggambarkan kecenderungan perilaku sistem. Pada Layanan Nilai di SIAKAD, karakteristik dibagi menjadi tiga kategori, yaitu operasional, struktural, dan lintas sektor.

## 1. Karakteristik Operasional

Berkaitan dengan bagaimana sistem bekerja dalam lingkungan penggunaan sehari-hari.

| Karakteristik | Deskripsi | Implementasi Layanan Nilai di SIAKAD |
|---|---|---|
| Availability (Ketersediaan) | Sistem dapat diakses ketika dibutuhkan. | Sistem SIAKAD dapat diakses dosen, admin, dan mahasiswa melalui jaringan internet. |
| Continuity (Keberlangsungan) | Sistem tetap beroperasi dan menjaga proses layanan. | Data nilai, KHS, dan transkrip tetap tersimpan meskipun pengguna keluar dari sistem. |
| Performance (Kinerja) | Kecepatan sistem dalam merespons permintaan pengguna. | Menampilkan nilai, KHS, dan transkrip dalam waktu respons yang cepat. |
| Efficiency (Efisiensi) | Penggunaan sumber daya secara optimal. | Menggunakan query database yang efisien untuk menampilkan data nilai mahasiswa. |
| Supportability (Daya Dukung) | Kemudahan sistem dalam pemeliharaan dan perbaikan. | Menggunakan pencatatan error dan struktur modul agar kesalahan sistem mudah diperiksa. |

## 2. Karakteristik Struktural

Berkaitan dengan struktur internal sistem dan kemudahan pengembangan.

| Karakteristik | Deskripsi | Implementasi Layanan Nilai di SIAKAD |
|---|---|---|
| Configurability (Konfigurasi) | Sistem dapat diatur tanpa mengubah kode utama. | Pengaturan periode penginputan nilai dan batas waktu pengajuan sanggahan. |
| Extensibility (Ekstensibilitas) | Kemudahan menambahkan fitur baru. | Menambahkan fitur notifikasi nilai dan riwayat akademik tanpa mengubah keseluruhan sistem. |
| Modifiability (Kemudahan Modifikasi) | Sistem mudah diperbaiki atau diperbarui. | Memisahkan modul input nilai, pengesahan, KHS, transkrip, dan sanggahan. |
| Testability (Kemudahan Pengujian) | Sistem mudah diuji untuk memastikan fungsinya berjalan baik. | Melakukan pengujian pada proses input nilai, pengesahan, dan pengajuan sanggahan. |
| Reliability (Keandalan) | Sistem mampu bekerja secara konsisten. | Menggunakan transaksi database untuk menjaga konsistensi data nilai. |

## 3. Karakteristik Lintas Sektor

Berkaitan dengan kualitas sistem yang mendukung berbagai pengguna, platform, dan lingkungan.

| Karakteristik | Deskripsi | Implementasi Layanan Nilai di SIAKAD |
|---|---|---|
| Accessibility (Aksesibilitas) | Sistem dapat digunakan oleh berbagai pengguna. | Menyediakan tampilan yang mudah dipahami dan dapat diakses melalui komputer maupun smartphone. |
| Security (Keamanan) | Melindungi data dari akses yang tidak sah. | Menggunakan login, HTTPS, dan RBAC untuk membatasi hak akses pengguna. |
| Interoperability (Interoperabilitas) | Sistem dapat berkomunikasi dengan sistem lain. | Menggunakan REST API untuk pertukaran data dengan layanan akademik lainnya. |
| Environmental Quality (Kualitas Lingkungan) | Sistem dapat digunakan dalam lingkungan teknologi berbeda. | Mendukung berbagai browser dan perangkat dengan tampilan responsif. |

## 4. Prioritas Karakteristik

| Priority | Karakteristik | Alasan |
|---|---|---|
| 1 | Security | Data nilai merupakan informasi akademik mahasiswa yang harus dilindungi. |
| 2 | Reliability | Data nilai harus akurat dan konsisten agar tidak terjadi kesalahan pada KHS dan transkrip. |
| 3 | Performance | Sistem harus memberikan respons cepat ketika pengguna mengakses informasi nilai. |
| 4 | Availability | Sistem harus dapat diakses ketika dibutuhkan dosen, admin, dan mahasiswa. |
| 5 | Modifiability | Sistem harus mudah diperbaiki dan dikembangkan sesuai kebutuhan akademik. |
| 6 | Interoperability | Sistem perlu mendukung pertukaran data dengan layanan akademik lainnya. |


