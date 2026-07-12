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
#### 2.1. Fakta Terverifikasi Otoritas Hukum
Berdasarkan hasil investigasi resmi dari *Federal Trade Commission* (FTC) Amerika Serikat, *Information Commissioner's Office* (ICO) Inggris, serta dokumen pengakuan resmi dalam dengar pendapat parlemen (*Congressional Hearings*), berikut adalah fakta-fakta yang telah berkekuatan hukum tetap:
*   **Volume Pelanggaran Data:** Total subjek data yang diekstraksi secara tidak sah tanpa persetujuan eksplisit melalui mekanisme API Facebook mencapai 87 juta pengguna global, dengan mayoritas domisili subjek berada di wilayah Amerika Serikat.
*   **Komersialisasi Data Ilegal:** Terjadi transfer data dan transaksi komersial ilegal dari Global Science Research (GSR) oleh Dr. Aleksandr Kogan kepada Cambridge Analytica yang melanggar *Developer Terms of Service* Facebook.
*   **Kelalaian Pengawasan Platform:** Facebook telah mengetahui pelanggaran transfer data ini sejak akhir tahun 2015 namun menolak untuk melakukan audit teknis forensik secara mandiri dan hanya mengandalkan surat pernyataan kepatuhan tertulis dari Cambridge Analytica.
*   **Sanksi Hukum Resmi:** Facebook secara resmi dijatuhi sanksi denda administratif sebesar 5 Miliar Dolar AS oleh FTC pada tahun 2019 atas pelanggaran penyelesaian hak privasi konsumen (*privacy settlement*), serta denda sebesar 500.000 Poundsterling oleh ICO Inggris.
*   
#### 2.2. Catatan Transparansi Informasi (Status Investigasi dan Sengketa)
Untuk menjaga integritas laporan ilmiah, komponen berikut diklasifikasikan sebagai informasi yang sempat berada dalam sengketa atau memerlukan catatan transparansi khusus:
*   **Kuantifikasi Efektivitas Algoritma:** Klaim dari *whistleblower* Christopher Wylie mengenai tingkat efektivitas model psikometri OCEAN dalam mengubah keputusan politik pemilih secara absolut masih menjadi perdebatan akademis. Para peneliti ilmu sosial digital memisahkan antara fakta "keberhasilan pengumpulan data" dengan klaim "keberhasilan manipulasi psikologis total", karena tidak ada metrik yang dapat mengukur persentase murni perubahan suara pemilih yang hanya disebabkan oleh iklan media sosial.
*   **Keterlibatan Manajemen Eksekutif Tertinggi:** Status pengetahuan Mark Zuckerberg secara personal pada menit-menit awal kebocoran arsitektur Graph API di tahun 2014 sempat menjadi subjek sengketa informasi antara tim hukum internal platform dengan otoritas investigator hukum kongres sebelum akhirnya regulasi membuktikan adanya kelalaian sistemik korporasi.

### 3. Pemetaan Pemangku Kepentingan & Relasi Kuasa 
Analisis pemangku kepentingan (*stakeholders*) dalam skandal Facebook-Cambridge Analytica dibagi menjadi empat entitas utama yang terikat dalam struktur asimetri kekuasaan dan informasi:

#### 3.1. Penyedia Platform (Facebook Inc. / Meta)
*   **Peran dan Kedudukan:** Bertindak sebagai penyedia infrastruktur digital, pemilik data arsitektural Graph API, sekaligus pembuat kebijakan tata kelola ekosistem pengembang (*developer ecosystem*).
*   **Otoritas Pengambilan Keputusan:** Memiliki kontrol mutlak atas penentuan batasan hak akses data (*permission scopes*), mekanisme pengawasan pihak ketiga (*third-party monitoring*), dan tindakan mitigasi ketika pelanggaran terdeteksi.
*   **Motivasi/Kepentingan:** Maksimalisasi metrik pertumbuhan pengguna, durasi keterikatan platform (*user engagement*), dan peningkatan pendapatan kapitalisasi pasar melalui ekosistem periklanan digital.

