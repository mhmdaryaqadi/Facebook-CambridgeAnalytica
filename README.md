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


### 10. Rancangan Dampak Sosial & Kontrol Preventif Rekayasa Perangkat Lunak 

Sebagai upaya preventif guna memitigasi pengulangan insiden kebocoran data terstruktur di masa depan, kelompok kami merumuskan rekomendasi kontrol teknis pada level arsitektur rekayasa perangkat lunak dan analisis dampaknya terhadap masyarakat sipil:

#### 10.1. Implementasi Arsitektur Teknik Preventif
Rekomendasi taktis berbasis standar rekayasa perangkat lunak modern difokuskan pada tiga pilar pertahanan data:

*   **1. Penerapan Metode Privacy by Design (PbD):** Pengembang sistem wajib mengintegrasikan perlindungan privasi sebagai fitur bawaan default pada siklus hidup pengembangan perangkat lunak (SDLC), bukan sebagai modul tempelan eksternal. Setiap rilis fitur baru wajib melewati tahapan pengujian *Privacy Impact Assessment* (PIA) guna mendeteksi potensi efek samping eksploitasi fungsional.
*   **2. Restriksi Cakupan Akses Otorisasi (Scope Restriction):** Protokol otentikasi pihak ketiga (seperti OAuth 2.0) wajib membatasi hak penarikan token akses pengembang eksternal. Akses API secara default hanya dibuka untuk parameter profil dasar publik (*basic profile*) dan alamat email valid, sedangkan hak akses terhadap jaringan pertemanan (*social graph endpoints*) dinonaktifkan secara menyeluruh demi melindungi hak subjek data pihak ketiga.
*   **3. Penerapan Prinsip Data Minimization:** Pada level perancangan basis data, skema penyimpanan data diatur secara ketat untuk hanya menyimpan atribut data yang mutlak diperlukan bagi fungsionalitas transaksi utama pengguna. Data yang tidak lagi memiliki relevansi operasional wajib melewati proses penghapusan otomatis (*data purging*) atau anonimisasi forensik tingkat tinggi agar tidak dapat direkonstruksi menjadi profil psikometrik jika terjadi kebocoran internal.

#### 10.2. Analisis Dampak Sosial Terhadap Masyarakat Sipil
Formulasi kontrol teknis di atas dirancang untuk memberikan dampak positif yang signifikan pada struktur sosial kemasyarakatan digital:
*   **Restorasi Otonomi Informasi Warga Negara:** Penerapan *Privacy by Design* mengenangkan kendali mutlak identitas digital ke tangan subjek data, sehingga meminimalisasi risiko manipulasi kognitif terselubung oleh pihak broker data politik.
*   **Reduksi Penyeberan Gelembung Informasi (Filter Bubbles):** Dengan tertutupnya akses data psikometri model OCEAN, agensi kampanye tidak lagi memiliki instrumen untuk menyusun narasi propaganda kognitif yang mengeksploitasi ketakutan personal. Dampak sosialnya adalah penurunan eskalasi polarisasi digital dan penguatan ketahanan kohesi masyarakat sipil dari ancaman disinformasi sistemik.

  
### 11. Pelajaran Utama & Rujukan Pustaka 

#### 11.1. Pelajaran Utama (Lessons Learned)
Investigasi komprehensif terhadap skandal Facebook-Cambridge Analytica memberikan pemahaman krusial bahwa integritas suatu sistem komputasi tidak hanya diukur dari kekuatan parameter teknisnya, melainkan dari ketahanan etika fungsional arsitekturnya. Kode pemrograman dan rancangan algoritma bukan sekadar baris perintah netral, melainkan instrumen kekuasaan sosial yang memiliki dampak multiplikasi terhadap stabilitas demokrasi, hak asasi privasi, dan keadilan sosial di tengah masyarakat digital.

#### 11.2. Refleksi Mandiri Rencana Integritas Karier Individu (Sub-CPMK 9)
Sebagai bentuk internalisasi prinsip etika ke dalam rencana profesi masa depan, setiap personel kelompok merumuskan komitmen integritas karier sebagai berikut:

*   **Muhammad Arya Alqadi (4524210058):** Sebagai calon profesional informatika, saya berkomitmen untuk menempatkan transparansi tata kelola data di atas kepentingan metrik performa bisnis korporasi. Dalam peran kepemimpinan teknis masa depan, saya akan secara aktif menolak segala bentuk instruksi manajemen yang melibatkan penyembunyian cacat arsitektur sistem (*concealment of defect*) yang berpotensi merugikan hak privasi masyarakat luas.
*   **Muzakki Abrar (4524210071):** Refleksi mendalam atas kasus ini menyadarkan saya akan pentingnya menjaga watak kebajikan (*virtue ethics*) dalam setiap fase pengembangan sistem. Saya berkomitmen untuk menerapkan kejujuran profesional dan menolak melakukan rekayasa antarmuka manipulatif (*dark patterns*) yang mengaburkan keabsahan *informed consent* subjek data terdampak.
*   **Muhammad Jibran Ferdian (4524210067):** Saya berkomitmen untuk menjadikan nilai-nilai luhur Pancasila dan klausul Kode Etik ACM/IEEE sebagai kompas moral utama dalam karier profesional saya di bidang teknologi informasi. Saya akan memastikan bahwa setiap arsitektur perangkat lunak yang saya bangun senantiasa menghormati martabat manusia dan menghindari potensi bahaya (*avoid harm*) bagi keharmonisan sosial.
*   **Muhammad Arkan (4524210114):** Karier masa depan saya di bidang TI akan mengintegrasikan manajemen risiko berbasis kerangka ISO 31000 secara ketat. Saya berkomitmen untuk secara proaktif melakukan kuantifikasi dan mitigasi terhadap risiko-risiko etis teknologi sejak fase perancangan sistem awal guna mencegah penyalahgunaan kewenangan digital.
*   **Daffa Richadatul'Aisy (4524210136):** Saya berkomitmen untuk memperjuangkan implementasi standar teknis *Privacy by Design* dan prinsip *Data Minimization* secara konkret pada setiap basis data yang saya rancang. Rencana karier saya akan berfokus pada pelindungan hak asasi informasi subjek data demi mewujudkan keadilan sosial digital.

#### 11.3. Daftar Pustaka Rujukan Primer
1.  Cadwalladr, C., & Graham-Harrison, E. (2018). *Revealed: 50 million Facebook profiles harvested for Cambridge Analytica in major data breach*. The Guardian.
2.  Republik Indonesia. (2008). *Undang-Undang Nomor 11 Tahun 2008 tentang Informasi dan Transaksi Elektronik (UU ITE)*. Sekretariat Negara. Jakarta.
3.  Republik Indonesia. (2022). *Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi (UU PDP)*. Sekretariat Negara. Jakarta.
4.  Susser, D., Roessler, B., & Nissenbaum, H. (2019). *Technology, autonomy, and manipulation*. Internet Policy Review, 8(2).
5.  Wylie, C. (2019). *Mindfck: Cambridge Analytica and the Plot to Break America*. Random House.
6.  Association for Computing Machinery. (2018). *ACM Code of Ethics and Professional Conduct*. ACM.
