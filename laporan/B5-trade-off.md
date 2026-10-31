### B5. Analisis Trade-off

| Aspek | Trade-off 1: Keamanan versus Kinerja | Trade-off 2: Integritas dan Auditability versus Kinerja |
|---|---|---|
| Mengapa Bentrok | Otorisasi diperiksa pada setiap permintaan (ADR-002), sehingga menambah waktu pemrosesan. | Setiap perubahan nilai mencatat riwayat (ADR-001), sehingga proses penulisan data membutuhkan waktu lebih lama. |
| Dampak | Waktu respons KHS dan transkrip sedikit meningkat, terutama ketika banyak pengguna mengakses sistem secara bersamaan. | Proses perubahan nilai secara massal oleh dosen menjadi sedikit lebih lambat. |
| Alternatif | (a) Pemeriksaan dilakukan sekali per sesi: lebih cepat, tetapi keamanan bergantung pada validitas sesi. (b) Menyimpan hasil pemeriksaan sementara. (c) Melakukan pemeriksaan pada setiap permintaan. | (a) Riwayat ditulis belakangan: lebih cepat, tetapi riwayat berisiko hilang jika terjadi kegagalan. (b) Menyimpan perubahan dan riwayat dalam satu transaksi. (c) Tidak mencatat riwayat perubahan. |
| Prioritas Dipilih | Keamanan lebih tinggi. | Integritas lebih tinggi. |
| Alasan | Nilai merupakan data pribadi mahasiswa sehingga kebocoran dapat menimbulkan dampak besar. Sementara itu, masalah kinerja belum terbukti karena ASR-04 masih berupa hipotesis. | Sanggahan dan koreksi nilai harus dapat dibuktikan melalui riwayat perubahan. Riwayat hanya dicatat ketika terjadi perubahan nilai, bukan ketika data dibaca. |
