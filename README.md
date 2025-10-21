# Praktikum 5: Javascript

**Nama:** Abdi Putra Perdana  
**NIM:** 312410426  
**Kelas:** TI 24 A3 

---

## Langkah-langkah Praktikum

### 1. File lab5_javascript.html - Contoh Dasar

File dasar untuk mengenal JavaScript dengan `document.write()` dan `console.log()`.

**Kode:**
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

![Screenshot 1](screenshot/01_javascript_dasar.png)

**Penjelasan:**
- `document.write()` menampilkan output ke halaman HTML
- `console.log()` menampilkan output ke console browser (buka dengan F12)

---

### 2. File lab5_alert.html - Pemakaian Alert

Menggunakan `window.alert()` untuk menampilkan pesan.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Alert Box</title>
</head>
<body>
    <h1>Contoh Alert Box</h1>
    <script>
        window.alert("Ini adalah pesan untuk anda");
    </script>
</body>
</html>
```

**Output:**

![Screenshot 2](screenshot/02_alert.png)

**Penjelasan:**
- `window.alert()` menampilkan kotak dialog peringatan
- Dialog akan muncul otomatis saat halaman dimuat

---

### 3. File lab5_method.html - Pemakaian Method dalam Objek

Menggunakan method `document.write()` untuk menampilkan teks.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Skrip JavaScript</title>
</head>
<body>
    Percobaan memakai JavaScript:<br>
    <script>
        document.write("Selamat mencoba JavaScript<br>");
        document.write("Semoga sukses!");
    </script>
</body>
</html>
```

**Output:**

![Screenshot 3](screenshot/03_method.png)

**Penjelasan:**
- Method adalah fungsi yang terkait dengan objek
- `document.write()` adalah method dari objek document

---

### 4. File lab5_prompt.html - Pemakaian Prompt

Menggunakan `prompt()` untuk menerima input dari user.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Pemasukan Data</title>
</head>
<body>
    <h1>Contoh Prompt</h1>
    <script>
        var nama = prompt("Siapa nama Anda?", "Masukkan nama Anda");
        document.write("<h1>Halo " + nama + "</h1>");
    </script>
</body>
</html>
```

**Output:**

![Screenshot 4a](screenshot/04a_prompt_dialog.png)
![Screenshot 4b](screenshot/04b_prompt_hasil.png)

**Penjelasan:**
- `prompt()` menampilkan dialog box untuk input
- Parameter pertama adalah pesan, parameter kedua adalah nilai default
- Nilai yang diinput disimpan dalam variabel

---

### 5. File lab5_fungsi.html - Pembuatan Fungsi

Membuat dan memanggil fungsi JavaScript.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Contoh Program JavaScript</title>
    <script>
        function pesan() {
            alert("Memanggil JavaScript lewat body onload");
        }
    </script>
</head>
<body onload="pesan()">
    <h1>Contoh Fungsi JavaScript</h1>
</body>
</html>
```

**Output:**

![Screenshot 5](screenshot/05_fungsi.png)

**Penjelasan:**
- Fungsi adalah blok kode yang dapat dipanggil berulang kali
- `onload` adalah event yang terjadi saat halaman selesai dimuat
- Fungsi `pesan()` dipanggil otomatis saat body selesai dimuat

---

### 6. File lab5_aritmatika.html - Operasi Dasar Aritmatika

Melakukan operasi matematika dasar.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Operasi Aritmatika</title>
    <script>
        function test(val1, val2) {
            document.write("<br>Perkalian: " + val1 + " * " + val2 + " = " + (val1 * val2));
            document.write("<br>Pembagian: " + val1 + " / " + val2 + " = " + (val1 / val2));
            document.write("<br>Penjumlahan: " + val1 + " + " + val2 + " = " + (val1 + val2));
            document.write("<br>Pengurangan: " + val1 + " - " + val2 + " = " + (val1 - val2));
            document.write("<br>Modulus: " + val1 + " % " + val2 + " = " + (val1 % val2));
        }
    </script>
</head>
<body>
    <h1>Operasi Dasar Aritmatika</h1>
    <input type="button" value="Arithmetic" onclick="test(9,4)">
