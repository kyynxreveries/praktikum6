DAFTAR ISI
==========
- [LAPORAN PRAKTIKUM 6](#laporan-praktikum-6)   
    - [CODE PROGRAM DAFTAR NILAI](#code-program-daftar-nilai)
    - [FLOWCHART DAFTAR NILAI](#flowchart-daftar-nilai)
    - [KESIMPULAN](#kesimpulan)


# LAPORAN PRAKTIKUM 6


## CODE PROGRAM DAFTAR NILAI
### Step 1: Inisialisasi Data
Tambahkan variabel data_mahasiswa sebagai list kosong yang digunakan untuk menyimpan data mahasiswa, setiap elemen dalam list adalah dictionary yang berisi informasi mahasiswa berupa Nilai Mahasiswa untuk kasus ini :

![step1](https://github.com/user-attachments/assets/13c3f1f8-be50-4595-8b36-6cbee733d1e1)

### Step 2: Fungsi Tambah ()
Fungsi ini untuk menambahkan data mahasiswa baru yang akan diproses sebagai :

* Meminta pengguna memasukkan nama dan nilai mahasiswa.
* Data yang dimasukkan disimpan dalam bentuk dictionary {"nama": nama, "nilai": nilai}.
* Dictionary ini ditambahkan ke dalam list data_mahasiswa menggunakan .append().

![step2](https://github.com/user-attachments/assets/23fc8ccc-cf46-4c3f-ba24-b941c2df252a)

### step 3: Fungsi Tampilkan ()
Fungsi ini digunakan untuk menampilkan data nilai mahasiswa ke dalam data_mahasiswa. Tujuan dapat menampilkan seluruh data mahasiswa. Menu ini mampu mengecek apakah data_mahasiswa kosong, Jika tidak kosong data ditampilkan dalam bentuk tabel sesuai data yang telah ditambahkan, Menggunakan enumerate untuk memberikan nomor pada setiap mahasiswa dalam daftar :

![step3](https://github.com/user-attachments/assets/594956dd-8495-4b62-8052-fdc90d254a7a)

### Step 4: Fungsi Hapus (nama)
Menghapus data mahasiswa berdasarkan nama yang dimasukan/input, sebagai proses menggunakan list comprehension untuk membuat daftar baru yang tidak berisi mahasiswa dengan nama yang dimasukkan, variabel data_mahasiswa diperbarui dengan daftar baru ini :

![step4](https://github.com/user-attachments/assets/bf36c1b8-9404-49ca-bb35-0b4f0de6e302)

### Step 5: Fungsi Ubah (nama)
Fungsi yang akan mengubah nilai mahasiswa berdasarkan nama yang dimasukan/input, mencari data mahasiswa dengan nama tertentu di dalam data_mahasiswa. Jika data ditemukan, maka nilai mahasiswa tersebut diperbarui sesuai input pengguna :

![step5](https://github.com/user-attachments/assets/c599f344-82ef-4c8f-852a-232ee80683df)


### Step 6: Fungsi Menu ()
Menyediakan Tampilan menu sebagai opsi pengguna, menggunakan perulangan while untuk terus menampilkan menu namun untuk menghentikan program masukan break sebagai perhentian :

Pilihan menu:

* 1: Memanggil fungsi tambah().
* 2: Memanggil fungsi tampilkan().
* 3: Memanggil fungsi hapus(nama).
* 4: Memanggil fungsi ubah(nama).
* 5: Menghentikan program.

![step6 1](https://github.com/user-attachments/assets/ce3dcd0a-9f05-4caa-a65b-08ae8ca05736)

![step6 2](https://github.com/user-attachments/assets/ed918921-7b72-4f5d-b97f-25075ff3ab7e)

### Step 7: Closed Program
Pakai menu() untuk memulai sebuah program ketika dirun :

![step7](https://github.com/user-attachments/assets/01c87280-ccfe-4ad1-a26e-e959d983ed0b)

### Step 8: Run Program
Tahap akhir adalah uji coba code program yang sudah dibuat.

# CONTOH OUTPUT

### 1. Tambah Data
Pertama saya mencoba menambahkan data mahasiswa pada tabel, dengan menginputkan '1' untuk menambahkan data mahasiswa.

* Untuk perawalan, mencoba memasukan satu data mahasiswa :
  * Nama : Rizky Maulana
  * Nilai : 85

### 2. Tampilkan Data
Selanjutnya, kondisi kedua menginputkan '2' untuk melihat daftar data mahasiswa pada tabel, namun dari kondisi sebelumnya yang sudah menambahkan data mahasiswa saya coba tambahkan 4 data mahasiswa lagi. maka akan terlihat pada isi tabel :

![output 2 0](https://github.com/user-attachments/assets/15f2cd38-f772-42bd-b1b1-de2a31b94a4b)

### 3. Hapus Data
Kondisi ketiga, kita mencoba menghapus sebuah data mahasiswa dengan menginputkan '3' untuk menghapuskan data mahasiswa lalu user diminta memasukan nama mahasiswa yang akan dihapus :

![output 3](https://github.com/user-attachments/assets/67d65614-200f-47b6-a56b-9f0ca35ab952)

### 4. Ubah Data
Masuk kondisi keempat saya akan coba mengubah data, ada data yang salah diinputkan pada Nilai Mahasiswa 81 diubah menjadi 88, sebelum itu inputkan '4' untuk mengubah maka akan ditampilkan daftar nilai tabel dan diminta untuk memasukan nama mahasiswa yang ingin diubah data nilai -nya. User diminta memasukan kembali data valid yang akan diubah.

* Coba memasukan data mahasiswa berikut :
  * Nama : Rakha Ghani Ghani Ghani
  * Nilai : 88

![output 4](https://github.com/user-attachments/assets/cc6a83bb-bb81-4b96-adab-0a9bf6a548a5)

### 5. Keluar
Jika semua data atau program input sudah selesai semua, user dapat menginputkan 5 untuk keluar dari progam :

![output 5](https://github.com/user-attachments/assets/990d819f-7362-4cc2-92ad-d363c171953f)

# FLOWCHART DAFTAR NILAI

![flowchart](https://github.com/user-attachments/assets/17876fc1-c60a-4b22-8252-324dcb853fb0)

### Step 1 :
Titik mulai sebuah program atau alur.

### Step 2 :
lalu lakukan inisialisasi dengan menampilkan menu yang tersedia.

### Step 3 :
Inputkan code menu yang ingin dilakukan, setiap code berisi :

1. Tambah,
2. Tampilkan,
3. Hapus,
4. Ubah,
5. Keluar.

### Step 4 :
Dalam kasus ini semua kemgkinan dapat terjadi, kondisi yang diperlukan sesuai apa yang akan diinoutkan user.

* Jika Tampilkan, maka user akan di tampilkan sebuah tabel dari daftar nilai, namun jika tabel belum ada isi/kosong maka akan tampil Belum ada data, jika ada maka ditampilkan sebuah data nilai mahasiswa. Setelah tampilkan data maka akan kembali menuju inisialisasi menu.

* Jika Tambah, user diminta memasukan sebuah data yang berupa :

  * Nama
  * Nilai
Lalu User akan diarahkan kembali ke inisialiasi menu.

* Jika Ubah, sama dengan Tampilkan jika tidak ada data nilai maka akan tampil tidak ada data nilai namun Ubah kalau ada data nilai user diminta menginputkan
 Nama Mahasiswa yang akan diubah, setelah itu diminta untuk mengisi atau menginputkan data valid yang diubah. Setelah itu user kembali ke inisialisasi menu.

* Jika Hapus, user akan ditampilkan daftar nilai lalu diminta memasukan sebuah Nama yang ingin dihapus dari daftar. Setelah itu kembali ke inisialisasi menu.

* jika Keluar, User akan keluar program dan program akan berhenti.

# KESIMPULAN
Program yang telah dibuat adalah aplikasi sederhana untuk mengelola data nilai mahasiswa dengan menggunakan fungsi dalam Python. Program ini memiliki empat fitur utama
yang dapat dijalankan melalui menu interaktif:
