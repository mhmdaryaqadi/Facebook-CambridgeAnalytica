<div align="center">

# LAPORAN INVESTIGASI PROJECT-BASED LEARNING (PBL)
## MATA KULIAH: ETIKA PROFESI 

<br>

### ANALISIS ETIKA DAN DAMPAK SOSIAL PELANGGARAN PRIVASI GLOBAL 
## "STUDI KASUS FACEBOOK–CAMBRIDGE ANALYTICA"

<br>

<img width="470" height="351" alt="image" src="https://github.com/user-attachments/assets/071a26bb-b0e8-410e-868b-fce1184ecc7d" />

<br>

### Disusun Oleh Kelompok 11:

| Nama Anggota | NPM |
| :--- | :--- |
| Muhammad Arya Alqadi | 4524210058 |
| Muzakki Abrar | 4524210071 |
| Muhammad Jibran Ferdian | 4524210067 |
| Muhammad Arkan | 4524210114 |
| Daffa Richadatul'Aisy | 4524210136 |

<br>

**Dosen Pengampu:**  
Adi Wahyu Pribadi, S.Si., M.Kom

<br>

## PROGRAM STUDI TEKNIK INFORMATIKA
## FAKULTAS TEKNIK UNIVERSITAS PANCASILA
## 2026

</div>

---

##  HEADER PEMETAAN SUB-CPMK

*   **Nomor Kelompok:** Kelompok 11
*   **Kasus Investigasi:** Eksploitasi Data Pengguna pada Kasus Facebook-Cambridge Analytica (Klaster D - Platform, Gig Economy & Dampak Sosial)
*   **Daftar Capaian Pembelajaran:** Sub-CPMK 1, Sub-CPMK 2, Sub-CPMK 3, Sub-CPMK 4, Sub-CPMK 5, Sub-CPMK 7, Sub-CPMK 8, dan Sub-CPMK 9
*   **Tautan Video Dokumentasi YouTube (Unlisted):** [Tautan video menyusul setelah proses rekaman selesai]

### Distribusi Peran dan Tanggung Jawab Segmen Laporan:
1.  **Muhammad Arya Alqadi (4524210058) - Ketua Kelompok:** Penanggung Jawab Integrasi Sistem, Penulisan Langkah 1 (Kronologi & Konteks Teknis), Langkah 7 (Analisis Regulasi & Hukum), dan Langkah 8 (Checkpoint Integritas & Anti-Korupsi).
2.  **Muzakki Abrar (4524210071):** Penulisan Langkah 2 (Fakta Kunci & Catatan Transparansi), Langkah 3 (Pemetaan Pemangku Kepentingan), dan Langkah 4 (Analisis Empat Teori Etika).
3.  **Muhammad Jibran Ferdian (4524210067):** Penulisan Langkah 5 (Lensa Kelima Pancasila) dan Langkah 6 (Kode Etik Profesi).
4.  **Muhammad Arkan (4524210114):** Penulisan Langkah 9 (Manajemen Risiko & Opsi 4T ISO 31000).
5.  **Daffa Richadatul'Aisy (4524210136):** Penulisan Langkah 10 (Rancangan Dampak & Kontrol Preventif) dan Langkah 11 (Pelajaran Utama & Daftar Pustaka).

---

## ANALISIS INVESTIGASI 

### 1. Kronologi & Konteks Teknis 


### 2. Fakta Kunci & Catatan Transparansi 


### 3. Pemetaan Pemangku Kepentingan & Relasi Kuasa 


### 4. Analisis Berdasarkan Empat Teori Etika Moral 


### 5. Lensa Kelima Pancasila & Nilai Luhur UP 


### 6. Kepatuhan Kode Etik Profesi Internasional 


### 7. Analisis Regulasi Yuridis & Yurisdiksi Hukum 


### 8. Checkpoint Integritas & Pencegahan Penyalahgunaan Kewenangan 


