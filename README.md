# Laporan Praktikum 5 - Pemrograman Web (JavaScript Dasar)

## Data Mahasiswa
- **Nama**: Abdi Putra Perdana
- **NIM**: 312410426
- **Kelas**: TI 24 A3
- **Mata Kuliah**: Pemrograman Web

---

## Tujuan Praktikum
1. Memahami konsep dasar JavaScript
2. Mengenal cara penggunaan JavaScript pada HTML
3. Mampu membuat script sederhana menggunakan JavaScript
4. Memahami penggunaan form dan validasi dengan JavaScript
5. Mengenal HTML DOM (Document Object Model)

---

## Langkah Praktikum

### 1. Pengenalan JavaScript
**File: lab5_javascript.html**

Membuat file HTML sederhana dengan menggunakan `document.write()` dan `console.log()`.

**Kode Program:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```

**Output:**

![Screenshot lab5_javascript](screenshot/01_pengenalan_javascript.png)

**Penjelasan:**
- `document.write()` digunakan untuk menampilkan output langsung ke halaman web
- `console.log()` digunakan untuk menampilkan output ke console browser (dapat dilihat dengan menekan F12)

---

### 2. JavaScript Dasar - Pemakaian Alert
**File: alert_box.html**

Membuat alert box sebagai property dari objek window.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>alert box</title>
</head>
<body>
    <script language="javascript">
        <!--
        window.alert("ini merupakan pesan untuk anda");
        //-->
    </script>
</body>
</html>
```

**Output:**

![Screenshot alert_box](screenshot/02_alert_box.png)

**Penjelasan:**
- `window.alert()` menampilkan kotak dialog dengan pesan tertentu
- Alert box akan muncul otomatis saat halaman dimuat

---

### 3. Pemakaian Method dalam Objek
**File: skrip_javascript.html**

Menggunakan method `document.write()` untuk menampilkan teks.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>skrip javascript</title>
</head>
<body>
    percobaan memakai javascript:<br>
    <script language="javascript">
        document.write("selamat mencoba javascript<br>");
        document.write("semoga sukses!");
        //-->
    </script>
</body>
</html>
```

**Output:**

![Screenshot skrip_javascript](screenshot/03_method_objek.png)

**Penjelasan:**
- Method `document.write()` dapat dipanggil berkali-kali
- Tag HTML seperti `<br>` dapat digunakan di dalam string untuk formatting

---

### 4. Pemakaian Prompt
**File: pemasukan_data.html**

Menggunakan prompt untuk input data dari user.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language="javascript">
        <!--
        var nama = prompt("siapa nama anda?", "masukkan nama anda");
        document.write("hai, " + nama);
        //-->
    </script>
</body>
</html>
```

**Output:**

![Screenshot pemasukan_data](screenshot/04_prompt.png)

**Penjelasan:**
- `prompt()` menampilkan dialog box untuk input data
- Data yang diinput disimpan dalam variabel dan dapat digunakan dalam program

---

### 5. Pembuatan Fungsi dan Cara Pemanggilannya
**File: contoh_program_javascript.html**

Membuat fungsi JavaScript dan memanggilnya melalui event `onload`.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function pesan() {
            alert("memanggil javascript lewat body onload");
        }
    </script>
</head>
<body onload="pesan()">
</body>
</html>
```

**Output:**

![Screenshot fungsi](screenshot/05_fungsi.png)

**Penjelasan:**
- Fungsi `pesan()` didefinisikan di dalam tag `<script>`
- Fungsi dipanggil otomatis saat body selesai dimuat menggunakan event `onload`

---

### 6. Operasi Dasar Aritmatika
**File: aritmatika.html**

Membuat program untuk operasi aritmatika dasar.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test(val1, val2) {
            document.write("<br>" + "perkalian : val1*val2 " + "<br>");
            document.write(val1 * val2);
            document.write("<br>" + "pembagian : val1/val2 " + "<br>");
            document.write(val1 / val2);
            document.write("<br>" + "penjumlahan : val1+val2 " + "<br>");
            document.write(val1 + val2);
            document.write("<br>" + "pengurangan : val1-val2 " + "<br>");
            document.write(val1 - val2);
            document.write("<br>" + "modulus : val1%val2 " + "<br>");
            document.write(val1 % val2);
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick="test(9,4)">
</body>
</html>
```

**Output:**

![Screenshot aritmatika](screenshot/06_aritmatika.png)

**Penjelasan:**
- Fungsi `test()` menerima dua parameter (val1 dan val2)
- Menampilkan hasil dari 5 operasi: perkalian, pembagian, penjumlahan, pengurangan, dan modulus

---

### 7. Seleksi Kondisi (if-else)
**File: if-else.html**

Membuat program seleksi kondisi menggunakan if-else.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language="javascript">
        <!--
        var nilai = prompt("nilai (0-100): ", 0);
        var hasil = "";
        if (nilai >= 60)
            hasil = "lulus";
        else
            hasil = "tidak lulus";
        document.write("hasil: " + hasil);
        //-->
    </script>
