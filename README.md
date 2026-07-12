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
#### 1.1. Konteks Arsitektur Teknis Platform
Insiden pelanggaran privasi global ini tidak diinisiasi oleh penetrasi paksa atau peretasan konvensional (*hacking*) terhadap perimeter keamanan server Facebook. Krisis ini berakar pada eksploitasi celah struktural fungsional yang terdapat pada arsitektur rekayasa perangkat lunak Facebook Graph API versi 1.0, khususnya pada *endpoint permission* `user_friends`. 

Secara arsitektural, Protokol OAuth dan Graph API pada periode tersebut didesain untuk memaksimalkan interkoneksi ekosistem aplikasi pihak ketiga (*third-party developers*). Ketika seorang pengguna memberikan otorisasi akses kepada suatu aplikasi, *endpoint* `user_friends` secara otomatis membuka gerbang akses data agregat yang mencakup profil, preferensi, dan jaringan pertemanan dari pengguna utama tersebut. Implikasinya, seluruh individu yang berada dalam relasi pertemanan pengguna utama ikut terekstraksi datanya, meskipun subjek data pihak ketiga tersebut tidak pernah berinteraksi, memberikan izin, atau mengonfirmasi persetujuan (*informed consent*) secara langsung terhadap aplikasi bersangkutan.

<div align="center">
  <img width="8192" height="1972" alt="etprof2" src="https://github.com/user-attachments/assets/e758341d-7e6c-461d-b41d-afca3803f036" />
  <br>
  <em>Gambar 1.1: Sequence Diagram Alur Pemanenan dan Otorisasi Akses Pihak Ketiga pada Graph API v1.0</em>
</div>

#### 1.2. Linimasa dan Kronologi Peristiwa
Rekonstruksi rangkaian peristiwa eksploitasi data berskala besar ini disusun berdasarkan urutan waktu kejadian sebagai berikut:

*   **Tahun 2013 (Fase Inisiasi & Pengembangan Aplikasi):** Dr. Aleksandr Kogan, seorang peneliti psikologi dari University of Cambridge, mendirikan entitas Global Science Research (GSR). Kogan membangun sebuah aplikasi kuis kepribadian berbasis digital di platform Facebook yang dinamakan *"thisisyourdigitallife"*.
*   **Tahun 2014 (Fase Pemanenan Data Masif / *Data Harvesting*):** Aplikasi *"thisisyourdigitallife"* berhasil menjaring sekitar 270.000 pengguna aktif yang memberikan izin akses. Melalui eksploitasi celah *endpoint* Graph API `user_friends` yang aktif pada saat itu, GSR berhasil menyedot data pribadi dari jaringan pertemanan para pengguna utama secara eksponensial, hingga mengumpulkan profil psikometrik dari total 87 juta individu di seluruh dunia secara prosedural-legal platform namun cacat moral.
*   **Tahun 2014 - 2015 (Fase Transaksi Transgresif & Komodifikasi Data):** Bertentangan dengan ketentuan layanan pengembang Facebook yang melarang pemindahtanganan data ke pihak ketiga untuk tujuan komersial, Global Science Research (GSR) melakukan transaksi penjualan basis data tersebut kepada Cambridge Analytica (CA), sebuah perusahaan konsultan politik yang dipimpin oleh Alexander Nix.
*   **Tahun 2015 - 2016 (Fase Senjataisasi Algoritma & Rekayasa Psikologis):** Cambridge Analytica mengolah mahadata (*Big Data*) tersebut menggunakan model psikometri OCEAN (*Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism*). Data ini dijadikan instrumen untuk memetakan kerentanan psikologis individu, yang kemudian digunakan untuk mendistribusikan propaganda kognitif secara presisi melalui metode *political micro-targeting* guna memengaruhi dinamika politik global, termasuk kampanye Pemilu Presiden Amerika Serikat 2016 dan referendum Brexit di Inggris.
*   **Desember 2015 (Fase Penemuan Internal & Mitigasi Lemah Platform):** Jurnalis *The Guardian*, Harry Davies, menerbitkan laporan awal mengenai pemanfaatan data Facebook oleh Cambridge Analytica. Pihak Facebook mendeteksi adanya pelanggaran kebijakan pengembang dan meminta secara formal kepada Cambridge Analytica untuk menghapus seluruh data yang diperoleh. Namun, Facebook tidak melakukan verifikasi forensik digital lanjutan dan memilih memercayai surat pernyataan penghapusan sepihak dari CA demi menjaga stabilitas reputasi korporasi.
*   **Maret 2018 (Fase Eksposur Publik & Investigasi Global):** Christopher Wylie, mantan analis data dari Cambridge Analytica, bertindak sebagai *whistleblower* dengan membeberkan dokumen internal kepada media *The Guardian* dan *The New York Times*. Pengakuan ini memicu kecaman publik global, penurunan kapitalisasi pasar Facebook secara drastis, serta dimulainya investigasi formal oleh lembaga regulator internasional seperti *Federal Trade Commission* (FTC) di AS dan *Information Commissioner's Office* (ICO) di Inggris.

