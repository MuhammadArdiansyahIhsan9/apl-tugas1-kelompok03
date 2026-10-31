# A2. Stakeholder dan Peta Power/Interest

## 2.1 Stakeholder register

| No | Stakeholder | Kelompok | Peran pada layanan nilai | Kebutuhan utama | Ekspektasi kualitas | Prioritas |
| :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | Mahasiswa | Pengguna akhir | Melihat KHS dan transkrip, mengajukan sanggahan nilai | Nilai yang benar dan terbit tepat waktu; jalur sanggahan yang jelas | Mudah digunakan (*usability*), tetap dapat diakses saat banyak mahasiswa membuka nilai bersamaan (*availability*), data pribadi terlindungi (*security*) | Sedang |
| 2 | Dosen pengampu | Pengguna akhir | Memasukkan nilai mata kuliah dan menanggapi sanggahan | Input nilai cepat dan mudah dikoreksi sebelum disahkan; bukti nilai yang sudah diinput | Mudah digunakan (*usability*), data tidak hilang atau berubah tanpa jejak (*integrity*), hanya dosen pengampu yang dapat mengubah nilainya (*security*) | Sedang |
| 3 | Tim pengembang SIAKAD | Tim pengembang | Membangun dan memelihara fitur nilai | Kebutuhan dan aturan penilaian yang jelas; fitur nilai dapat diubah tanpa mengganggu fitur lain | Mudah dipelihara (*maintainability*) dan diuji (*testability*) | Tinggi |
| 4 | Unit teknologi informasi kampus | Tim operasional | Menjalankan, memantau, dan mencadangkan sistem | Sistem stabil saat nilai terbit; gangguan cepat terdeteksi dan dipulihkan; data dicadangkan | Ketersediaan (*availability*), keamanan (*security*), kemudahan pemulihan (*recoverability*) | Tinggi |
| 5 | Biro akademik | Manajer bisnis | Mengelola data dan laporan akademik, termasuk keabsahan KHS dan transkrip | Nilai resmi konsisten di KHS dan transkrip; perubahan nilai terkendali dan tercatat | Keakuratan dan integritas data (*integrity*), jejak perubahan yang dapat ditelusuri (*auditability*) | Tinggi |
| 6 | Ketua program studi (Kaprodi) | Manajer bisnis | Memeriksa dan mengesahkan nilai sebelum diterbitkan | Nilai yang disahkan lengkap dan benar; ada catatan siapa mengesahkan dan kapan | Akuntabilitas (*accountability*), hak akses sesuai peran (*security*) | Sedang |


## 2.2 Penilaian Power/Interest

| No | Stakeholder | Power | Interest | Alasan | Kuadran |
| :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | Mahasiswa | Rendah | Tinggi | Sangat terdampak oleh ketepatan nilai, tetapi tidak memutuskan rancangan atau aturan layanan. | *Keep Informed* |
| 2 | Dosen pengampu | Rendah | Tinggi | Bergantung pada layanan setiap semester, tetapi sebagai pengguna tidak menentukan rancangan sistem. | *Keep Informed* |
| 3 | Tim pengembang SIAKAD | Tinggi | Tinggi | Menentukan bagaimana fitur dibangun dan diubah, dan langsung terdampak oleh rancangan arsitektur. | *Manage Closely* |
| 4 | Unit teknologi informasi kampus | Tinggi | Tinggi | Menentukan lingkungan pelaksanaan dan keandalan sistem, dan langsung menangani gangguan. | *Manage Closely* |
| 5 | Biro akademik | Tinggi | Tinggi | Menentukan aturan nilai resmi dan keabsahan dokumen akademik, serta bergantung pada layanan ini. | *Manage Closely* |
| 6 | Ketua program studi (Kaprodi) | Tinggi | Rendah | Menentukan kapan nilai sah, tetapi diasumsikan hanya memakai layanan pada tahap pengesahan. | *Keep Satisfied* |

