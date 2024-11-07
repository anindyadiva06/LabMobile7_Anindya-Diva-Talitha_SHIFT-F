ANINDYA DIVA TALITHA | H1D022026

Proses login dimulai dari 'LoginPage' yang berisi input username dan password. Sebelumnya, username dan passsword harus sudah ada pda database agar dapat melakukan login.
Ketika pengguna memasukkan username dan password mereka lalu menekan tombol login maka fungsi 'login()' dipanggil. Fungsi ini memeriksa apakah username dan password tidak kosong. 
Jika keduanya diisi, data login tersebut dikirim melalui metode 'postMethod' dari 'AuthenticationService' ke file 'login.php' di server. Server memproses permintaan ini dan mengembalikan respons dari aksi tersebut. 
Jika login berhasil, token autentikasi dan nama pengguna disimpan menggunakan metode 'saveData' pada 'AuthenticationService' dan pengguna diarahkan ke halaman beranda. Jika login gagal, muncul pop-up yang menginformasikan bahwa username atau password salah.

Di halaman 'HomePage' nama pengguna ditampilkan berdasarkan data yang diambil dari 'AuthenticationService'. Pengguna juga dapat logout dari halaman ini. Saat pengguna melakukan logout, fungsi 'logout() pada 'AuthenticationService' dipanggil untuk membersihkan 
data autentikasi yang tersimpan, lalu pengguna akan kembali ke halaman login. Proses autentikasi ini memastikan bahwa hanya pengguna yang berhasil login yang dapat mengakses halaman beranda.

Tampilan Login
![image](https://github.com/user-attachments/assets/1134825b-a237-4b0b-ac59-96d167583aef)

Tampilan Login Gagal
![image](https://github.com/user-attachments/assets/39bd9f06-83ea-4a9b-8a44-73816b544e8b)

Tampilan Beranda
![image](https://github.com/user-attachments/assets/564f0f75-6e01-4f00-ad02-cbd63c6e352d)