</body>
</html>
```

**Output:**

![Screenshot 6](screenshot/06_aritmatika.png)

**Penjelasan:**
- Fungsi `test()` menerima 2 parameter
- Melakukan 5 operasi: perkalian (*), pembagian (/), penjumlahan (+), pengurangan (-), modulus (%)
- Hasil ditampilkan dengan `document.write()`

---

### 7. File lab5_ifelse.html - Seleksi Kondisi (if...else)

Menggunakan percabangan untuk membuat keputusan.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Seleksi Kondisi</title>
    <script>
        var nilai = prompt("Nilai (0-100): ", 0);
        var hasil = "";
        
        if (nilai >= 60)
            hasil = "Lulus";
        else
            hasil = "Tidak Lulus";
        
        document.write("Hasil: " + hasil);
    </script>
</head>
<body>
    <h1>Seleksi Kondisi</h1>
</body>
</html>
```

**Output:**

![Screenshot 7a](screenshot/07a_ifelse_input.png)
![Screenshot 7b](screenshot/07b_ifelse_hasil.png)

**Penjelasan:**
- `if...else` digunakan untuk membuat keputusan berdasarkan kondisi
- Jika nilai >= 60 maka "Lulus", selain itu "Tidak Lulus"

---

### 8. File lab5_switch.html - Penggunaan Switch

Menggunakan switch case untuk seleksi kondisi dengan banyak pilihan.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Switch Case</title>
    <script>
        var nilai = prompt("Nilai (1-5): ", 0);
        var hasil = "";
        
        switch(parseInt(nilai)) {
            case 1:
                hasil = "Bilangan satu";
                break;
            case 2:
                hasil = "Bilangan dua";
                break;
            case 3:
                hasil = "Bilangan tiga";
                break;
            case 4:
                hasil = "Bilangan empat";
                break;
            case 5:
                hasil = "Bilangan lima";
                break;
            default:
                hasil = "Bilangan lainnya";
        }
        
        document.write("Hasil: " + hasil);
    </script>
</head>
<body>
    <h1>Switch Case</h1>
</body>
</html>
```

**Output:**

![Screenshot 8a](screenshot/08a_switch_input.png)
![Screenshot 8b](screenshot/08b_switch_hasil.png)

**Penjelasan:**
- `switch` digunakan untuk mengevaluasi satu ekspresi dengan banyak kondisi
- `parseInt()` mengkonversi string menjadi integer
- `break` menghentikan eksekusi dan keluar dari switch
- `default` dijalankan jika tidak ada case yang cocok

---

### 9. File lab5_form.html - Pembuatan Form Input

Form sederhana dengan input dan button.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Form Input</title>
    <script>
        function tampil() {
            var nama = document.getElementById("nama").value;
            var hasil = "Halo " + nama + ", Selamat Datang";
            document.getElementById("hasil").innerHTML = hasil;
        }
    </script>
</head>
<body>
    <h1>Form Input</h1>
    <label>Nama:</label>
    <input type="text" id="nama" name="nama">
    <input type="button" value="Tampilkan" onclick="tampil()">
    <p id="hasil"></p>
</body>
</html>
```

**Output:**

![Screenshot 9](screenshot/09_form_input.png)

**Penjelasan:**
- `document.getElementById()` mengambil elemen berdasarkan ID
- `.value` mengambil nilai dari input
- `.innerHTML` mengubah konten HTML dari elemen

---

### 10. File lab5_button.html - Form Button

Manipulasi DOM dengan button.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Form Button</title>
    <script>
        function ubahWarna(warna) {
            document.getElementById("kotak").style.backgroundColor = warna;
        }
        
        function ubahUkuran(ukuran) {
            document.getElementById("kotak").style.width = ukuran + "px";
            document.getElementById("kotak").style.height = ukuran + "px";
        }
    </script>
</head>
<body>
    <h1>Form Button</h1>
    <input type="button" value="Merah" onclick="ubahWarna('red')">
    <input type="button" value="Hijau" onclick="ubahWarna('green')">
    <input type="button" value="Biru" onclick="ubahWarna('blue')">
    <br><br>
    <input type="button" value="Perbesar" onclick="ubahUkuran(200)">
    <input type="button" value="Perkecil" onclick="ubahUkuran(100)">
    <br><br>
    <div id="kotak" style="width:100px; height:100px; background-color:yellow; border:1px solid black;"></div>
