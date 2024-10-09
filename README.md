# LATIHAN 1
## 1. Apa yang harus didefinisikan sebelum membuat objek?
- Class adalah cetak biru (blueprint) atau template yang digunakan untuk membuat objek.
- Atribut adalah variabel yang digunakan untuk menyimpan data atau informasi dalam kelas
- Constructor adalah metode khusus yang digunakan untuk menginisialisasi (memberi nilai awal) objek ketika objek tersebut dibuat.
- Metode adalah fungsi atau prosedur yang didefinisikan di dalam kelas dan memungkinkan objek untuk melakukan aksi atau operasi tertentu.

## 2. Buatlah gambar diagram class dan dua buah objek dari class Person bernama Antor dan Riko!
- Diagram Class

  ![Diagram Class](https://github.com/user-attachments/assets/0a677f6d-3132-4597-9770-09e83269b8d1)

- Diagram Objek
| Person | Nama | Jenis Kelamin | Umur |
|:------ |:---- |:------------- |:----:|
| Antor  | Antor| L             | 25   |
| Riko   | Riko | L             | 35   |
Objek Antor dan Riko adalah instance dari class Person, yang dimana atribut seperti nama, jenis kelamin, dan umur di isi biodata mereka

## 3. uatlah gambar diagram objek AkunBank dengan instance method simpanUang, ambilUang dan cekSaldo
- Diagram Class

  ![Diagram Class (2)](https://github.com/user-attachments/assets/a762312d-2455-432b-8d30-c88ca831040a)

- Diagram Objek
| Akun saya : AkunBank |
|:--------------------:|
|saldo : 100000        |
|simpanUang(500000)    |
|ambilUang(150000)     |
|cekSaldo()            |

# LATIHAN 2
## 1. Mendeklarasikan class Person, dengan atribut Nama, JenisKelamin, Umur

![Screenshot 2024-10-09 194722](https://github.com/user-attachments/assets/c7a71555-c265-4e71-bbb0-d737196d71c7)

Atribut nama, jenisKelamin, dan umur dideklarasikan sebagai bagian dari class Person. Setiap objek dari class ini akan memiliki ketiga atribut tersebut.
- String nama akan menyimpan nama seseorang.
- String jenisKelamin akan menyimpan jenis kelamin (misalnya: "Laki-laki" atau "Perempuan").
- int umur akan menyimpan umur dalam angka
  
## 2. Buatlah dua buah objek dari class Person bernama Anton dan Riko

![Screenshot 2024-10-09 194916](https://github.com/user-attachments/assets/4511a013-8712-4348-82a7-136116f96100)

Ketika kita membuat objek dari class Person, kita harus memberikan nilai untuk nama, jenisKelamin, dan umur. Nilai-nilai ini kemudian disimpan dalam atribut yang sesuai menggunakan keyword this.
- this.nama = nama; berarti kita menetapkan nilai yang diterima sebagai argumen nama ke atribut nama milik objek yang sedang dibuat.

![Screenshot 2024-10-09 195140](https://github.com/user-attachments/assets/a9820886-d560-4924-ada7-f47d194768b6)

- Ketika metode ini dipanggil, program akan mencetak nilai dari atribut nama, jenisKelamin, dan umur pada konsol.
- Di dalam metode main, kita membuat dua objek dari class Person, yaitu anton dan riko.
- Person anton = new Person("Anton", "Laki-laki", 25); membuat objek anton dengan nama "Anton", jenisKelamin "Laki-laki", dan umur 25.
- Person riko = new Person("Riko", "Laki-laki", 30); membuat objek riko dengan nama "Riko", jenisKelamin "Laki-laki", dan umur 30.
- Setelah objek dibuat, metode tampilkanInfo() dipanggil untuk setiap objek. Ini akan menampilkan informasi dari masing-masing objek di layar.

# Hasil Output

![Screenshot 2024-10-09 195431](https://github.com/user-attachments/assets/72ebcc1f-ac73-4390-a419-2e8d509a3933)
Output ini menunjukkan bahwa atribut nama, jenisKelamin, dan umur dari masing-masing objek telah dicetak ke layar.

# LATIHAN 3 
## 1. Mendeklarasikan class AkunBank dengan instance method simpanUang, ambilUang dan cekSaldo
## 2. Buat objek AkunBank dan tetapkan nilai saldo awal Rp. 100000, kemudian panggil 3 method tersebut dan tampilkan proses berikut:
![Screenshot 2024-10-09 201012](https://github.com/user-attachments/assets/87ca1eb4-1815-4cd6-8e4a-348592875b9f)

## Jawaban Soal 1 dan 2
![Screenshot 2024-10-09 195732](https://github.com/user-attachments/assets/7243ff33-9ee0-4db6-a3e2-a988a343ca43)
![Screenshot 2024-10-09 195756](https://github.com/user-attachments/assets/5b612b17-3cf9-4786-bee7-4ca6bbf5416f)
![Screenshot 2024-10-09 195804](https://github.com/user-attachments/assets/74334528-0380-4023-b2ce-61beac4e69ab)

1. Class AkunBank:
   - Atribut saldo digunakan untuk menyimpan saldo dari akun bank. Constructor 
   - AkunBank(int saldoAwal) digunakan untuk menginisialisasi saldo awal ketika 
2. Method simpanUang(int jumlah):
   - Metode ini menambah saldo dengan nilai jumlah yang diberikan.
   - Setelah saldo ditambahkan, metode ini memanggil cekSaldo() untuk menampilkan saldo terbaru.
3. Method ambilUang(int jumlah):
   - Metode ini mengurangi saldo jika saldo mencukupi, jika tidak, ditampilkan pesan bahwa saldo tidak mencukupi.
   - Setelah mengambil uang, saldo kembali dicek dengan memanggil cekSaldo().
4. Method cokSaldo():
   Mtode ini hanya menampilkan saldo saat ini.
5. Main Class:
   - Membuat objek AkunBank dengan saldo awal sebesar Rp. 100000.
   - Kemudian, memanggil metode simpanUang(500000) untuk menambah saldo dan ambilUang(150000) untuk mengambil uang, serta menampilkan saldo setelah setiap transaksi.

# Hasil Output

![Screenshot 2024-10-09 201053](https://github.com/user-attachments/assets/eb5e1027-083a-454f-a9d6-a64b0943b18c)

- Program menampilkan pesan "Selamat Datang di Bank ABC" dan saldo awal Rp. 100000.
- Setelah menyimpan uang sebesar Rp. 500000, saldo menjadi Rp. 600000.
- Setelah mengambil uang sebesar Rp. 150000, saldo berkurang menjadi Rp. 450000.
