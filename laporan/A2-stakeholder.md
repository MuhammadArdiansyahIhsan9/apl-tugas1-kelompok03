# A2. Stakeholder dan Peta Power/Interest

<!-- Penanggung jawab: [Muhammad Ardiansyah Ihsan] -->

Layanan yang dianalisis adalah layanan nilai pada SIAKAD UMI, yaitu input nilai oleh dosen, pengesahan nilai, Kartu Hasil Studi (KHS), transkrip, dan sanggahan nilai. Daftar stakeholder berikut disusun dari fungsi layanan dan menu yang terlihat pada SIAKAD (Nilai KHS dan Nilai Transkrip). Stakeholder, kebutuhan, dan penilaian *power/interest* di bawah ini adalah **hasil analisis penulis dan belum diverifikasi** melalui wawancara maupun dokumen resmi UMI. Hasil wawancara (R1 dan seterusnya) akan menjadi bahan untuk mengonfirmasi atau mengoreksinya.

## 2.1 Stakeholder register

| No | Stakeholder | Kelompok | Peran pada layanan nilai | Kebutuhan utama | Ekspektasi kualitas | Prioritas |
| :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | Mahasiswa | Pengguna akhir | Melihat KHS dan transkrip, serta mengajukan sanggahan nilai | Nilai yang benar dan terbit tepat waktu; jalur sanggahan yang jelas | Mudah digunakan (*usability*), tetap dapat diakses saat banyak mahasiswa membuka nilai bersamaan (*availability*), data pribadi terlindungi (*security*) | Sedang |
| 2 | Dosen pengampu | Pengguna akhir | Memasukkan nilai mata kuliah dan menanggapi sanggahan | Input nilai cepat dan mudah dikoreksi sebelum disahkan; bukti nilai yang sudah diinput | Mudah digunakan (*usability*), data tidak hilang atau berubah tanpa jejak (*integrity*), hanya dosen pengampu yang dapat mengubah nilainya (*security*) | Sedang |
| 3 | Tim pengembang SIAKAD | Tim pengembang | Membangun dan memelihara fitur nilai | Kebutuhan dan aturan penilaian yang jelas; fitur nilai dapat diubah tanpa mengganggu fitur lain | Mudah dipelihara (*maintainability*) dan mudah diuji (*testability*) | Tinggi |
| 4 | Unit teknologi informasi kampus | Tim operasional | Menjalankan, memantau, dan mencadangkan sistem | Sistem stabil saat nilai terbit; gangguan cepat terdeteksi dan dipulihkan; data dicadangkan | Ketersediaan (*availability*), keamanan (*security*), kemudahan pemulihan (*recoverability*) | Tinggi |
| 5 | Biro akademik | Manajer bisnis | Mengelola data dan laporan akademik, termasuk keabsahan KHS dan transkrip | Nilai resmi konsisten di KHS dan transkrip; perubahan nilai terkendali dan tercatat | Keakuratan dan integritas data (*integrity*), jejak perubahan yang dapat ditelusuri (*auditability*) | Tinggi |
| 6 | Pihak pengesah nilai (ketua program studi atau dekan) | Manajer bisnis | Memeriksa dan mengesahkan nilai sebelum diterbitkan | Nilai yang diesahkan lengkap dan benar; ada catatan siapa mengesahkan dan kapan | Akuntabilitas (*accountability*), hak akses sesuai peran (*security*) | Sedang |
| 7 | Lembaga akreditasi dan auditor mutu | Pihak eksternal | Menilai mutu pengelolaan akademik dari data nilai | Data nilai tercatat, konsisten, dan dapat diaudit | Dapat diaudit (*auditability*) dan konsisten (*integrity*) | Rendah |

Keterangan prioritas: prioritas keterlibatan dalam pengembangan layanan, mengikuti kuadran pada Tabel 2.2. Prioritas rendah tidak berarti tidak penting, tetapi stakeholder tersebut tidak terlibat dalam keputusan sehari-hari.

Dasar penetapan stakeholder:
- **Mahasiswa**: menu Nilai KHS dan Nilai Transkrip terlihat pada tampilan SIAKAD. Kebutuhannya adalah asumsi analisis.
- **Dosen pengampu**: peran disebut pada deskripsi layanan di dokumen tugas ("input nilai oleh dosen"). Halaman input nilai belum terlihat, sehingga kebutuhannya adalah asumsi analisis.
- **Tim pengembang SIAKAD**: footer SIAKAD menampilkan "© 2014 Boegis Media". Itu hanya keterangan hak cipta dan tidak membuktikan siapa yang mengembangkan atau memelihara layanan nilai. Pihak yang berperan sebagai pengembang adalah asumsi analisis.
- **Unit teknologi informasi kampus**: asumsi analisis bahwa sistem yang dipakai seluruh mahasiswa dan dosen memiliki pengelola operasional. Nama unitnya belum terkonfirmasi.
- **Biro akademik**: asumsi analisis, karena KHS dan transkrip adalah dokumen akademik. Pembagian tugasnya di UMI belum terkonfirmasi.
- **Pihak pengesah nilai**: asumsi analisis dari tahap "pengesahan" pada deskripsi layanan. Bagian A1 laporan ini menyebut pengesahan oleh Kaprodi, tetapi hal itu belum diverifikasi. Pengesah sebenarnya (ketua program studi, dekan, atau pihak lain) perlu dikonfirmasi.
- **Lembaga akreditasi dan auditor mutu**: asumsi analisis, karena data nilai menjadi salah satu bukti mutu akademik.