</body>
</html>
```

**Output:**

![Screenshot 10](screenshot/10_button.png)

**Penjelasan:**
- Manipulasi CSS melalui JavaScript menggunakan `.style`
- Event `onclick` memanggil fungsi saat button diklik
- Fungsi dapat menerima parameter untuk mengubah properti elemen

---

### 11. File lab5_checkbox.html - HTML DOM dengan Checkbox

Checkbox dengan perhitungan otomatis.

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Checkbox dengan Perhitungan</title>
    <script>
        function hitung() {
            var total = 0;
            
            if(document.getElementById("cb1").checked)
                total += parseInt(document.getElementById("cb1").value);
            if(document.getElementById("cb2").checked)
                total += parseInt(document.getElementById("cb2").value);
            if(document.getElementById("cb3").checked)
                total += parseInt(document.getElementById("cb3").value);
            if(document.getElementById("cb4").checked)
                total += parseInt(document.getElementById("cb4").value);
            
            document.getElementById("total").value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" id="cb1" value="5000" onclick="hitung()"> Ayam Goreng Rp. 5.000</label><br>
    <label><input type="checkbox" id="cb2" value="3000" onclick="hitung()"> Tempe Goreng Rp. 3.000</label><br>
    <label><input type="checkbox" id="cb3" value="2500" onclick="hitung()"> Tahu Goreng Rp. 2.500</label><br>
    <label><input type="checkbox" id="cb4" value="3000" onclick="hitung()"> Es Teh Rp. 3.000</label><br>
    <br>
    <strong>Total Bayar: Rp. <input type="text" id="total" value="0" readonly></strong>
</body>
</html>
```

**Output:**

![Screenshot 11](screenshot/11_checkbox.png)

**Penjelasan:**
- `.checked` memeriksa apakah checkbox dicentang
- Perhitungan dilakukan setiap kali checkbox diklik
- `readonly` membuat input tidak bisa diedit manual

---

### 12. File lab5_validasi.html - TUGAS (Validasi Form)

Form pendaftaran dengan validasi lengkap.

**Fitur Validasi:**
1. **Nama Lengkap** - minimal 3 karakter
2. **NIM** - harus berupa angka
3. **Email** - format email valid (mengandung @)
4. **Nomor Telepon** - minimal 10 digit, harus angka
5. **Jenis Kelamin** - harus dipilih
6. **Alamat** - minimal 10 karakter