</body>
</html>
```

**Output:**

![Screenshot if-else](screenshot/07_if_else.png)

**Penjelasan:**
- Program meminta input nilai dari user
- Jika nilai >= 60, maka hasilnya "lulus"
- Jika nilai < 60, maka hasilnya "tidak lulus"

---

### 8. Penggunaan Operator Switch
**File: switch.html**

Membuat program dengan operator switch untuk seleksi kondisi.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test() {
            val1 = window.prompt("input nilai (1-5):");
            switch (val1) {
                case "1":
                    document.write("bilangan satu");
                    break;
                case "2":
                    document.write("bilangan dua");
                    break;
                case "3":
                    document.write("bilangan tiga");
                    break;
                case "4":
                    document.write("bilangan empat");
                    break;
                case "5":
                    document.write("bilangan lima");
                    break;
                default:
                    document.write("bilangan lainnya");
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick="test()">
</body>
</html>
```

**Output:**

![Screenshot switch](screenshot/08_switch.png)

**Penjelasan:**
- Operator switch digunakan untuk memilih salah satu dari beberapa blok kode
- Statement `break` digunakan untuk keluar dari switch
- `default` dijalankan jika tidak ada case yang cocok

---

### 9. Pembuatan Form Input
**File: form_input.html**

Membuat form untuk mengecek bilangan genap atau ganjil.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <script language="javascript">
        function test() {
            var val1 = document.kirim.T1.value;
            if (val1 % 2 == 0)
                document.kirim.T2.value = "bilangan genap";
            else
                document.kirim.T2.value = "bilangan ganjil";
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20"> MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick="test()"></p>
    </form>
</body>
</html>
```

**Output:**

![Screenshot form_input](screenshot/09_form_input.png)

**Penjelasan:**
- Form memiliki 2 input text dan 1 button
- Menggunakan operator modulus (%) untuk mengecek bilangan genap/ganjil
- Hasil ditampilkan pada input text kedua

---

### 10. Form Button - Mengubah Warna
**File: form_button.html**

Membuat form dengan button untuk mengubah warna background dan text.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language="javascript">
        function ubahWarnaLB(warna) {
            document.bgColor = warna;
        }
        function ubahWarnaLD(warna) {
            document.fgColor = warna;
        }
    </script>
    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language="javascript">
        document.write("dimodifikasi terakhir pada " + document.lastModified);
    </script>
</body>
</html>
```

**Output:**

![Screenshot form_button](screenshot/10_form_button.png)

**Penjelasan:**
- Menggunakan property `document.bgColor` untuk mengubah warna background
- Menggunakan property `document.fgColor` untuk mengubah warna text
- Property `document.lastModified` menampilkan waktu modifikasi terakhir dokumen

---

### 11. HTML DOM - Checkbox dengan Perhitungan
**File: daftar_menu.html**

Membuat form dengan checkbox yang dapat menghitung total otomatis.

**Kode Program:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
            total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }

            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"> Telur Dadar Rp. 2.500</label><br />
    <strong>Total Bayar: Rp. <input id="total" type="text"></strong>
</body>
</html>
```

**Output:**

![Screenshot daftar_menu](screenshot/11_daftar_menu.png)

**Penjelasan:**
- Menggunakan `getElementById()` untuk mengakses elemen HTML
- Fungsi `hitung()` dipanggil setiap kali checkbox di-click
- Total harga dihitung otomatis saat checkbox dicentang atau dilepas

---

## Pertanyaan dan Tugas

### Pertanyaan:
**Buat script untuk melakukan validasi pada isian form**

**Jawaban:**

**File: form_validasi.html**

Program validasi form dengan beberapa kriteria:
- Nama harus diisi minimal 3 karakter
- Email harus valid 
- Alamat harus diisi minimal 10 karakter
- Password harus diisi minimal 6 karakter

**Output:**

![Screenshot form_validasi](screenshot/12_form_validasi.png)

**Penjelasan:**
- Validasi dilakukan saat form di-submit
- Setiap field memiliki pesan error yang spesifik
- Menggunakan regex untuk validasi format email
- Form hanya akan diproses jika semua validasi berhasil

```

---

## Kesimpulan

Dari praktikum ini dapat disimpulkan bahwa:

1. **JavaScript** adalah bahasa pemrograman yang berjalan di sisi client (browser)
2. JavaScript dapat digunakan untuk:
   - Menampilkan output (`document.write()`, `console.log()`, `alert()`)
   - Menerima input dari user (`prompt()`)
   - Membuat fungsi dan menjalankannya dengan event
   - Melakukan operasi aritmatika dan logika
   - Membuat seleksi kondisi (if-else, switch)
   - Memanipulasi form HTML
   - Mengubah property dokumen secara dinamis
3. **HTML DOM** memungkinkan JavaScript untuk mengakses dan memanipulasi elemen HTML
4. **Validasi form** penting untuk memastikan data yang diinput user sesuai dengan ketentuan
5. JavaScript membuat website menjadi lebih interaktif dan dinamis

---

**© 2025 - Laporan Praktikum Pemrograman Web**
