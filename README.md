# PostTest1_ManajemenKoleksiLukisan
Nama : Marcela Persa Linthin 

NIM : 2409116072

# Deskripsi Singkat Program
Program ini adalah aplikasi sederhana untuk Manajemen Koleksi Lukisan yang menggunakan bahasa pemrograman Java. Program ini memungkinkan pengguna untuk mengelola data lukisan dengan fitur CRUD (Create, Read, Update, Delete). Data lukisan yang dikelola berupa ID Lukisan, Judul, Nama Pelukis, dan Tahun. Pengguna dapat menambahkan data lukisan baru, melihat daftar lukisan, memperbarui data lukisan yang sudah ada, menghapus data lukisan dari koleksi serta keluar dari program. Selama pengguna belum memilih menu keluar, program akan terus berjalan dan menampilkan kembali menu utama.

# Penjelasan Alur Program dan Output
<img width="343" height="66" alt="image" src="https://github.com/user-attachments/assets/0e854910-e644-4e21-a135-f35cb50a8a0b" />

Program menggunakan dua library bawaan dari Java, yaitu ArrayList dan Scanner. Library ArrayList berfungsi sebagai wadah penyimpanan data lukisan. ArrayList dipilih karena bersifat dinamis sehingga jumlah data bisa bertambah atau berkurang sesuai jumlah data yang dimasukkan atau dihapus. Sementara itu, library Scanner digunakan untuk membaca input dari pengguna.

<img width="900" height="424" alt="image" src="https://github.com/user-attachments/assets/04f8994c-3b88-42c3-bf29-fcb174fc642d" />

Pada bagian awal, program mengimpor library ArrayList dan Scanner kemudian membuat sebuah class Main. Di dalam class ini terdapat class statis bernama Lukisan yang merepresentasikan struktur data lukisan. Tiap objek Lukisan ini menyimpan id, judul, pelukis, dan tahun.

<img width="727" height="104" alt="image" src="https://github.com/user-attachments/assets/d5d8e980-4693-4c9b-bdb5-d7abb0d2be30" />

Di dalam method main, setiap data lukisan (objek dari class Lukisan) disimpan ke dalam ArrayList<Lukisan> koleksi. Scanner input = new Scanner(System.in); digunakan untuk menerima masukan berupa angka (untuk menu ID, tahun) maupun teks (judul, nama pelukis).

<img width="838" height="297" alt="image" src="https://github.com/user-attachments/assets/36432ace-9097-4b6e-8a77-e8c684d9d5aa" />
  
Program menggunakan perulangan while(true) agar menu selalu muncul berulang kali selama pengguna belum memilih keluar. Program akan menampilkan menu pilihan. Input menu pilihan disimpan dalam variabel pilih.

<img width="818" height="480" alt="image" src="https://github.com/user-attachments/assets/01bd98b0-17e7-43a7-ac3a-897171d2545f" />

Menggunakan percabangan (switch) untuk pemilihan menu.

Di case 1 ini, jika pengguna memilih menu Tambah Lukisan, program akan meminta data berupa ID, judul, pelukis, dan tahun. Data kemudian disimpan sebagai objek Lukisan baru di dalam ArrayList. Output yang ditampilkan adalah pesan konfirmasi, contohnya:

<img width="384" height="271" alt="image" src="https://github.com/user-attachments/assets/0be26a7f-c075-469d-916e-1588879b6c99" />

<img width="785" height="408" alt="image" src="https://github.com/user-attachments/assets/c3c935ec-62fd-495f-896e-0193ca535a0f" />

Jika pengguna memilih menu Lihat Daftar Lukisan, program akan memeriksa apakah ArrayList kosong atau tidak. Jika ada data, program menampilkan seluruh koleksi lukisan menggunakan perulangan. Misalnya setelah menambahkan satu data, output yang muncul adalah:

<img width="668" height="231" alt="image" src="https://github.com/user-attachments/assets/85df74a5-f550-4012-9fc4-a7c8336c4a3a" />

<img width="993" height="704" alt="image" src="https://github.com/user-attachments/assets/63a8201b-8de5-4cec-9e37-af4a0bab9b72" />

Ketika pengguna memilih menu Update Lukisan, program akan meminta ID lukisan yang ingin diubah dan kemudian mencari data di dalam ArrayList. Jika ditemukan, pengguna diminta menginputkan data baru untuk mengganti data lama. Contohnya: 

<img width="396" height="267" alt="image" src="https://github.com/user-attachments/assets/e419fbca-80ab-4236-8a44-a93037af4549" />

<img width="985" height="538" alt="image" src="https://github.com/user-attachments/assets/35d5f84f-b0a7-4cfa-991d-8d1fb4bef172" />

Sama seperti menu Update Lukisan, program akan meminta ID lukisan lalu menghapus data yang sesuai dari ArrayList jika ditemukan.

<img width="395" height="206" alt="image" src="https://github.com/user-attachments/assets/02eb1954-9d5c-4170-b9c5-93ad03fe6edc" />

Namun, jika ID yang dimasukkan tidak ada di dalam koleksi, baik pada saat update maupun hapus, maka program menampilkan pesan:
<img width="402" height="45" alt="image" src="https://github.com/user-attachments/assets/67345f96-9b49-4013-ad0b-011473aa4768" />

<img width="1072" height="275" alt="image" src="https://github.com/user-attachments/assets/ed26c5ab-c97e-4031-8933-e28153284352" />

Apabila pengguna memilih menu Keluar, program akan menghentikan perulangan while(true) dengan perintah System.exit(0) dan menampilkan pesan perpisahan:

<img width="556" height="53" alt="image" src="https://github.com/user-attachments/assets/ffc6df05-8cda-4b66-a9a8-cbffff0995b3" />


