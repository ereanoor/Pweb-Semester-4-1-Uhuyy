1. index.html
Struktur Metadata & Dependensi: Menggunakan standar HTML5 dengan optimasi viewport untuk responsivitas. Proyek ini mengintegrasikan AOS.js melalui CDN untuk manajemen animasi berbasis scroll dan FontAwesome untuk penyediaan aset ikon vektor pada antarmuka.

Sistem Navigasi: Implementasi Sticky Header dengan teknik position: fixed. Navigasi menggunakan anchor links (#) yang bekerja sama dengan properti CSS scroll-behavior: smooth untuk menciptakan pengalaman navigasi satu halaman (Single Page Application style).

Hero Section & Typewriter Logic: Menggunakan elemen kontainer untuk tata letak terpusat. Fitur utama di sini adalah manipulasi DOM pada elemen dengan ID typewriter. Logika JavaScript di akhir file mengatur siklus array string, durasi jeda, dan efek penghapusan karakter untuk mensimulasikan pengetikan manual.

Layout Grid Hobi: Memanfaatkan sistem Grid yang dinamis. Setiap elemen kartu dibungkus dalam tag jangkar (<a>) yang mengarah ke file HTML internal. Atribut data-aos disematkan pada tiap kartu untuk mentrigger animasi masuk saat fungsi AOS.init() dijalankan.

Social Integration: Footer disusun menggunakan kontainer fleksibel yang memuat tautan absolut. Atribut target="_blank" digunakan secara konsisten pada semua tautan eksternal (LinkedIn, GitHub, dll.) untuk menjaga retensi pengguna pada halaman utama.

2. membaca.html
Arsitektur Sub-Halaman: Menggunakan kelas CSS sub-page untuk merubah skema tata letak dari full-height menjadi konten berbasis alur (flow-based).

Komponen Detail Box: Implementasi elemen .detail-box yang menggunakan border-left tebal untuk penekanan visual. Secara teknis, ini digunakan untuk mengelompokkan konten tematik terkait genre Kingdom Building.

Navigasi Rekursif: Terdapat komponen tombol kembali yang menggunakan jalur relatif index.html#hobbies. Ini memastikan fungsi "Back" mengarahkan pengguna tepat ke bagian galeri hobi di halaman utama, bukan kembali ke atas halaman.

3. bermusik.html
Audio Engine: Menggunakan tag standar <audio> dengan ID myAudio. File sumber diarahkan ke path lokal sounds/lagu.mp3. Secara teknis, kontrol autoplay dimatikan untuk mengikuti kebijakan browser modern.

DOM Interaction: JavaScript digunakan untuk menjembatani elemen UI (tombol) dengan API Audio. Fungsi event listener click menjalankan logika kondisional: jika audio dalam status paused, panggil metode .play(), jika tidak, panggil .pause().

Sync Animasi: Skrip juga memanipulasi kelas CSS pada ikon disk-icon. Penambahan kelas .fa-spin secara dinamis saat musik diputar memberikan indikator visual state audio yang aktif kepada pengguna.

4. ngoding.html
Semantic Content: Berfokus pada penggunaan tag paragraf yang terstruktur untuk membangun narasi profesional.

Thematic Iconography: Menggunakan kelas ikon spesifik (fa-brain) untuk memperkuat konteks visual mengenai spesialisasi Artificial Intelligence. Secara struktur, file ini mengikuti pola reusable components dari halaman detail lainnya untuk menjaga konsistensi kode.

5. gaming.html
Performance Tracking: Bagian ini memanfaatkan elemen .detail-box untuk menampilkan poin-poin pencapaian kompetitif. Secara teknis, penggunaan elemen <strong> digunakan untuk menekankan kata kunci seperti nama game dan peringkat leaderboard demi optimasi keterbacaan (skimmability).
