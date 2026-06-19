# Netflix-Content-Analysis-PowerBI
Netflix Content Analysis Dashboard Using Power BI
Project Overview
Project ini merupakan analisis data konten Netflix menggunakan Microsoft Power BI yang bertujuan untuk memahami pola distribusi konten, tren genre, rating, serta perkembangan jumlah konten berdasarkan waktu.
Dataset yang dianalisis terdiri dari 6.234 konten Netflix yang mencakup Movie dan TV Show. Melalui proses data cleaning, data modeling, pembuatan DAX measure, dan dashboard interaktif, data mentah diolah menjadi insight yang dapat membantu memahami karakteristik konten Netflix.
Project ini menerapkan alur kerja Data Analyst mulai dari tahap persiapan data hingga menghasilkan visualisasi dan insight berbasis data.
Project Objectives
Tujuan project ini adalah menganalisis distribusi Movie dan TV Show, mengidentifikasi genre yang dominan, menganalisis pertumbuhan konten Netflix berdasarkan tahun, memahami distribusi rating, dan membuat dashboard yang mendukung analisis berbasis data.
Berdasarkan hasil analisis Netflix memiliki total 6.234 konten dengan 4.110 konten merupakan Movie yang menunjukan bahwa katalog Netflix lebih di dominasi oleh film dibandingkan TV Show.
Dataset
Dataset yang digunakan adalah Netflix Titles Dataset. Dataset berisi informasi show_id, type, title, director, cast, country, date_added, release_year, rating, duration, genre, dan description.
Data Cleaning Process
Proses data cleaning dilakukan menggunakan Power Query untuk memastikan data siap dianalisis. Tahapan yang dilakukan:
1.	Handling Missing Values
Melakukan pengecekan dan penanganan nilai kosong pada beberapa atribut seperti: date_added, rating, country dan director. Nilai kosong ditangani sesuai kebutuhan analisis agar tidak mengganggu hasil visualisasi.
2.	Data Type Transformation
Melakukan perubahan tipe data:
•	date_added diubah menjadi tipe Date. 
•	release_year diubah menjadi Whole Number. 
•	duration dipisahkan menjadi nilai numerik dan satuan durasi.
3.	Duration Transformation
Kolom duration awal memiliki format campuran seperti 90 min dan juga 3 Seasons. Oelh sebab itu dilakukan pemisahan menjadi Duration Value dan Duration Unit, sehingga dapat digunakan untuk perhitungan rata-rata durasi.
4.	Date Transformation
Kolom date_added dikembangkan menjadi atribut waktu yaitu Added Year dan Added Month untuk mendukung analisis tren penambahan konten Netflix.
Data Modeling
Project ini menggunakan konsep star schema. Fact_Netflix digunakan sebagai fact table, sedangkan Dim_Date, Dim_Genre, Dim_Rating, dan Dim_Country digunakan sebagai dimension table. Bridge_Genre digunakan untuk menangani hubungan many-to-many antara konten dan genre.
DAX Measures
DAX measure yang dibuat meliputi Total Content untuk menghitung jumlah konten, Total Movies untuk menghitung jumlah film, Total TV Shows untuk menghitung jumlah serial, dan Average Duration untuk menghitung rata-rata durasi.
Dashboard Features
Dashboard menampilkan KPI utama, perbandingan Movie dan TV Show, Top 10 Genre, tren pertumbuhan konten berdasarkan tahun, serta filter interaktif berdasarkan tahun, rating, dan tipe konten.
Key Insights
Berdasarkan hasil analisis:
•	Netflix memiliki 6.234 total konten, dengan mayoritas berupa Movie sebanyak 4.110 konten. 
•	Movie memiliki proporsi lebih besar dibandingkan TV Show dalam katalog Netflix. 
•	Genre International Movies dan Drama termasuk kategori dengan jumlah konten tertinggi. 
•	Pertumbuhan jumlah konten Netflix mengalami peningkatan signifikan setelah tahun 2015. 
•	Dashboard membantu memahami pola distribusi konten berdasarkan waktu, genre, rating, dan tipe konten.
Conclusion
Project ini menunjukkan penerapan proses analisis data secara lengkap mulai dari data cleaning, data modeling, DAX calculation, hingga dashboard visualization menggunakan Power BI.