### 2. Fakta Kunci & Catatan Transparansi 


### 3. Pemetaan Pemangku Kepentingan & Relasi Kuasa 


### 4. Analisis Berdasarkan Empat Teori Etika Moral 


### 5. Lensa Kelima Pancasila & Nilai Luhur UP 


### 6. Kepatuhan Kode Etik Profesi Internasional 


### 7. Analisis Regulasi Yuridis & Yurisdiksi Hukum 

Evaluasi yuridis terhadap skandal Facebook-Cambridge Analytica dianalisis menggunakan kerangka hukum positif Republik Indonesia serta pemisahan yurisdiksi tanggung jawab sebagai berikut:

#### 7.1. Evaluasi Berdasarkan UU Pelindungan Data Pribadi (UU PDP No. 27 Tahun 2022)
Meskipun secara kronologis insiden ini terjadi sebelum pengesahan UU PDP No. 27 Tahun 2022 (asas legalitas/non-retroaktif), instrumen ini sangat krusial digunakan sebagai kerangka evaluasi yuridis kontemporer terhadap tata kelola data platform.
*   **Pelanggaran Asas Pemrosesan Data (Pasal 16):** UU PDP mewajibkan pemrosesan data pribadi dilakukan secara terbatas, spesifik, sah secara hukum, dan transparan. Tindakan eksploitasi data pengguna untuk kepentingan micro-targeting politik di luar tujuan awal pengumpulan data (kuis kepribadian) merupakan pelanggaran absolut terhadap pasal ini.
*   **Kegagalan Dasar Hukum Pemrosesan (Pasal 20):** Pengumpul data wajib memiliki dasar hukum (*lawful basis*) yang sah, salah satunya berupa persetujuan sah yang eksplisit (*explicit consent*). Penyerapan data jaringan pertemanan (*third-party data*) tanpa interaksi otorisasi langsung tidak memiliki dasar hukum yuridis yang sah di bawah kerangka UU PDP.
*   **Ketentuan Sanksi Kontemporer:** Jika insiden ini dievaluasi dengan yurisdiksi hukum Indonesia saat ini, kebocoran data berskala masif akibat kelalaian sistemik dapat menjatuhkan sanksi administratif berupa penghentian pemrosesan, penghapusan data, hingga denda denda administratif paling tinggi 2 persen dari pendapatan tahunan terhadap korporasi selaku Pengendali Data Pribadi.

#### 7.2. Evaluasi Berdasarkan UU Informasi dan Transaksi Elektronik (UU ITE)
*   **Pelanggaran Hak Otonomi Data (Pasal 26 ayat 1):** UU ITE menegaskan bahwa kecuali ditentukan lain oleh peraturan perundang-undangan, penggunaan setiap informasi melalui media elektronik yang menyangkut data pribadi seseorang harus dilakukan atas persetujuan (*consent*) orang yang bersangkutan.
*   **Keabsahan Persetujuan Digital:** Kasus ini membuktikan secara yuridis bahwa persetujuan yang diperoleh melalui manipulasi antarmuka digital (*dark patterns*) atau klausul tersembunyi berstatus tidak sah secara hukum. Subjek data yang haknya dilanggar berhak mengajukan gugatan atas kerugian yang ditimbulkan berdasarkan Pasal 26 ayat 2 UU ITE.

#### 7.3. Pemisahan Tegas Tanggung Jawab Hukum (Legal) vs Tanggung Jawab Moral
Investigasi kelompok kami memisahkan batas akuntabilitas platform ke dalam dua domain:
1.  **Tanggung Jawab Hukum (Legal Responsibility):** Terikat pada kepatuhan formal terhadap pemenuhan dokumen kontrak, *Developer Terms of Service*, dan aturan tertulis di masing-masing yurisdiksi negara (seperti kepatuhan formal Facebook terhadap *Consent Decree* FTC di AS). Secara prosedural arsitektur API pada tahun 2014, penarikan data tersebut dimungkinkan oleh sistem, namun eksploitasi komersialnya melanggar batas legalitas perjanjian kontrak pihak ketiga.
2.  **Tanggung Jawab Moral (Moral Responsibility):** Berada pada tataran etika profesi rekayasa perangkat lunak. Meskipun suatu fitur secara prosedural teknis "diizinkan" atau belum diatur oleh undang-undang spesifik pada masa itu, pengembang platform memiliki tanggung jawab moral *a priori* untuk menerapkan prinsip *Privacy by Design* demi melindungi hak privasi subjek data yang rentan. Ketiadaan regulasi hukum formal tidak boleh dijadikan pembenaran etis atas tindakan komodifikasi identitas manusia.

