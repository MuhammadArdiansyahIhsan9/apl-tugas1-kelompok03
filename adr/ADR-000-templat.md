# ADR-001: Riwayat nilai dan status nilai dikelola satu modul

<!-- Salin berkas ini menjadi ADR-001-judul-singkat.md, ADR-002-... dan seterusnya. -->

- **Status:** Diusulkan / Diterima / Digantikan oleh ADR-[001]
- **Tanggal:** [31-10-2026]
- **Pengambil keputusan:** [Muhammad Ardiansyah Ihsan]

## Context
 
Nilai melewati input oleh dosen, pengesahan, tampil di KHS dan transkrip, lalu dapat disanggah mahasiswa (ASR-01). Perubahan nilai setelah disahkan harus dapat dibuktikan (ASR-02). Cara SIAKAD mencatat perubahan nilai saat ini belum diketahui [DATA BELUM TERSEDIA]. Platform yang sudah ada (Gamelan ERP) tidak diasumsikan dapat diubah pada bagian inti (K-01).
 
## Decision
 
Kami akan menetapkan satu modul Pengelola Nilai sebagai satu-satunya jalur yang boleh mengubah nilai. Modul ini menyimpan status nilai (input, disahkan, dikoreksi) dan menulis catatan riwayat yang hanya dapat ditambah (append-only) setiap kali nilai berubah. KHS dan transkrip hanya membaca nilai berstatus disahkan.
 
## Consequences
 
- Untung: satu tempat untuk aturan status dan audit; sanggahan dan koreksi dapat dibuktikan; KHS dan transkrip konsisten.
- Rugi: semua fitur yang mengubah nilai harus lewat modul ini sehingga perlu penyesuaian; riwayat menambah kebutuhan penyimpanan; perubahan nilai sedikit lebih lambat karena ada penulisan riwayat.
## Compliance
 
- Tinjauan kode: tidak ada kode di luar Pengelola Nilai yang menulis ke data nilai.
- Uji (usulan angka): dari 50 perubahan nilai di lingkungan uji, 100% menghasilkan catatan riwayat lengkap; percobaan mengubah atau menghapus riwayat lewat aplikasi ditolak.
- Ditinjau setiap akhir semester.
