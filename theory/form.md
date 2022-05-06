# Form
Di halaman ini kita akan belajar memahami apa itu validasi formulir dari sisi klien, mengapa itu penting dan bagaimana menerapkan berbagai teknik untuk mengimplementasikannya.

Client-side validation adalah pengecekan data di sisi klien sebelum dikirimkan ke server, ini berguna untuk memberikan interaksi lebih baik, meminimalisir kesalahan data disisi klien, namun disarankan server tetap mengecek data yang dikirimkan oleh klien, referensi bacaan [keamanan website](https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Website_security).

Tiga alasan utama, untuk kita menggunakan form dengan baik dan benar:

- Mendapatkan data yang benar, dalam format yang tepat.
- Melindungi data pengguna, misalnya memaksa pengguna untuk memasukkan kata sandi yang aman.
- Melindungi diri sendiri, ada banyak cara pengguna jahat dapat menyalahgunakan formulir yang tidak dilindungi untuk merusak aplikasi.

<aside>
⚠️ Peringatan: Jangan pernah mempercayai data yang dikirimkan ke server Anda dari klien. Bahkan jika formulir Anda divalidasi dengan benar dan mencegah input yang salah di sisi klien, pengguna jahat masih dapat mengubah permintaan jaringan.

</aside>

## Berbagai jenis validasi disisi klien

Ada dua jenis validasi sisi klien yang berbeda yang akan Anda temui di web:

- Menggunakan HTML 5, umumnya tidak memerlukan banyak JavaScript. Pengunaanya sederhana da
- Menggunakan JavaScript, validasi ini sepenuhnya dapat disesuaikan, tetapi anda harus membuatnya semunya atau menggunakan library

## Menggunakan Validasi Formulir

Salah satu fitur paling signifikan dari kontrol formulir HTML5 adalah kemampuan untuk memvalidasi sebagian besar data pengguna tanpa bergantung pada JavaScript. Berikut beberapa validasnya:

- `required` : menentukan apakah bidang formulir perlu diisi sebelum formulir dapat dikirimkan.
- `minlength` dan `maxlength` : menentukan minimum dan maksimal panjang data tekstual (string).
- `min` dan `max` : menentukan minimum dan maksimal panjang tipe angka.
- `type` : menentukan apakah data perlu berupa nomor, alamat email, atau jeris tertentu lainnya.
- `pattern` : menentukan ekspresi reguler yang mendefinisikan pola yang harus diikuti oleh data yang dimasukkan.

Jika data yang dimasukkan dalam bidang formulir mengikuti semua aturan yang ditentukan oleh atribut di atas, itu dianggap valid. Jika tidak maka dianggap tidak sah.