**Kode:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Form Validasi JavaScript</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .form-container {
            max-width: 500px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, textarea, select {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }
        .error {
            color: red;
            font-size: 12px;
            display: none;
        }
        .btn {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        .btn:hover {
            background-color: #45a049;
        }
        .success {
            color: green;
            font-weight: bold;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h2>Form Pendaftaran Mahasiswa</h2>
        <form name="formMahasiswa" onsubmit="return validasiForm()">
            <div class="form-group">
                <label>Nama Lengkap:</label>
                <input type="text" id="nama" name="nama">
                <span class="error" id="errorNama">Nama harus diisi!</span>
            </div>

            <div class="form-group">
                <label>NIM:</label>
                <input type="text" id="nim" name="nim">
                <span class="error" id="errorNim">NIM harus diisi dan berupa angka!</span>
            </div>

            <div class="form-group">
                <label>Email:</label>
                <input type="text" id="email" name="email">
                <span class="error" id="errorEmail">Email tidak valid!</span>
            </div>

            <div class="form-group">
                <label>Nomor Telepon:</label>
                <input type="text" id="telepon" name="telepon">
                <span class="error" id="errorTelepon">Nomor telepon harus diisi dan berupa angka!</span>
            </div>

            <div class="form-group">
                <label>Jenis Kelamin:</label>
                <select id="jenisKelamin" name="jenisKelamin">
                    <option value="">-- Pilih --</option>
                    <option value="L">Laki-laki</option>
                    <option value="P">Perempuan</option>
                </select>
                <span class="error" id="errorJenisKelamin">Jenis kelamin harus dipilih!</span>
            </div>

            <div class="form-group">
                <label>Alamat:</label>
                <textarea id="alamat" name="alamat" rows="4"></textarea>
                <span class="error" id="errorAlamat">Alamat harus diisi!</span>
            </div>

            <button type="submit" class="btn">Daftar</button>
            <div id="pesan" class="success"></div>
        </form>
    </div>

    <script>
        function validasiForm() {
            // Reset semua error
            var errors = document.getElementsByClassName("error");
            for(var i = 0; i < errors.length; i++) {
                errors[i].style.display = "none";
            }

            var valid = true;

            // Validasi Nama
            var nama = document.getElementById("nama").value;
            if(nama == "" || nama.length < 3) {
                document.getElementById("errorNama").style.display = "block";
                valid = false;
            }

            // Validasi NIM
            var nim = document.getElementById("nim").value;
            if(nim == "" || isNaN(nim)) {
                document.getElementById("errorNim").style.display = "block";
                valid = false;
            }

            // Validasi Email
            var email = document.getElementById("email").value;
            var emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if(email == "" || !emailPattern.test(email)) {
                document.getElementById("errorEmail").style.display = "block";
                valid = false;
            }

            // Validasi Telepon
            var telepon = document.getElementById("telepon").value;
            if(telepon == "" || isNaN(telepon) || telepon.length < 10) {
                document.getElementById("errorTelepon").style.display = "block";
                valid = false;
            }

            // Validasi Jenis Kelamin
            var jenisKelamin = document.getElementById("jenisKelamin").value;
            if(jenisKelamin == "") {
                document.getElementById("errorJenisKelamin").style.display = "block";
                valid = false;
            }

            // Validasi Alamat
            var alamat = document.getElementById("alamat").value;
            if(alamat == "" || alamat.length < 10) {
                document.getElementById("errorAlamat").style.display = "block";
                valid = false;
            }

            // Jika semua validasi berhasil
            if(valid) {
                document.getElementById("pesan").innerHTML = "Pendaftaran berhasil! Data Anda telah tersimpan.";
                setTimeout(function() {
                    document.forms["formMahasiswa"].reset();
                    document.getElementById("pesan").innerHTML = "";
                }, 2000);
            }

            return false;
        }
    </script>
</body>
</html>
```

**Output:**

![Screenshot 12a](screenshot/12a_validasi_kosong.png)
![Screenshot 12b](screenshot/12b_validasi_error.png)
![Screenshot 12c](screenshot/12c_validasi_sukses.png)

**Penjelasan:**
- Fungsi `validasiForm()` dipanggil saat form di-submit
- Setiap field divalidasi dengan kondisi tertentu
- `isNaN()` memeriksa apakah nilai bukan angka
- Regular expression `/^[^\s@]+@[^\s@]+\.[^\s@]+$/` untuk validasi email
- Error message ditampilkan dengan mengubah `display` style
- Form direset otomatis setelah 2 detik jika berhasil

---

## Kesimpulan

Dari praktikum ini telah dipelajari:

1. **Sintaks Dasar JavaScript**
   - Penulisan script di dalam tag `<script>`
   - Penempatan script di `<head>` atau `<body>`
   - Penggunaan file JavaScript eksternal

2. **Output JavaScript**
   - `document.write()` - output ke halaman HTML
   - `console.log()` - output ke console
   - `alert()` - output ke dialog box
   - `prompt()` - input dari user
   - `innerHTML` - manipulasi konten elemen

3. **Pemrograman Dasar**
   - Variabel dan tipe data
   - Operator aritmatika
   - Seleksi kondisi (if-else, switch)
   - Fungsi (function)

4. **DOM Manipulation**
   - `getElementById()` - mengambil elemen berdasarkan ID
   - `.value` - mengambil/mengisi nilai input
   - `.innerHTML` - mengubah konten HTML
   - `.style` - mengubah CSS
   - `.checked` - memeriksa status checkbox

5. **Event Handling**
   - `onclick` - event saat diklik
   - `onload` - event saat halaman dimuat
   - `onsubmit` - event saat form di-submit

6. **Form Validation**
   - Validasi input tidak boleh kosong
   - Validasi tipe data (angka, email)
   - Validasi panjang karakter
   - Menampilkan pesan error

JavaScript adalah bahasa pemrograman yang sangat powerful untuk membuat halaman web menjadi interaktif dan dinamis.

---

**© 2025 - Praktikum Pemrograman Web**