## 2.2 Penilaian Power/Interest

*Power* dinilai dari kemampuan memengaruhi keputusan terhadap layanan, bukan dari jumlah pengguna. *Interest* dinilai dari seberapa besar stakeholder terdampak oleh layanan.

| No | Stakeholder | Power | Interest | Alasan | Kuadran dan strategi |
| :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | Mahasiswa | Rendah | Tinggi | Sangat terdampak oleh ketepatan nilai, tetapi tidak memutuskan rancangan atau aturan layanan. | *Keep Informed* |
| 2 | Dosen pengampu | Rendah | Tinggi | Bergantung pada layanan setiap semester, tetapi sebagai pengguna tidak menentukan rancangan sistem. | *Keep Informed* |
| 3 | Tim pengembang SIAKAD | Tinggi | Tinggi | Menentukan bagaimana fitur dibangun dan diubah, dan langsung terdampak oleh rancangan arsitektur. | *Manage Closely* |
| 4 | Unit teknologi informasi kampus | Tinggi | Tinggi | Menentukan lingkungan pelaksanaan dan keandalan sistem, dan langsung menangani gangguan. | *Manage Closely* |
| 5 | Biro akademik | Tinggi | Tinggi | Menentukan aturan nilai resmi dan keabsahan dokumen akademik, serta bergantung pada layanan ini. | *Manage Closely* |
| 6 | Pihak pengesah nilai | Tinggi | Rendah | Menentukan kapan nilai sah, tetapi diasumsikan hanya memakai layanan pada tahap pengesahan. | *Keep Satisfied* |
| 7 | Lembaga akreditasi dan auditor mutu | Tinggi | Rendah | Hasil penilaiannya berpengaruh pada institusi, tetapi tidak memakai layanan sehari-hari. | *Keep Satisfied* |

Penempatan stakeholder pada kuadran:

| | Interest rendah | Interest tinggi |
| :-- | :-- | :-- |
| **Power tinggi** | *Keep Satisfied*: pihak pengesah nilai; lembaga akreditasi dan auditor mutu | *Manage Closely*: tim pengembang SIAKAD; unit teknologi informasi kampus; biro akademik |
| **Power rendah** | *Monitor*: tidak ada stakeholder pada kuadran ini | *Keep Informed*: mahasiswa; dosen pengampu |

**Gambar 2.1.** Peta *power/interest* stakeholder layanan nilai SIAKAD UMI (hasil analisis penulis)

[GAMBAR BELUM TERSEDIA: berkas `diagram/A2-peta-power-interest.png` belum ada di repository. Sisipkan gambar di sini setelah tersedia, dengan tujuh stakeholder yang sama seperti Tabel 2.2.]

## 2.3 Strategi tiap kuadran

- ***Manage Closely* (tim pengembang SIAKAD, unit teknologi informasi kampus, biro akademik).** Dilibatkan dalam setiap keputusan arsitektur penting, termasuk saat keputusan dicatat dalam ADR. Kebutuhan mereka menjadi dasar utama kebutuhan arsitektur (A4).
- ***Keep Satisfied* (pihak pengesah nilai, lembaga akreditasi dan auditor mutu).** Tidak dilibatkan dalam pekerjaan harian. Mereka diberi ringkasan keputusan yang berkaitan dengan pengesahan, jejak perubahan, dan kemampuan audit, serta dimintai persetujuan atau masukan pada hal tersebut.
- ***Keep Informed* (mahasiswa, dosen pengampu).** Diberi informasi tentang perubahan layanan, jadwal penerbitan nilai, dan cara sanggahan. Umpan balik dikumpulkan secara berkala, misalnya melalui survei singkat.
- ***Monitor*.** Tidak ada stakeholder yang ditempatkan pada kuadran ini. Jika di kemudian hari ditemukan pihak lain dengan power dan interest rendah, cukup dipantau tanpa keterlibatan khusus.

## 2.4 Kesimpulan A2

Biro akademik, tim pengembang SIAKAD, dan unit teknologi informasi kampus adalah stakeholder yang paling memengaruhi kebutuhan dan keberhasilan layanan nilai, karena mereka menentukan aturan nilai dan menjaga layanan tetap andal. Mahasiswa dan dosen menentukan kebutuhan fungsional dari sisi penggunaan, tetapi tidak memutuskan rancangan. Seluruh klasifikasi di atas adalah asumsi analisis dan akan dikonfirmasi atau dikoreksi setelah wawancara dilakukan.
