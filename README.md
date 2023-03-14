# TP1DPBO2023
##### Saya Muhammad Rizki NIM 2107922 mengerjakan soal TP 1 dalam mata kuliah Desain Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

### Diagram UML Program
---------------
![TP1 drawio](https://user-images.githubusercontent.com/100481579/224930423-805bcc0d-a9d2-40d5-ace1-7509756b4c4a.png)

### Penjelasan kelas
---------------
1. Human
  * kelas yang merepresentasikan manusia
  * Atribut
    - _nik: atribut ini berisi nomor identitas kependudukan dari manusia dan dianggap sebagai identitas unik dari setiap manusia. Atribut ini merupakan variabel bertipe       data string yang diterapkan sebagai parameter pertama dalam metode init() dan hanya dapat diakses melalui metode get_nik() dan set_nik().
    - _nama: atribut ini berisi nama manusia dan merupakan variabel bertipe data string yang diterapkan sebagai parameter kedua dalam metode init() dan hanya dapat       diakses melalui metode get_nama() dan set_nama().
    - _jenis_kelamin: atribut ini berisi jenis kelamin manusia dan merupakan variabel bertipe data string yang diterapkan sebagai parameter ketiga dalam metode init() dan hanya dapat diakses melalui metode get_jenis_kelamin() dan set_jenis_kelamin().
    * method
    - set & get untuk akses tiap atribut
    - eat(): metode ini mencetak pesan yang menyatakan bahwa manusia sedang makan.
    - drink(): metode ini mencetak pesan yang menyatakan bahwa manusia sedang minum.
    - sleep(): metode ini mencetak pesan yang menyatakan bahwa manusia sedang tidur.
 2. Sivitas Akademik
  * merupakan kelas turunan dari kelas Human, yang merepresentasikan sekelompok orang yang terlibat dalam kegiatan akademik
  * Atribut 
    - _asal_universitas: atribut ini berisi informasi mengenai universitas atau perguruan tinggi yang diwakili oleh sivitas akademik tersebut.
    - _email_edu: atribut ini berisi informasi mengenai email akademik yang dimiliki oleh sivitas akademik.
  * Method
    - set & get untuk akses tiap atribut
3. Mahasiswa
  * merupakan kelas turunan dari SivitasAkademik dan Human. Class ini merepresentasikan seorang mahasiswa
  * Atribut
    - _nim: nomor induk mahasiswa.
    - _fakultas: fakultas tempat mahasiswa tersebut belajar.
    - _prodi: program studi yang diambil oleh mahasiswa tersebut.
    - _laptop: jenis laptop yang dimiliki oleh mahasiswa.
    - _textbook: daftar buku-buku teks yang dimiliki oleh mahasiswa.
    - _nilai_matkul: dictionary yang berisi nilai dari setiap mata kuliah yang diambil oleh mahasiswa.
  * Method
    - set & get untuk akses tiap atribut
    - tambah_textbook(textbook): menambahkan buku teks baru ke dalam daftar _textbook.
    - get_all_data(): menampilkan seluruh data yang dimiliki oleh mahasiswa, seperti nama, NIK, NIM, jenis kelamin, fakultas, program studi, asal universitas, email edu, laptop, daftar textbook, dan nilai matkul.
4. BEM
  * merepresentasikan organisasi BEM
  *atribut
    -__nama_kabinet: atribut private yang berisi nama kabinet BEM.
    - __periode: atribut private yang berisi periode kepengurusan BEM.
    - __anggota: atribut private yang berisi list objek Orang yang menjadi anggota BEM.
  * Method
    - set & get untuk akses tiap atribut
    - tambah_anggota(): method untuk menambahkan objek Orang ke dalam list __anggota.
    - get_all_data(): method untuk menampilkan data kabinet BEM seperti nama kabinet dan periode kepengurusan.
    - tampilkan_anggota(): method untuk menampilkan daftar anggota BEM beserta peran yang diemban dalam kabinet.
5. BEM member
  * merupakan kelas turunan dari Mahasiswa. merepresentasikan mahasiswa yang juga sebagai anggota BEM
  * atribut
    - planning: list kosong yang akan berisi program-program yang direncanakan
    - implementing: list kosong yang akan berisi program-program yang sedang diimplementasikan
    - evaluations: list kosong yang akan berisi program-program yang telah dievaluasi
    - BEM: atribut yang akan menunjukkan keanggotaan BEM dari seorang mahasiswa
    - role: atribut yang akan menunjukkan peran seorang mahasiswa di dalam BEM
  * Method
    - set & get untuk akses tiap atribut
    - tambah_planning(): digunakan untuk menambahkan program-program yang direncanakan ke dalam atribut self._planning
    - planning_programs(): digunakan untuk menampilkan pesan bahwa seorang mahasiswa sedang merencanakan program-program tertentu
    - tambah_implementing(): digunakan untuk menambahkan program-program yang sedang diimplementasikan ke dalam atribut self._implementing
    - implementing_programs(): digunakan untuk menampilkan pesan bahwa seorang mahasiswa sedang mengimplementasikan program-program tertentu
    - tambah_evaluations(): digunakan untuk menambahkan program-program yang telah dievaluasi ke dalam atribut self._evaluations
    - attending_evaluations(): digunakan untuk menampilkan pesan bahwa seorang mahasiswa sedang menghadiri evaluasi program-program tertentu.
    
  
