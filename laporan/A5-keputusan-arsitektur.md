# A5. Keputusan Arsitektur dan ADR
Keputusan arsitektur pada Layanan Nilai di SIAKAD dibuat berdasarkan kebutuhan untuk menjaga keamanan, konsistensi, dan transparansi pengelolaan nilai akademik. Keputusan ini didokumentasikan dalam Architecture Decision Record (ADR).

## 1. Ringkasan Keputusan Arsitektur

| No. | ADR | Keputusan Arsitektur | Dasar Keputusan |
|---|---|---|---|
| 1 | ADR-000 | Pembatasan Hak Akses Pengguna Berdasarkan Peran (RBAC) | Mengatur hak akses dosen, admin akademik, dan mahasiswa agar data nilai terlindungi. |
| 2 | ADR-001 | Riwayat Nilai dan Status Nilai Dikelola Satu Modul | Menjaga konsistensi data nilai serta memastikan setiap perubahan dapat ditelusuri. |

## 2. Detail Keputusan Arsitektur

| Komponen | ADR-000 | ADR-001 |
|---|---|---|
| Title | Pembatasan Hak Akses Pengguna Berdasarkan Peran (RBAC) | Riwayat Nilai dan Status Nilai Dikelola Satu Modul |
| Status | Diterima | Diterima |
| Context | Terdapat beberapa pengguna dengan tugas dan kewenangan berbeda dalam layanan nilai SIAKAD. | Nilai melewati proses input, pengesahan, penampilan pada KHS dan transkrip, serta sanggahan mahasiswa. Perubahan nilai harus dapat dibuktikan. |
| Decision | Menggunakan Role-Based Access Control (RBAC) untuk mengatur hak akses dosen, admin akademik, dan mahasiswa. | Menggunakan satu modul Pengelola Nilai sebagai satu-satunya jalur perubahan nilai. Setiap perubahan dicatat dalam riwayat yang bersifat append-only. |
| Consequences | Keamanan data lebih terjaga dan akses pengguna lebih terkontrol, tetapi membutuhkan pengelolaan hak akses. | Nilai lebih konsisten dan perubahan dapat ditelusuri, tetapi membutuhkan penyimpanan riwayat tambahan. |
| Compliance | Setiap pengguna wajib login dan hanya dapat mengakses fitur sesuai kewenangannya. | Setiap perubahan nilai harus menghasilkan catatan riwayat. KHS dan transkrip hanya membaca nilai yang telah disahkan. |

## 3. Prioritas Keputusan

| No. | Keputusan | Prioritas | Alasan |
|---|---|---|---|
| 1 | Pembatasan Hak Akses Pengguna (RBAC) | Tinggi | Melindungi data akademik mahasiswa dari akses yang tidak berwenang. |
| 2 | Pengelolaan Riwayat dan Status Nilai | Tinggi | Menjamin konsistensi nilai dan memudahkan penelusuran perubahan nilai. |

## 4. Dokumentasi ADR

Dokumen ADR lengkap disimpan dalam folder `adr/`, yaitu:

- ADR-000-templat.md
- ADR-001-templat.md

Setiap dokumen memuat Title, Status, Tanggal, Pengambil Keputusan, Context, Decision, Consequences, dan Compliance.

