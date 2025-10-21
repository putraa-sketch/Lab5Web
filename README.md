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

<img width="1858" height="464" alt="image" src="https://github.com/user-attachments/assets/ffd9cbd3-2c89-4468-9ecd-545ef77be6cb" />


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

<img width="1033" height="320" alt="image" src="https://github.com/user-attachments/assets/f321f1b1-2916-435a-80c3-247f74af02ed" />

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

<img width="859" height="268" alt="image" src="https://github.com/user-attachments/assets/1e2899d6-502d-4314-b925-a158bebd9681" />

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

<img width="846" height="364" alt="image" src="https://github.com/user-attachments/assets/80702957-f8c0-470b-9dd0-e215c37074cf" />
<img width="434" height="137" alt="image" src="https://github.com/user-attachments/assets/0ea4a9bc-a90f-4419-974a-1589a681b563" />



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

<img width="771" height="260" alt="image" src="https://github.com/user-attachments/assets/9ae7db09-ac6f-44f9-8afe-e9e43af8fd1a" />


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

<img width="328" height="146" alt="image" src="https://github.com/user-attachments/assets/03c544f7-d6c1-4c76-8d74-4578801af226" />
<img width="324" height="410" alt="image" src="https://github.com/user-attachments/assets/64115a77-537d-4be9-b29b-c209169958c8" />


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

<img width="718" height="266" alt="image" src="https://github.com/user-attachments/assets/0d2d3fa9-d317-4529-8075-2aef04ff5ca6" />
<img width="1640" height="192" alt="image" src="https://github.com/user-attachments/assets/f8fb427b-39b3-4e9a-ae41-ce53b0234fed" />

<img width="716" height="270" alt="image" src="https://github.com/user-attachments/assets/4bfc93a3-8541-4dd7-b766-7ce6fb84636c" />
<img width="1643" height="186" alt="image" src="https://github.com/user-attachments/assets/ce913917-dfc0-400e-9d76-15d2a466db4d" />




**Penjelasan:**
- Program meminta input nilai dari user
- Jika nilai < 60, maka hasilnya "tidak lulus"
- Jika nilai >= 60, maka hasilnya "lulus"

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

<img width="461" height="122" alt="image" src="https://github.com/user-attachments/assets/4a9c73b3-ed42-49e8-81ce-a6c6a2765525" />
<img width="703" height="262" alt="image" src="https://github.com/user-attachments/assets/7b05c2e3-a01a-4b4b-a766-6d06bc38e701" />
<img width="410" height="147" alt="image" src="https://github.com/user-attachments/assets/1b95e9ab-361d-4739-aaba-d3c80f7018fc" />


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

<img width="1021" height="265" alt="image" src="https://github.com/user-attachments/assets/0876dc9a-1ccf-42f4-b6f6-fc3a974bbafc" />
<img width="805" height="180" alt="image" src="https://github.com/user-attachments/assets/f2565baf-4570-45dc-83a9-521b9a1b4a11" />


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

<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/4e2f9769-ace0-4fe9-b0a6-74fc6f11341a" />


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

<img width="961" height="389" alt="image" src="https://github.com/user-attachments/assets/a5aeae93-121f-45d9-bb11-21d20bba8d58" />


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

**Kode Program:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Form Validasi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 500px;
            margin: 50px auto;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .form-container {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h2 {
            color: #333;
            text-align: center;
            margin-bottom: 30px;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            color: #555;
            font-weight: bold;
        }
        input[type="text"],
        input[type="email"],
        input[type="password"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
        }
        input[type="text"]:focus,
        input[type="email"]:focus,
        input[type="password"]:focus {
            outline: none;
            border-color: #4CAF50;
        }
        .error {
            color: red;
            font-size: 12px;
            margin-top: 5px;
            display: none;
        }
        .submit-btn {
            width: 100%;
            padding: 12px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
            margin-top: 10px;
        }
        .submit-btn:hover {
            background-color: #45a049;
        }
        .success {
            color: green;
            text-align: center;
            margin-top: 15px;
            display: none;
        }
    </style>
    <script>
        function validateForm() {
            // Reset error messages
            var errors = document.getElementsByClassName('error');
            for (var i = 0; i < errors.length; i++) {
                errors[i].style.display = 'none';
            }
            
            var isValid = true;
            
            // Validasi Nama
            var nama = document.getElementById('nama').value;
            if (nama == "" || nama.length < 3) {
                document.getElementById('namaError').style.display = 'block';
                document.getElementById('namaError').innerHTML = 'Nama harus diisi minimal 3 karakter!';
                isValid = false;
            }
            
            // Validasi Email
            var email = document.getElementById('email').value;
            var emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (email == "") {
                document.getElementById('emailError').style.display = 'block';
                document.getElementById('emailError').innerHTML = 'Email harus diisi!';
                isValid = false;
            } else if (!emailPattern.test(email)) {
                document.getElementById('emailError').style.display = 'block';
                document.getElementById('emailError').innerHTML = 'Format email tidak valid!';
                isValid = false;
            }
            
            // Validasi Alamat
            var alamat = document.getElementById('alamat').value;
            if (alamat == "" || alamat.length < 10) {
                document.getElementById('alamatError').style.display = 'block';
                document.getElementById('alamatError').innerHTML = 'Alamat harus diisi minimal 10 karakter!';
                isValid = false;
            }
            
            // Validasi Password
            var password = document.getElementById('password').value;
            if (password == "" || password.length < 6) {
                document.getElementById('passwordError').style.display = 'block';
                document.getElementById('passwordError').innerHTML = 'Password harus diisi minimal 6 karakter!';
                isValid = false;
            }
            
            // Jika semua validasi berhasil
            if (isValid) {
                document.getElementById('successMsg').style.display = 'block';
                document.getElementById('successMsg').innerHTML = 'Form berhasil divalidasi! Data siap dikirim.';
                return true;
            }
            
            return false;
        }
    </script>
</head>
<body>
    <div class="form-container">
        <h2>Form Pendaftaran</h2>
        <form onsubmit="return validateForm()">
            <div class="form-group">
                <label for="nama">Nama Lengkap:</label>
                <input type="text" id="nama" name="nama" placeholder="Masukkan nama lengkap">
                <div id="namaError" class="error"></div>
            </div>
            
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Masukkan email">
                <div id="emailError" class="error"></div>
            </div>
            
            <div class="form-group">
                <label for="alamat">Alamat:</label>
                <input type="text" id="alamat" name="alamat" placeholder="Masukkan alamat lengkap">
                <div id="alamatError" class="error"></div>
            </div>
            
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Masukkan password">
                <div id="passwordError" class="error"></div>
            </div>
            
            <button type="submit" class="submit-btn">Submit</button>
            <div id="successMsg" class="success"></div>
        </form>
    </div>
</body>
</html>

```

**Output:**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/9a528abb-855e-47e1-883a-312219dbb756" />

**Penjelasan:**
- Validasi dilakukan saat form di-submit
- Setiap field memiliki pesan error yang spesifik
- Menggunakan regex untuk validasi format email
- Form hanya akan diproses jika semua validasi berhasil

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
