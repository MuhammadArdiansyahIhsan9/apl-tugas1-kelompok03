# A5. Keputusan Arsitektur dan ADR

Keputusan arsitektur pada Layanan Nilai di SIAKAD dibuat berdasarkan kebutuhan untuk menjaga keamanan, konsistensi, dan transparansi pengelolaan nilai akademik. Keputusan ini didokumentasikan dalam Architecture Decision Record (ADR).

## 1. Ringkasan Keputusan Arsitektur

| No. | ADR | Keputusan Arsitektur | Dasar Keputusan |
|---|---|---|---|
| 1 | ADR-001 | Riwayat Nilai dan Status Nilai Dikelola Satu Modul | Menjaga konsistensi data nilai serta memastikan setiap perubahan dapat ditelusuri. |
| 2 | ADR-002 | Otorisasi Dilakukan di Sisi Server Berdasarkan Identitas Sesi | Melindungi data nilai dengan memastikan pengguna hanya dapat mengakses data sesuai hak aksesnya. |

## 2. Detail Keputusan Arsitektur

| Komponen | ADR-001 | ADR-002 |
|---|---|---|
| Title | Riwayat Nilai dan Status Nilai Dikelola Satu Modul | Otorisasi Dilakukan di Sisi Server Berdasarkan Identitas Sesi |
| Status | Sesuai dokumen ADR-001 | Sesuai dokumen ADR-002 |
| Context | Nilai melewati proses input, pengesahan, penampilan pada KHS dan transkrip, serta sanggahan mahasiswa. Perubahan nilai harus dapat dibuktikan. | Halaman KHS dan transkrip memiliki isian NPM/NIM yang terikat pada akun login. Nilai merupakan data pribadi sehingga akses harus dibatasi. |
| Decision | Menggunakan satu modul Pengelola Nilai sebagai satu-satunya jalur perubahan nilai. Setiap perubahan dicatat dalam riwayat yang bersifat append-only. | Pemeriksaan hak akses dilakukan di sisi server berdasarkan identitas sesi login. Mahasiswa hanya dapat mengakses data miliknya, sedangkan dosen hanya dapat mengakses kelas yang diampunya. |
| Consequences | Nilai lebih konsisten dan perubahan dapat ditelusuri, tetapi membutuhkan penyimpanan riwayat tambahan. | Keamanan data lebih terjaga dan mengurangi risiko kebocoran data antarakun, tetapi setiap permintaan data membutuhkan pemeriksaan hak akses tambahan. |
| Compliance | Setiap perubahan nilai harus menghasilkan catatan riwayat. KHS dan transkrip hanya membaca nilai yang telah disahkan. | Pengujian dilakukan menggunakan akun uji. Sebanyak 30 permintaan data milik akun lain harus ditolak seluruhnya. Semua modul nilai wajib melewati komponen Otorisasi. |

## 3. Prioritas Keputusan

| No. | Keputusan | Prioritas | Alasan |
|---|---|---|---|
| 1 | Riwayat Nilai dan Status Nilai Dikelola Satu Modul | Tinggi | Menjamin konsistensi nilai dan memudahkan penelusuran perubahan nilai. |
| 2 | Otorisasi di Sisi Server Berdasarkan Identitas Sesi | Tinggi | Melindungi data akademik mahasiswa dari akses yang tidak berwenang. |

## 4. Dokumentasi ADR

Dokumen ADR lengkap disimpan dalam folder `adr/`, yaitu:

- ADR-001-templat.md
- ADR-002-templat.md

Setiap dokumen memuat Title, Status, Tanggal, Pengambil Keputusan, Context, Decision, Consequences, dan Compliance.
