---
layout: post
title: Information Retrieval pada Search Engine
author: Catherine Almira
---

Dewasa ini, jumlah informasi yang beredar di internet semakin banyak dan tak terhitung jumlahnya sehingga hampir seluruh informasi yang dibutuhkan dapat diperoleh dari internet. Pengumpulan suatu informasi yang dibutuhkan memerlukan proses pencarian dari sejumlah informasi yang telah tersimpan tersebut.

## Information Retrieval pada Search Engine
-----

Dewasa ini, jumlah informasi yang beredar di internet semakin banyak dan tak terhitung jumlahnya sehingga hampir seluruh informasi yang dibutuhkan dapat diperoleh dari internet. Pengumpulan suatu informasi yang dibutuhkan memerlukan proses pencarian dari sejumlah informasi yang telah tersimpan tersebut. Sistem pencarian suatu informasi dari sejumlah informasi yang ada disebut information retrieval.

Pada awalnya, informasi yang ada hanya didokumentasikan dan diberi indeks sehingga lebih teratur dan mempermudah proses pencarian. Namun, dengan semakin banyaknya informasi yang ada, dokumentasi dan indeks saja tidak cukup untuk mencari informasi yang dibutuhkan dari kumpulan informasi yang jumlahnya sangat banyak, terlebih lagi apabila pencarian dilakukan pada isi dokumen, tidak hanya pada judul atau kategori yang cenderung lebih mudah dicari. Salah satu information retriever yang paling umum digunakan adalah search engine.

Interaksi suatu information retriever dengan pengguna adalah dengan meminta kata kunci dari informasi yang akan dicari dari sekumpulan informasi yang ada. Kata kunci yang dimasukkan ini disebut dengan query dan kemudian information retriever ini akan memunculkan informasi-informasi yang relevan dari informasi yang ada dengan melihat kecocokan query dengan informasi yang ada.

![Ilustrasi Information Retrieval](/images/pic1.jpg)

Dasar-dasar dari information retrieval:
1.	Text Operations (operasi terhadap teks) yang meliputi pemilihan kata-kata dalam query maupun dokumen dalam pentransformasian dokumen atau query menjadi terms index (indeks dari kata-kata).
2.	Query Formulation (formulasi terhadap query) yang memberi bobot pada indeks kata-kata query.
3.	Ranking, mencari dokumen-dokumen yang relevan terhadap query dan mengurutkan dokumen tersebut berdasarkan kesesuaiannya dengan query.
4.	Indexing, membangun data indeks dari koleksi dokumen. Dilkakukan terlebih dahulu sebelum pencarian dokumen, sistem temu balik informasi menerima query dari pengguna, kemudian melakukan perangkingan terhadap pada koleksi berdasarkan kesesuaiannya dengan query. Hasil perangkingan yang diberikan kepada pengguna merupakan dokumen yang sistem, relevan dengan query, namun relevansi dokumen terhadap suatu query merupakan penilaian pengguna yang subjektif dan dipengaruhi banyak faktor.

Contoh cara kerja IR pada kasus mesin pencari (search-engine):
Mesin pencari web atau yang lebih dikenal dengan istilah web search engine merupakan program komputer yang dirancang untuk mencari informasi yang tersedia didalam dunia maya. Berbeda halnya dengan direktori web (seperti dmoz.org) yang dikerjakan oleh manusia untuk mengelompokkan suatu halaman informasi berdasarkan kriteria yang ada, web search engine mengumpulkan informasi yang tersedia secara otomatis.

Mesin pencari web bekerja dengan cara menyimpan hampir semua informasi halaman web, yang diambil langsung dari www. Halaman-halaman ini diambil secara otomatis. Isi setiap halaman lalu dianalisis untuk menentukan cara mengindeksnya (misalnya, kata-kata diambil dari judul, subjudul, atau field khusus yang disebut meta tag). Data tentang halaman web disimpan dalam sebuah database indeks untuk digunakan dalam pencarian selanjutnya. Sebagian mesin pencari, seperti Google, menyimpan seluruh atau sebagian halaman sumber (yang disebut cache) maupun informasi tentang halaman web itu sendiri.

Ketika seorang pengguna mengunjungi mesin pencari dan memasukkan query, biasanya dengan memasukkan kata kunci, mesin mencari indeks dan memberikan daftar halaman web yang paling sesuai dengan kriterianya, biasanya disertai ringkasan singkat mengenai judul dokumen dan terkadang sebagian teksnya. Mesin pencari lain yang menggunakan proses real-time, seperti Orase, tidak menggunakan indeks dalam cara kerjanya. Informasi yang diperlukan mesin tersebut hanya dikumpulkan jika ada pencarian baru. Jika dibandingkan dengan sistem berbasis indeks yang digunakan mesin-mesin seperti Google, sistem real-time ini unggul dalam beberapa hal seperti informasi selalu mutakhir, (hampir) tak ada broken link, dan lebih sedikit sumberdaya sistem yang diperlukan (Google menggunakan hampir 100.000 komputer, Orase hanya satu). Tetapi, ada juga kelemahannya yaitu pencarian lebih lama rampungnya.

Komponen utama dalam Search Engine
Sebuah search engine memiliki beberapa komponen agar dapat menyediakan layanan utamanya sebagai sebuah mesin pencari informasi. Komponen tersebut antara lain :

1.	Web Crawler

