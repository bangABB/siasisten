TUGAS 9


Menjawab beberapa pertanyaan berikut pada README.md pada root folder:
    1. Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?
        - jawabannya bisa, dengan menggunakan fungsi jsonDecode dari pustaka dart:convert yang dapat mengubah string JSON menjadi Map . Kemudian, kita bisa mengakses nilai-nilai yang kita butuhkan dari map tersebut dengan menggunakan kunci-kunci yang sesuai. 
    2. Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.
        - CookieRequest adalah kelas yang digunakan untuk mengelola cookies dalam aplikasi Flutter. Fungsi utamanya adalah untuk menyimpan dan mengambil cookies yang digunakan saat berinteraksi dengan server web. Instance CookieRequest perlu dibagikan ke semua komponen di aplikasi Flutter karena cookies sering digunakan untuk otentikasi pengguna, pelacakan sesi, dan menyimpan preferensi pengguna. Dengan membagikan instance yang sama, kita memastikan bahwa semua komponen aplikasi memiliki akses ke informasi yang sama dan konsisten.
    3. Jelaskan mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter.
        - a. ambil data json dengan post atau get 
          b. data json diuraikan ke bentuk paket objek atau struktur data, di tutorial kita menggunakan jsonDecode()
          c. objek dapat langsung digunakan di flutter, kita listviewkan atau card
    4. Jelaskan mekanisme autentikasi dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter.
        - 
        - Pertama, pengguna memasukkan data akun mereka (biasanya email dan kata sandi) melalui form di aplikasi Flutter.
        - Kedua, data ini kemudian dikirim ke server Django, biasanya melalui HTTP POST.
        - Ketiga, Django kemudian memverifikasi data ini dengan data yang ada di database. Jika data cocok, Django akan mengirimkan balasan yang    mengkonfirmasi bahwa autentikasi berhasil.
        - Keempat, aplikasi Flutter kemudian menerima balasan ini dan, jika autentikasi berhasil, menu ditampilkan kepada pengguna. Jika autentikasi gagal, pesan kesalahan ditampilkan.
    5. Sebutkan seluruh widget yang kamu pakai pada tugas ini dan jelaskan fungsinya masing-masing.
        - Tidak kelar
    6. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step
        - Tidak Kelar




TUGAS 8
1. Push: tanpa mengganti layar sebelumnya, Replace : menggantikan layar yang skerang di show
2.  - Container  
        widget yang dapat mengandung widget lain dan memberikan cara sederhana untuk mengatur properti seperti padding, margin, dan dekorasi.
    - row column
        baris dan kolom, seperti namanya. untuk mengatur tata letak dengan susunan baris atau kolom dari widget anak.
    - listView 
        viewnya berupa list. Ideal untuk menampilkan daftar item scrollable seperti daftar kontak, berita, atau item lainnya.
    - stack
        mengatur widget anak secara tumpuk, yang berarti satu di atas yang lain. Berguna untuk menyusun widget secara bersamaan, seperti menempatkan teks di atas gambar atau membuat tata letak kompleks.
    - gridview
        GridView adalah widget yang menampilkan anak-anak dalam tata letak grid. Berguna untuk menampilkan item dalam bentuk grid, seperti galeri foto atau aplikasi e-commerce dengan produk dalam grid.
    - expanded and felxible 
        Expanded dan Flexible adalah widget yang memungkinkan anak-anaknya memperluas ruang yang tersedia. Digunakan untuk memberikan fleksibilitas dalam pengaturan tata letak, terutama dalam Row dan Column.
3. text dan integer. karna text unutk nama sedangkan integer untuk harga dan gaji
4. lean Architecture adalah konsep arsitektur perangkat lunak yang bertujuan untuk memisahkan komponen-komponen utama aplikasi agar lebih terisolasi, mudah diuji, dan fleksibel terhadap perubahan. Terdapat beberapa prinsip utama dalam Clean Architecture, seperti Dependency Rule, Entities, Use Cases, Interface Adapters, dan Frameworks & Drivers. Penerapan Clean Architecture pada aplikasi Flutter melibatkan penggunaan paket atau struktur folder tertentu dan pemahaman terhadap prinsip-prinsip tersebut.
5. membuat input formnya lalu memvavlidasi input, seperti tidak boleh kosong. lalu mengimplementasikannya dengan membuat action berdasarkan nama.
    