#### 3.2. Penyedia Aplikasi & Data Broker (Global Science Research & Cambridge Analytica)
*   **Peran dan Kedudukan:** Entitas riset akademik dan konsultan politik yang mengeksploitasi keterbukaan fungsional Graph API untuk memanen basis data berskala besar (*data harvesting*).
*   **Otoritas Pengambilan Keputusan:** Mengambil keputusan secara sadar untuk memproses data psikometrik pengguna di luar tujuan awal pengumpulan data (kuis kepribadian akademik) dan mentransaksikannya demi keuntungan komersial-politik.
*   **Motivasi/Kepentingan:** Monetisasi data identitas digital dan pembuktian efektivitas algoritma pemetaan psikologis model OCEAN dalam kampanye rekayasa opini publik politik.

#### 3.3. Subjek Data / Pihak Terdampak (Pengguna Facebook & Jaringan Pertemanannya)
*   **Peran dan Kedudukan:** Pengguna layanan digital (*end-users*) yang datanya diekstraksi. Terdiri dari pengguna langsung aplikasi kuis serta "teman" dari pengguna tersebut yang datanya ikut tersedot secara pasif tanpa interaksi aktif.
*   **Otoritas Pengambilan Keputusan:** Tidak memiliki daya tawar (*bargaining power*) atau pilihan kontrol fungsional atas data mereka karena dikaburkan oleh desain antarmuka platform (*dark patterns*) dan ketiadaan transparansi izin operasional API.
*   **Motivasi/Kepentingan:** Memanfaatkan utilitas interaksi sosial gratis pada platform media sosial tanpa ekspektasi bahwa identitas digital mereka akan dipersenjatai untuk kepentingan manipulasi politik.

#### 3.4. Institusi Demokrasi & Masyarakat Sipil Global
*   **Peran dan Kedudukan:** Lingkungan sosial-politik eksternal yang stabilitas dan kedaulatannya bergantung pada kejujuran peredaran informasi.
*   **Otoritas Pengambilan Keputusan:** Lembaga pengawas pemilu dan pemilih umum yang hak otonomi suaranya terdistorsi oleh paparan iklan terselubung (*dark ads*).
*   **Motivasi/Kepentingan:** Menjaga integritas proses demokrasi, transparansi kompetisi politik, dan pelindungan hak asasi warga negara atas informasi yang objektif.

#### 3.5. Analisis Asimetri Relasi Kuasa
Investigasi kelompok kami menunjukkan adanya ketimpangan kuasa (*power asymmetry*) yang masif. Korporasi teknologi raksasa (Facebook) dan agensi mahadata (Cambridge Analytica) memegang kendali penuh atas asimetri informasi, di mana mereka mengetahui secara presisi kerentanan psikologis subjek data melalui komputasi tingkat tinggi. Sebaliknya, 87 juta subjek data berada dalam kondisi ketidaktahuan total (*total ignorance*), tidak mampu memverifikasi ke mana data mereka dialirkan, dan hak otonomi mereka sebagai manusia direduksi menjadi komoditas finansial murni. Ketimpangan relasi kuasa inilah yang menjadi celah utama runtuhnya ketahanan etika fungsional teknologi.

### 4. Analisis Berdasarkan Empat Teori Etika Moral 
Evaluasi etika terhadap tindakan Facebook Inc. dan Cambridge Analytica dilakukan secara eksplisit menggunakan empat kerangka filsafat moral normatif sebagai berikut:

