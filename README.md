# TP1DPBO2023
##### Saya Muhammad Rizki NIM 2107922 mengerjakan soal TP 1 dalam mata kuliah Desain Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

### Diagram UML Program
---------------
![TP1 drawio](https://user-images.githubusercontent.com/100481579/224930423-805bcc0d-a9d2-40d5-ace1-7509756b4c4a.png)
---------------
### Penjelasan kelas
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
 6. English Club
   * merepresentasikan organisasi english club
   * Atribut
     - __nama_club : digunakan untuk menyimpan nama English Club.
     - _deskripsi : digunakan untuk menyimpan deskripsi dari English Club.
     - __anggota : digunakan untuk menyimpan daftar anggota English Club.
   * Method
     - set & get untuk akses tiap atribut
     - tambah_anggota(self, anggota_baru) : method yang digunakan untuk menambahkan anggota baru ke dalam list __anggota.
     - get_all_data(self) : method yang digunakan untuk menampilkan informasi dari objek EnglishClub, yaitu nama club dan deskripsi.
     - tampilkan_anggota(self) : method yang digunakan untuk menampilkan daftar anggota English Club beserta dengan role-nya.
7. English Club Member
  * Merupakan turunan dari kelas mahasiswa, merepresentasikan mahasiswa yang termasuk dalam anggota english club
  * Atribut
    - _role : digunakan untuk menyimpan peran (role) anggota di English Club, nilai defaultnya adalah "member".
    - _EnglishClub : digunakan untuk menyimpan informasi mengenai club yang diikuti oleh anggota ini.
  * Method
    - set & get untuk akses tiap atribut
    - advance_language(self) : method yang digunakan untuk menampilkan pesan bahwa anggota English Club ini sedang meningkatkan kemampuan bahasa Inggrisnya.
    - plan_program(self) : method yang digunakan untuk menampilkan pesan bahwa anggota English Club ini sedang merencanakan program untuk club yang diikutinya. Method ini memanggil method get_nama() untuk mendapatkan nama anggota, dan memanggil method get_club_name() untuk mendapatkan nama English Club yang diikuti oleh anggota ini.
8. Assistand
  * Merupakan turunan dari kelas mahasiswa
  * Atribut
    - _dosen : digunakan untuk menyimpan informasi mengenai dosen yang diasisten oleh mahasiswa ini.
  * Method
    - set & get untuk akses tiap atribut
    - mengajar(self) : method yang digunakan untuk menampilkan pesan bahwa mahasiswa ini sedang mengajar sebagai asisten dari seorang dosen. 
    - memberikan_tugas(self) : method yang digunakan untuk menampilkan pesan bahwa mahasiswa ini sedang memberikan tugas sebagai asisten dari seorang dosen.
9. Dosen
  * merupakan turunan kelas sivitas akademik, merepresentasikan dosen dalam kegiatan akademika
  * Atribut
    - nip: nomor induk pegawai dosen
    - fakultas: fakultas tempat dosen bekerja
    - pend_terakhir: pendidikan terakhir dosen
    - keahlian: keahlian dosen
    - laptop: laptop yang digunakan oleh dosen
    - whiteBoardMarker: alat tulis yang digunakan oleh dosen
    - matkul_diampu: list mata kuliah yang diampu oleh dosen
  * Method
    - set & get untuk akses tiap atribut
    - add_matkul_diampu(matkul): menambahkan mata kuliah matkul ke dalam list mata kuliah yang diampu oleh dosen
    - get_all_data(): mencetak seluruh atribut dosen beserta nilainya.
    - beri_nilai(mhs, matkul, nilai): memberikan nilai pada mata kuliah matkul untuk mahasiswa mhs dengan nilai nilai. Jika matkul tidak termasuk mata kuliah yang diampu oleh dosen, maka akan muncul pesan bahwa nilai tidak dapat diberikan.
---------------
### Alur Program
* Program menampilkan 4 menu utama
![image](https://user-images.githubusercontent.com/100481579/224984185-a4a83ff7-0226-4123-a27e-c1f3d52ad402.png)
* jika memilih 1, maka program akan menampilkan semua karakter yang dimiliki
* jika memilih 2 maka program akan memberikan menu informasi tentang BEM
* jika memilik 3 maka program akan memberikan menu informasi tentang english club
* semua menu berada dalam sebuah loop, loop hanya akan berakhir jika user memilih opsi exit
---------------
### interaksi dalam class dan antar class
1. Kelas Mahasiswa
  * Mahasiswa hanya mendapat nilai dari dosen
2. BEM member
  * Setiap BEM member memiliki 3 array tahapan untuk actifity mereka, yaitu:
    - Planning -> adalah array dimana proker direncanakan
    - implementing -> diisi berdasarkan proker pada array planning. **tidak dapat mengimplementasikan proker jika belum di-planing!
    - evaluation -> diisi berdasarkan proker pada array implementing. **tidak dapat mengimplementasikan proker jika belum di-implementing! 
3. Dosen
  * Dosen dapat mengisi nilai ke semua mahasiswa dengan syarat **dosen memberi nilai pada mata kuliah yang dia ampu saja

---------------
### Dokumentasi
![image](https://user-images.githubusercontent.com/100481579/224987755-a65f74a1-c363-4f28-8e3d-62182d58ec99.png)
![image](https://user-images.githubusercontent.com/100481579/224988050-46037b87-4270-4737-afd3-35d08e522aa1.png)
![image](https://user-images.githubusercontent.com/100481579/224988126-f44dd394-28ce-4f62-b675-480d73847dc8.png)
![image](https://user-images.githubusercontent.com/100481579/224988631-6501d3e8-87dd-4412-9e6f-ef24c638bca7.png)
![image](https://user-images.githubusercontent.com/100481579/224989473-61a8f8f6-b84e-4006-b2df-efe163fc5893.png)
![image](https://user-images.githubusercontent.com/100481579/224990054-65aa798c-86ab-4c0f-a6fb-37f2c4c72e30.png)
![image](https://user-images.githubusercontent.com/100481579/224990139-a2d5d4c2-899b-40d3-b149-c15e8e23fc49.png)







