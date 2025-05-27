# Laporan Proyek Machine Learning -Tiesya Andriani Ramadhanti
## Project Overview
### Latar Belakang
Dalam era digital saat ini, jumlah konten hiburan seperti film terus meningkat secara signifikan. Pengguna sering kali menghadapi kesulitan dalam memilih film yang sesuai dengan preferensi mereka akibat banyaknya pilihan yang tersedia. Oleh karena itu, dibutuhkan sebuah sistem yang dapat membantu pengguna untuk menemukan film yang relevan dan sesuai dengan minat mereka secara otomatis. Salah satu solusi yang umum digunakan adalah **sistem rekomendasi film** (*movie recommendation system*).Sistem rekomendasi telah menjadi komponen penting dalam berbagai platform digital seperti Netflix, YouTube, dan Amazon. Sistem ini memanfaatkan teknik kecerdasan buatan dan pembelajaran mesin untuk menganalisis data historis pengguna dan menghasilkan rekomendasi yang dipersonalisasi.Pada proyek ini, dibangun sebuah sistem rekomendasi film menggunakan **dataset dari Kaggle** yang berjudul [*Movie Recommendation Data*](https://www.kaggle.com/datasets/rohan4050/movie-recommendation-data). Dataset ini berisi informasi mengenai pengguna, film, dan rating yang diberikan, yang dapat digunakan untuk membangun model rekomendasi berbasis konten (*content-based filtering*) maupun berbasis kolaboratif (*collaborative filtering*).
Tujuan dari proyek ini adalah untuk:
- Menganalisis preferensi pengguna terhadap film berdasarkan data rating.
- Mengembangkan model yang mampu merekomendasikan film secara personal.
- Menyediakan wawasan dari hasil rekomendasi yang dihasilkan sistem.

Dengan adanya sistem ini, diharapkan pengguna dapat memperoleh pengalaman menonton yang lebih baik dan efisien melalui saran film yang sesuai dengan selera mereka.

### Daftar Referensi
Yang, Y., & Woradit, K. (2025). Hybrid Movie Recommendation System with Content-Based and Memory-Based Collaborative Filtering based on Deep Neural Network. *ECTI Transactions on Electrical Engineering, Electronics, and Communications*, 23(1), 131–139. https://doi.org/10.37936/ecti-eec.2525231.255176

## Bussiness Understanding
### Problem Statement
Dengan semakin banyaknya jumlah film yang tersedia setiap tahunnya, pengguna menghadapi tantangan dalam memilih film yang sesuai dengan preferensi mereka. Tanpa sistem rekomendasi yang baik, pengguna bisa merasa kewalahan oleh banyaknya pilihan dan akhirnya menghabiskan waktu lebih lama untuk memilih daripada menonton.
1. Banyak pengguna mengalami kesulitan dalam menemukan film yang sesuai dengan minat atau preferensi pribadi mereka akibat banyaknya pilihan yang tersedia.
2. Film-film berkualitas, khususnya film lama atau kurang populer, seringkali tidak muncul dalam rekomendasi standar dan kurang terekspos oleh pengguna.
3. Belum tersedia sistem rekomendasi yang secara optimal menggabungkan pendekatan *collaborative filtering* dan *content-based filtering* untuk memberikan saran film yang akurat dan personal.

### Goals
Tujuan dari proyek sistem rekomendasi film ini adalah sebagai berikut:
1. Mengembangkan sistem rekomendasi film berbasis data yang mampu memahami preferensi unik dari masing-masing pengguna.
2. Meningkatkan visibilitas film-film berkualitas yang jarang terekspos melalui mekanisme rekomendasi yang lebih cerdas.
3. Menciptakan sistem rekomendasi yang mengintegrasikan metode *collaborative* dan *content-based filtering* untuk menghasilkan saran film yang lebih relevan dan personal.
Dengan tercapainya tujuan ini, sistem diharapkan mampu meningkatkan pengalaman pengguna dalam menemukan film yang relevan dengan cepat dan efisien.

### Solution Approach

Untuk mencapai tujuan di atas, sistem akan dikembangkan dengan mengimplementasikan lebih dari satu pendekatan rekomendasi yang saling melengkapi:

- **Content-Based Filtering**  
Content-Based Filtering menganalisis karakteristik dari film yang disukai oleh pengguna, seperti judul, genre, dan tahun rilis. Sistem kemudian merekomendasikan film lain yang memiliki fitur serupa berdasarkan kemiripan kontennya, sehingga pengguna mendapatkan saran film yang sejalan dengan preferensi pribadi mereka.

- **Collaborative Filtering**  
Collaborative Filtering membangun sistem rekomendasi berdasarkan penilaian atau rating dari pengguna lain. Sistem ini akan menyarankan film yang disukai oleh pengguna dengan preferensi yang mirip, bahkan jika pengguna tersebut belum pernah menonton atau memberikan rating terhadap film tersebut sebelumnya.

## Data Understanding
Dataset yang digunakan dalam proyek ini berjudul [*Movie Recommendation Data*](https://www.kaggle.com/datasets/rohan4050/movie-recommendation-data). dan tersedia di platform Kaggle . Dataset ini berisi data film, rating pengguna, serta informasi terkait yang mendukung pengembangan sistem rekomendasi film.
Terdapat beberapa file utama yang digunakan, yaitu:  
- **movies.csv**, yang berisi informasi film seperti judul dan genre,  
- **ratings.csv**, yang berisi data rating yang diberikan oleh pengguna kepada film,  
- **tags.csv**, yang berisi tag atau label tambahan dari pengguna untuk film tertentu,  
- **links.csv**, yang menghubungkan ID film dalam dataset dengan ID film di platform lain seperti IMDb dan TMDb.