#### 4.1. Analisis Utilitarianisme
Teori Utilitarianisme (Jeremy Bentham & John Stuart Mill) menyatakan bahwa suatu tindakan dianggap benar secara moral jika mampu menghasilkan kemanfaatan atau kebahagiaan terbesar bagi jumlah orang terbanyak (*the greatest happiness for the greatest number*), serta meminimalkan penderitaan (*harm*).
*   **Aplikasi Kasus:** Tindakan pemanenan data oleh Cambridge Analytica dan pembiaran celah arsitektur oleh Facebook secara mutlak gagal memenuhi standar moral utilitarian. Kebahagiaan atau keuntungan finansial-politik hanya dirasakan oleh segelintir entitas korporasi dan aktor politik.
*   **Kalkulasi Utilitas:** Di sisi lain, tindakan ini mendistribusikan penderitaan (*harm*) berskala masif berupa pelanggaran hak privasi 87 juta individu, erosi kepercayaan publik terhadap ekosistem digital, serta polarisasi sosial akibat paparan propaganda kognitif. Berdasarkan kalkulasi utilitas net, tindakan ekosistem industri data ini menghasilkan akumulasi penderitaan yang jauh melampaui utilitas positifnya, sehingga diklasifikasikan sebagai tindakan yang cacat moral.

#### 4.2. Analisis Deontologi
Teori Deontologi (Immanuel Kant) menekankan bahwa moralitas suatu tindakan dinilai berdasarkan kepatuhannya terhadap kewajiban (*duty*) dan prinsip moral imperatif kategoris, terlepas dari hasil akhir yang diperoleh. Kant merumuskan bahwa manusia harus selalu diperlakukan sebagai tujuan pada dirinya sendiri (*end in itself*), dan tidak pernah boleh direduksi sekadar sebagai sarana (*mere means*).
*   **Aplikasi Kasus:** Facebook memiliki kewajiban moral *a priori* untuk melindungi integritas privasi subjek data yang mempercayakan identitas mereka pada platform. Ketika Facebook membiarkan eksploitasi fitur Graph API demi pertumbuhan metrik dan Cambridge Analytica memperjualbelikan basis data tersebut, kedua entitas ini secara sadar memperlakukan 87 juta manusia sekadar sebagai komoditas atau alat (sarana) demi meraih profitabilitas ekonomi dan kemenangan politik klien. Tindakan ini melanggar maksim universalitas dan kewajiban moral fundamental, sehingga dinilai tidak etis secara deontologis.

#### 4.3. Analisis Etika Kebajikan (Virtue Ethics)
Etika Kebajikan (Aristoteles) berfokus pada watak, karakter moral, dan integritas batin dari pelaku tindakan (*agent*), bukan sekadar kepatuhan pada aturan atau kalkulasi dampak. Kebajikan profesional diukur melalui nilai kejujuran (*honesty*), transparansi, tanggung jawab (*accountability*), dan kehati-hatian (*prudence*).
*   **Aplikasi Kasus:** Investigasi membuktikan ketiadaan watak kebajikan (*virtues*) pada manajemen Facebook dan Cambridge Analytica. Sikap Facebook yang mendeteksi penyalahgunaan data pada tahun 2015 namun memilih menyembunyikannya dari publik demi proteksi reputasi korporasi mencerminkan karakter ketidakjujuran (*dishonesty*) dan pengabaian profesional (*professional negligence*). Cambridge Analytica juga menunjukkan cacat watak *vice* (keburukan) berupa keserakahan dan manipulasi sistemik. Kedua entitas gagal mendemonstrasikan karakteristik profesional TI yang berintegritas mulia.