Web Crawler atau yang dikenal juga dengan istilah web spider bertugas untuk mengumpulkan semua informasi yang ada di dalam halaman web. Web crawler bekerja secara otomatis dengan cara memberikan sejumlah alamat website untuk dikunjungi serta menyimpan semua informasi yang terkandung didalamnya. Setiap kali web crawler mengunjungi sebuah website, maka dia akan mendata semua link yang ada dihalaman yang dikunjunginya itu untuk kemudian di kunjungi lagi satu persatu.

Proses web crawler dalam mengunjungi setiap dokumen web disebut dengan web crawling atau spidering. Beberapa websites, khususnya yang berhubungan dengan pencarian menggunakan proses spidering untuk memperbaharui data data mereka. Web crawler biasa digunakan untuk membuat salinan secara sebhagian atau keseluruhan halaman web yang telah dikunjunginya agar dapat dip roses lebih lanjut oleh system pengindexan. Crawler dapat juga digunakan untuk proses pemeliharaan sebuah website, seperti memvalidasi kode html sebuah web, dan crawler juga digunakan untuk memperoleh data yang khusus seperti mengumpulkan alamat e-mail.

Web crawler termasuk kedalam bagian software agent atau yang lebih dikenal dengan istilah program bot. Secara umum crawler memulai prosesnya dengan memberikan daftar sejumlah alamat website untuk dikunjungi, disebut sebagai seeds. Setiap kali sebuah halaman web dikunjungi, crawler akan mencari alamat yang lain yang terdapat didalamnya dan menambahkan kedalam daftar seeds sebelumnya.

Dalam melakukan prosesnya, web crawler juga mempunyai beberapa persoalan yang harus mampu di atasinya. Permasalahan tersebut mencakup:

•	Halaman mana yang harus dikunjungi terlebih dahulu.

•	Aturan dalam proses mengunjungi kembali sebuah halaman.

•	Performansi, mencakup banyaknya halaman yang harus dikunjungi.

•	Aturan dalam setiap kunjungan agar server yang dikunjungi tidak kelebihan beban.

•	Kegagalan, mencakup tidak tersedianya halaman yang dikunjungi, server down, timeout, maupun jebakan yang sengaja dibuat oleh webmaster.

•	Seberapa jauh kedalaman sebuah website yang akan dikunjungi.

•	Hal yang tak kalah pentingnya adalah kemampuan web crawler untuk mengikuti perkembangan teknologi web, dimana setiap kali teknologi baru muncul, web crawler harus dapat menyesuaikan diri agar dapat mengunjungi halaman web yang menggunakan teknologi baru tersebut. Proses sebuah web crawler untuk mendata link–link yang terdapat didalam sebuah halaman web menggunakan pendekatan regular expression. Crawler akan menelurusi setiap karakter yang ada untuk menemukan hyperlink tag html (<a>). Setiap hyperlink tag yang ditemukan diperiksa lebih lanjut apakah tag tersebut mengandung atribut nofollow rel, jika tidak ada maka diambil nilai yang terdapat didalam attribute href yang merupakan sebuah link baru.

2.	Indexing System

Indexing system bertugas untuk menganalisa halaman web yang telah tersimpan sebelumnya dengan cara mengindeks setiap kemungkinan term yang terdapat di dalamnnya. Data term yang ditemukan disimpan dalam sebuah database indeks untuk digunakan dalam pencarian selanjutnya.

Indexing system mengumpulkan, memilah dan menyimpan data untuk memberikan kemudahan dalam pengaksesan informasi secara tepat dan akurat. Proses pengolahan halaman web agar dapat digunakan untuk proses pencarian berikutnya dinakamakan web indexing. Dalam implementasinya index system dirancang dari penggabungan beberapa cabang ilmu antara lain ilmu bahasa, psikologi, matematika, informatika, fisika, dan ilmu komputer.

Tujuan dari penyimpanan data berupa indeks adalah untuk performansi dan kecepatan dalam menemukan informasi yang relevan berdasarkan inputan user. Tanpa adanya indeks, search engine harus melakukan scan terhadap setiap dokumen yang ada didalam database. Hal ini tentu saja akan membutuhkan proses sumber daya yang sangat besar dalam proses komputasi. Sebagai contoh, indeks dari 10.000 dokumen dapat diproses dalam waktu beberapa detik saja, sedangkan penulusuran secara berurutan setiap kata yang terdapat di dalam 10.000 dokumen akan membutuhkan waktu yang berjam lamanya. Tempat tambahan mungkin akan dibutuhkan di dalam computer untuk penyimpanan indeks, tapi hal ini akan terbayar dengan penghematan waktu pada saat pemrosesan pencarian dokumen yang dibutuhkan.

3.	Search system

Search system inilah yang berhubungan langsung dengan pengguna, meyediakan hasil pencarian informasi yang diinginkan. Ketika seorang pengguna mengunjungi mesin pencari dan memasukkan kata pencarian biasanya dengan beberapa kata kunci, search system akan mencari data dari indeks database, data yang cocok kemudian akan ditampilkan, biasanya disertai ringkasan singkat mengenai judul dokumen dan terkadang sebagian teksnya.




Referensi:

https://armunantos.wordpress.com/2013/02/17/uts-information-retrieval/

http://www.kumpulancara.com/2009/08/8-trik-memperoleh-ranking-pada-search.html#axzz18KCnFqv9



