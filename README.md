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


### 8. Checkpoint Integritas & Pencegahan Penyalahgunaan Kewenangan 


### 9. Manajemen Risiko Teknologi Berbasis Kerangka ISO 31000 


### 10. Rancangan Dampak Sosial & Kontrol Preventif Rekayasa Perangkat Lunak 


### 11. Pelajaran Utama & Rujukan Pustaka 