#### 4.4. Analisis Etika Hak / Kontraktarian
Teori Etika Hak menyatakan bahwa suatu tindakan secara moral benar jika menghormati hak-hak asasi fundamental yang melekat pada setiap individu, termasuk hak atas privasi dan hak otonomi diri (*autonomy*). Dalam era digital, hak ini dimanifestasikan melalui pemenuhan kontrak sosial digital berupa mekanisme *informed consent* yang valid, transparan, dan eksplisit.
*   **Aplikasi Kasus:** Terjadi degradasi total terhadap otonomi individu subjek data. Fitur eksploitatif Graph API `user_friends` secara sengaja menerobos hak privasi pihak ketiga (jaringan pertemanan pengguna utama) tanpa adanya interaksi otorisasi langsung. Mekanisme persetujuan yang disajikan oleh Facebook diklasifikasikan sebagai *dark patterns* yang manipulatif, sehingga persetujuan pengguna tidak sah di mata etika kontraktarian. Kegagalan *informed consent* ini meruntuhkan kontrak sosial antara penyedia platform dengan masyarakat digital, menjadikannya pelanggaran hak asasi informasi yang sangat berat.
### 5. Lensa Kelima Pancasila & Nilai Luhur UP 
Analisis komprehensif terhadap skandal pemanenan data Facebook-Cambridge Analytica dievaluasi melalui dasar filosofis negara (Sila 1–5) serta lima Nilai Kepancasilaan Universitas Pancasila (UP):
*   *Sila Pertama - Ketuhanan Yang Maha Esa:* Eksploitasi identitas digital demi profit dan kekuasaan politik mencerminkan pengabaian terhadap eksistensi moralitas ketuhanan yang mewajibkan setiap manusia memperlakukan sesamanya dengan kejujuran mutlak. Penipuan sistemik dan manipulasi psikologis terselubung merupakan bentuk pengingkaran terhadap nilai-nilai spiritual dan nurani luhur kemanusiaan.
*   *Sila Kedua - Kemanusiaan yang Adil dan Beradab:* Komodifikasi identitas digital manusia menjadi komoditas finansial murni oleh data broker merupakan bentuk degradasi terhadap harkat dan martabat manusia. Tindakan memperlakukan 87 juta subjek data sebagai instrumen manipulasi kognitif tanpa adab perlindungan privasi merupakan pelanggaran berat terhadap hak asasi kemanusiaan.
*   *Sila Ketiga - Persatuan Indonesia:* Senjataisasi algoritma melalui taktik political micro-targeting dirancang khusus untuk mengeksploitasi bias psikologis dan ketakutan individu. Hal ini memicu radikalisasi opini, penyebaran berita bohong secara masif, dan pengkutuban sosial yang secara langsung mengancam kohesi serta persatuan nasional dalam masyarakat demokratis.
*   *Sila Keempat - Kerakyatan yang Dipimpin oleh Hikmat Kebijaksanaan dalam Permusyawaratan/Perwakilan:* Skandal ini merusak pilar otonomi informasi yang krusial bagi demokrasi yang sehat. Ketika hak masyarakat untuk mendapatkan informasi yang objektif didistorsi oleh propaganda terselubung (dark ads), maka asas kedaulatan rakyat dan pengambilan keputusan yang bijaksana dalam proses politik telah dicederai secara sistemik.
*   *Sila Kelima - Keadilan Sosial bagi Seluruh Rakyat Indonesia:* Terjadi ketimpangan keadilan (asymmetry) yang masif di mana korporasi teknologi raksasa memonopoli kontrol atas mahadata masyarakat demi keuntungan sepihak. Ketiadaan perlindungan hak privasi dan akses ruang banding yang setara bagi subjek data terdampak mencerminkan pelanggaran terhadap prinsip keadilan sosial di ruang digital.

*   #### 5.2. Penyelarasan Nilai Kepancasilaan Universitas Pancasila (UP)
*   *Integritas:* Facebook dan Cambridge Analytica secara nyata melanggar nilai integritas melalui tindakan penyembunyian cacat Graph API dan pemindahtanganan data ilegal. Pengembang gagal mempertahankan kejujuran ilmiah dan transparansi profesional.
*   *Kepedulian:* Terjadi pengabaian total (professional negligence) terhadap keselamatan hak privasi konsumen. Metrik pertumbuhan profit platform ditempatkan jauh di atas kepedulian terhadap keamanan data pribadi subjek.
*   *Harmonis:* Tindakan pembiaran manipulasi data berujung pada terciptanya gelembung informasi (filter bubbles) yang merusak keharmonisan kehidupan bermasyarakat, memicu konflik horizontal berbasis sentimen psikometrik yang dieksploitasi.
*   *Kolaboratif:* Hubungan kerja sama antara Dr. Aleksandr Kogan (GSR) dengan Cambridge Analytica dikategorikan sebagai kolaborasi transgresif yang merusak kepercayaan publik, bertentangan dengan prinsip kolaborasi positif demi kemaslahatan ilmu pengetahuan.
*   *Profesionalisme:* Sebagai calon profesional informatika, kegagalan penegakan prinsip Privacy by Design dalam kasus ini menjadi cerminan runtuhnya kompetensi moral dan tanggung jawab keahlian yang seharusnya melekat pada seorang arsitek rekayasa perangkat lunak.