### 9. Manajemen Risiko Teknologi Berbasis Kerangka ISO 31000 

Analisis manajemen risiko ini disusun berdasarkan kerangka kerja standar ISO 31000 dengan menempatkan posisi kelompok sebagai tim evaluator arsitektur teknologi informasi pada platform penyedia data skala masif.

#### 9.1. Identifikasi dan Matriks Analisis Risiko
Proses identifikasi risiko difokuskan pada tiga ancaman struktural yang terjadi dalam ekosistem platform:

| ID Risiko | Deskripsi Ancaman Risiko | Probabilitas (1-5) | Dampak (1-5) | Tingkat Risiko (PxD) | Kesimpulan Status Risiko |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **R-01** | Kebocoran data agregat subjek pihak ketiga akibat pelonggaran otorisasi cakupan (*permission scopes*) pada endpoint API pihak ketiga. | 5 (Sangat Tinggi) | 5 (Katastropik) | 25 | **Critical (Ekstrim)** |
| **R-02** | Pelanggaran regulasi perlindungan data internasional akibat transaksi pemindahtanganan data ilegal oleh mitra pengembang eksternal. | 4 (Tinggi) | 5 (Katastropik) | 20 | **High (Tinggi)** |
| **R-03** | Penurunan nilai kapitalisasi pasar korporasi dan runtuhnya reputasi institusional akibat penundaan eksposur publik (*concealment of defect*). | 3 (Sedang) | 5 (Katastropik) | 15 | **High (Tinggi)**

#### 9.2. Formulasi Opsi Mitigasi Penanganan Risiko (Strategi 4T)
Berdasarkan hasil pemetaan matriks risiko di atas, formulasi opsi perlakuan risiko ditentukan melalui kerangka kerja 4T sebagai berikut:

*   **1. Terminate (Tinggalkan / Hentikan):** Diterapkan secara mutlak pada risiko **R-01**. Platform wajib menghentikan operasional fungsional Graph API versi 1.0 yang membuka akses data jaringan pertemanan melalui endpoint `user_friends`. Kebijakan otorisasi data harus didepridasi total untuk menghapus celah eksploitasi data pasif subjek pihak ketiga.

*   **2. Treat (Tangani / Mitigasi):** Diterapkan pada risiko **R-02**. Pengembang platform wajib mengimplementasikan kontrol preventif berupa pembatasan ketat autentikasi OAuth (*Scope Restriction*) hanya pada profil dasar dan alamat email resmi. Selain itu, wajib dilakukan penegakan prosedur *third-party monitoring* secara berkala melalui audit forensik digital terjadwal untuk memverifikasi kepatuhan penggunaan data oleh pengembang aplikasi eksternal.

*   **3. Transfer (Alihkan Risiko):** Diterapkan pada aspek tanggung jawab operasional hukum pengolahan data. Risiko hukum dialihkan melalui klausul hukum yang mengikat (*Developer Terms of Service*) yang secara eksplisit memindahkan tanggung jawab pidana dan ganti rugi perdata kepada pihak ketiga (pengembang aplikasi) apabila terbukti melakukan pemindahtanganan data komersial tanpa izin. Risiko finansial korporasi juga dialihkan melalui pemanfaatan instrumen asuransi siber (*cyber insurance*).

*   **4. Tolerate (Terima Risiko):** Diterapkan pada sisa risiko residu (*residual risk*) setelah kontrol teknis diterapkan, seperti risiko adanya erosi data minimal akibat interaksi normal antarmuka yang sah oleh pengguna. Risiko ini dapat ditoleransi karena berada dalam batas ambang batas risiko (*risk appetite*) operasional platform yang dibutuhkan untuk menjaga interkonektivitas ekosistem aplikasi.

### 10. Rancangan Dampak Sosial & Kontrol Preventif Rekayasa Perangkat Lunak 


### 11. Pelajaran Utama & Rujukan Pustaka 
