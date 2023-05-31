## Creating and Manage User Account

1. Untuk membuat user akun didalam linux bisa menggunaka perintah `useradd username`. Secara default, perintah `useradd` hanya membuat akun pengguna baru tanpa mengatur sandi. Anda bisa mengatur sandi untuk akun pengguna dengan perintah `passwd username`. Gantilah `username` dengan nama akun pengguna yang telah Anda buat.

2. Untuk cara kedua bisa menggunaka perintah `adduser username`. Ketika menjalankan perintah `adduser`, Anda akan diminta untuk memasukkan sandi dan informasi tambahan seperti nama lengkap, nomor telepon, dll. Isilah informasi yang diminta sesuai kebutuhan.

3. Untuk mengubah properti akun pengguna di Linux, Anda dapat menggunakan perintah `usermod [opsi] nama_pengguna`

4. Gunakan opsi yang sesuai dengan perubahan yang ingin Anda lakukan. Beberapa opsi umum yang dapat digunakan dengan perintah usermod adalah:

- -c "Nama Lengkap": Mengubah nama lengkap pengguna.
- -d /path/ke/direktori: Mengubah direktori home pengguna.
- -e YYYY-MM-DD: Menentukan tanggal kedaluwarsa akun pengguna.
- -g nama_grup: Mengubah grup primer pengguna.
- -G grup1,grup2: Mengubah daftar grup tambahan pengguna.
- -s /path/ke/shell: Mengubah shell default pengguna.
- -l nama_baru: Mengubah nama pengguna.
- -L: Mengunci akun pengguna.
- -U: Membuka kunci akun pengguna.

Anda dapat menggabungkan beberapa opsi dalam satu perintah. Misalnya, untuk mengubah nama lengkap dan direktori home pengguna, perintahnya bisa menjadi: `usermod -c "Nama Lengkap Baru" -d /path/ke/direktori_baru nama_pengguna`. Setelah menjalankan perintah usermod, properti akun pengguna akan diubah sesuai dengan opsi yang Anda berikan.

5. Untuk menghapus user gunakan perintah berikut : `userdel nama_pengguna`. Secara default, perintah userdel hanya menghapus akun pengguna tanpa menghapus direktori home dan file-file yang terkait. Jika Anda ingin menghapus direktori home dan file-file pengguna, tambahkan opsi `-r` pada perintah: `userdel -r nama_pengguna`