### 6. Kepatuhan Kode Etik Profesi Internasional 
Investigasi kelompok kami memetakan bahwa praktik rekayasa perangkat lunak dan tata kelola data dalam skandal Facebook-Cambridge Analytica secara eksplisit melanggar klausul-klausul fundamental dalam ACM/IEEE Code of Ethics and Professional Conduct. Pelanggaran tersebut dianalisis pada poin-poin berikut:
*   *Ketentuan Kode Etik:* Profesional IT wajib meminimalkan konsekuensi negatif dari sistem komputasi, termasuk pelanggaran privasi, cedera fisik, maupun kerusakan sosial-ekonomi.
*   *Analisis Kasus:* Pengembang Facebook melakukan pembiaran (professional negligence) terhadap kerentanan arsitektural Graph API v1.0 demi akselerasi metrik bisnis. Tindakan ini memicu bahaya (harm) masif berupa eksploitasi psikometrik terhadap 87 juta individu serta polarisasi sosial global, yang bertentangan secara absolut dengan kewajiban untuk menghindari bahaya.

*   #### 6.2. Pelanggaran Klausul 1.6: Menghormati Privasi (Respect Privacy)
*   *Ketentuan Kode Etik:* Profesional IT wajib memahami bahwa privasi adalah hak asasi terintegrasi. Pengumpulan, transfer, dan penyimpanan data pribadi hanya boleh dilakukan atas persetujuan yang transparan dan sah dari pemilik data.
*   *Analisis Kasus:* Implementasi endpoint permission user_friends secara sengaja dirancang untuk menyedot data pihak ketiga (jaringan pertemanan pengguna utama) tanpa adanya interaksi otorisasi langsung. Tindakan pemanenan data masif (data harvesting) tanpa informed consent ini merupakan bentuk pelanggaran fatal terhadap klausul perlindungan privasi subjek data.

*   #### 6.3. Pelanggaran Klausul 2.3: Mematuhi Hukum dan Regulasi (Know and Respect Existing Rules)
*   *Ketentuan Kode Etik:* Profesional TI wajib mengetahui, memahami, dan mematuhi peraturan hukum, standar industri, serta ketentuan kebijakan operasional yang berlaku.
*   *Analisis Kasus:* Dr. Aleksandr Kogan secara sadar melanggar Developer Terms of Service Facebook dengan memindahtangan data komersial kepada Cambridge Analytica. Di sisi lain, Cambridge Analytica secara sengaja melanggar regulasi perlindungan data di berbagai yurisdiksi demi kepentingan manipulasi politik klien.

*   #### 6.4. Pelanggaran Klausul 2.5: Mengutamakan Penilaian Kualitatif Profesional (Give Comprehensive and Thorough Evaluations)
*   *Ketentuan Kode Etik:* Profesional IT wajib melakukan evaluasi risiko yang menyeluruh terhadap sistem komputasi dan dampaknya bagi masyarakat sipil.
*   *Analisis Kasus:* Tim perekayasa perangkat lunak Facebook gagal menerapkan prinsip Privacy by Design pada fase perancangan Graph API. Ketika cacat keamanan fungsional terdeteksi pada akhir 2015, manajemen platform memilih jalan pintas berupa perjanjian penghapusan data tertulis sepihak tanpa melakukan audit forensik digital lanjutan, demi melindungi kepentingan reputasi korporasi di atas keselamatan subjek data.

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
