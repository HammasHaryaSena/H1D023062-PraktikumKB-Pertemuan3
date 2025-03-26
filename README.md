Program Python ini adalah sebuah sistem manajemen tugas sederhana
berbasis teks yang memungkinkan pengguna untuk menambahkan,
melihat, dan menghapus tugas. Program ini menggunakan struktur
kontrol seperti perulangan while True untuk menjalankan menu
interaktif secara terus-menerus hingga pengguna memilih keluar,
serta percabangan if-elif-else untuk menangani berbagai pilihan
menu yang diberikan pengguna. Selain itu, program ini menerapkan
struktur data berupa list untuk menyimpan daftar tugas dan
dictionary untuk merepresentasikan setiap tugas dengan atribut
seperti ID, nama, prioritas, dan waktu pembuatan.

Program ini memanfaatkan dua library bawaan Python, yaitu random
dan datetime. Library random digunakan untuk menghasilkan ID unik
secara acak bagi setiap tugas, sehingga setiap tugas dapat
diidentifikasi dengan jelas. Sementara itu, library datetime
digunakan untuk mencatat waktu pembuatan tugas dalam format "YYYY
MM-DD HH:MM:SS", yang membantu pengguna mengetahui kapan tugas
tersebut dibuat.

Fungsi add_task() digunakan untuk menambahkan tugas baru ke dalam
daftar tasks, di mana setiap tugas disimpan sebagai dictionary yang
berisi ID unik, nama tugas, prioritas, dan waktu pembuatan. Fungsi
view_tasks() memungkinkan pengguna untuk melihat daftar tugas yang
telah ditambahkan dengan menampilkan semua informasi yang terkait
dengan setiap tugas, atau menampilkan pesan jika tidak ada tugas
yang tersedia. Fungsi remove_task() bertugas untuk menghapus tugas
berdasarkan ID yang diberikan oleh pengguna, dengan cara membuat
ulang list tasks tanpa memasukkan tugas yang memiliki ID yang cocok
dengan input pengguna.

Di dalam loop utama program, pengguna diberikan pilihan menu untuk
menambah tugas, melihat daftar tugas, menghapus tugas berdasarkan
ID, atau keluar dari program. Jika pengguna memilih opsi yang tidak
valid, program akan menampilkan pesan kesalahan dan meminta input
ulang. Program ini dirancang agar mudah digunakan dan dapat
dikembangkan lebih lanjut dengan fitur tambahan seperti penyimpanan
ke file atau penggunaan database untuk menyimpan data secara
permanen.