### 8. Checkpoint Integritas & Pencegahan Penyalahgunaan Kewenangan 

Berdasarkan parameter penugasan Project-Based Learning Etika Profesi, dimensi integritas dan anti-korupsi dalam ranah teknologi informasi dianalisis secara komprehensif sebagai bentuk pencegahan penyalahgunaan kewenangan serta manipulasi posisi dominan korporasi demi keuntungan sepihak. Evaluasi terhadap kasus ini dipetakan ke dalam beberapa bentuk pelanggaran integritas berikut:

#### 8.1. Penyalahgunaan Posisi Dominan dan Kepercayaan (Abuse of Trust)
Facebook Inc. memegang peranan sebagai pemelihara ekosistem digital yang menguasai data miliaran manusia secara global. Posisi dominan ini melahirkan kewajiban etis berupa penjagaan kepercayaan publik (*fiduciary duty*). Namun, investigasi membuktikan terjadinya pengabaian profesional (*professional negligence*) yang terstruktur. Pihak platform menyalahgunakan kepercayaan pengguna dengan membiarkan arsitektur data fungsionalnya dieksploitasi oleh pihak ketiga tanpa mitigasi ketat, demi menjaga pertumbuhan ekonomi korporasi berbasis monetisasi data identitas digital.

#### 8.2. Penyembunyian Cacat Fungsional Sistem (Concealment of Defect)
Pelanggaran integritas paling krusial terjadi ketika manajemen Facebook mendeteksi adanya transaksi pemindahtanganan basis data secara ilegal dari Global Science Research (GSR) ke Cambridge Analytica pada akhir tahun 2015. Alih-alih mengumumkan insiden kebocoran privasi ini kepada 87 juta subjek data terdampak atau melaporkannya kepada otoritas regulasi hukum, Facebook secara sadar memilih untuk menyembunyikan cacat penegakan kebijakan tersebut dari publik demi proteksi nilai kapitalisasi pasar korporasi. Penyelarasan tindakan ini dikategorikan sebagai bentuk ketidakjujuran profesional yang menempatkan metrik finansial di atas transparansi informasi.

#### 8.3. Konflik Kepentingan (Conflict of Interest)
Terdapat benturan kepentingan yang tidak terselesaikan antara komitmen etis pelindungan privasi dengan model bisnis inti platform yang bergantung pada pendapatan periklanan mikro (*targeted advertising*). Facebook membiarkan kebijakan pelonggaran otorisasi pihak ketiga berjalan tanpa pengawasan ketat (*third-party monitoring*) karena ekosistem aplikasi eksternal berkontribusi langsung pada peningkatan durasi keterikatan pengguna (*user engagement*) dan volume pertukaran data. Ketika profitabilitas bisnis berbenturan dengan keselamatan data subjek, integritas arsitektur rekayasa perangkat lunak dikompromikan demi memenangkan kepentingan pasar.

#### 8.4. Lensa Integrasi Anti-Korupsi Sektor Publik (Kontekstualisasi)
Meskipun kasus Facebook-Cambridge Analytica melibatkan entitas korporasi privat internasional, bentuk senjataisasi data ini memberikan dampak transgresif terhadap institusi negara dan proses demokrasi. Tindakan penyalahgunaan kewenangan digital oleh pengembang platform dan transaksi pemanfaatan data broker untuk rekayasa opini politik secara terselubung mencerminkan korupsi terhadap nilai kejujuran informasi. Dalam skala yurisdiksi nasional, pembiaran atau manipulasi data yang menyerang hak kedaulatan informasi publik diklasifikasikan sebagai bentuk kejahatan integritas tingkat tinggi yang mencederai keadilan sosial dan stabilitas tata kelola pemilu yang bersih.

### 9. Manajemen Risiko Teknologi Berbasis Kerangka ISO 31000 


### 10. Rancangan Dampak Sosial & Kontrol Preventif Rekayasa Perangkat Lunak 


### 11. Pelajaran Utama & Rujukan Pustaka 