TUGAS 7

1. StatelessWidget adalah jenis widget dalam pengembangan aplikasi Flutter yang tidak memiliki keadaan internal. Ini berarti setelah dibangun, kontennya tidak akan berubah dan tidak dapat berinteraksi dengan data yang berubah. StatelessWidget lebih cocok digunakan untuk menggambar komponen yang statis atau tidak berubah selama aplikasi berjalan, seperti tampilan yang tetap konsisten. Sedangkan, stateful widget adalah widget yang memiliki keadaan internal yang dapat berubah selama aplikasi berjalan. Widget ini memiliki metode build yang dapat dipanggil ulang ketika data yang terkait berubah, sehingga memungkinkan tampilan diperbarui sesuai dengan perubahan data. StatefulWidget sangat cocok digunakan untuk menggambar komponen yang memerlukan interaksi pengguna atau yang perlu diperbarui secara dinamis, seperti daftar item yang dapat ditambahkan, dihapus, atau diperbarui sesuai dengan input atau perubahan data.

Dalam penggunaan nya stateless widget digunakan untuk konten statis, sementara stateful widget digunakan untuk konten yang dapat berubah. 

2. Sebutkan seluruh widget yang kamu gunakan untuk menyelesaikan tugas ini dan jelaskan fungsinya masing-masing.
- MaterialApp: Widget yang menyediakan konfigurasi dasar untuk aplikasi berbasis material design, seperti tema, navigasi, dan judul.
- Scaffold: Widget yang menyediakan struktur visual untuk halaman, seperti app bar, body, dan floating action button.
- AppBar: Widget yang menampilkan app bar, yaitu sebuah panel horizontal di bagian atas halaman yang biasanya berisi judul, ikon, dan menu.
- Text: Widget yang menampilkan teks dengan gaya tertentu.
SingleChildScrollView: Widget yang memungkinkan konten untuk di-scroll secara vertikal jika konten lebih panjang dari layar.
- Padding: Widget yang menambahkan jarak antara konten dan tepi widget lainnya.
- Column: Widget yang menampilkan anak-anaknya dalam arah vertikal.
- GridView: Widget yang menampilkan anak-anaknya dalam grid dua dimensi.
- ShopItem: Widget yang saya buat sendiri untuk merepresentasikan item yang tersedia di toko, yang memiliki nama dan ikon.
- ShopCard: Widget yang saya buat sendiri untuk menampilkan item dalam bentuk kartu, yang memiliki warna latar belakang, ikon, dan teks.
- Material: Widget yang menambahkan efek material design pada widget lainnya, seperti elevasi, warna, dan bentuk.
- InkWell: Widget yang menambahkan efek air pada widget material saat ditekan, dan juga dapat menangani gesture seperti onTap.
- Container: Widget yang dapat menampung widget lainnya dengan berbagai properti, seperti padding, margin, dekorasi, dan ukuran.
- Center: Widget yang menempatkan widget anaknya di tengah-tengah widget induknya.
- Icon: Widget yang menampilkan ikon berdasarkan kumpulan ikon yang tersedia.
- ScaffoldMessenger: Widget yang dapat menampilkan snackbar di bawah scaffold.
- SnackBar: Widget yang menampilkan pesan singkat di bagian bawah layar.

3. Pada setp ini pertama saya membuat 
 flutter create < >

 lalu saya mengimport dart dan membuat file baru dengan nama menu.dart, selanjutnya saya
 mengikuti tutorial yang telah banyak ada + meminta diajarkan oleh teman hehe :D terimakasih 