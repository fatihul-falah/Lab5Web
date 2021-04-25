# Praktikum 5 - Pemrograman Web
### Fatihul Falah Hidayatullah - 311910460
### TI.19.A2

## LANGKAH 1
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
![1](https://i.imgur.com/GUzSYUY.png)
```
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
## LANGKAH 2 javascript Dasar
### Pemakaian Alert sebagai property window.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>alert box</title>
</head>
<body>
    <script language = "javascript">
 <!--
  window.alert("ini merupakan pesan untuk anda");
    </script>
</body>
</html>
```
![2](https://i.imgur.com/kSzd5yr.png)

### Pemakaian method dalam objek
 ```
 <!DOCTYPE html>
<html lang="en">
<head>
    <title>skrip javascript</title>
</head>
<body>
    percobaan memakai javascript:<br>
    <script language = "javascript">
 <!--
 document.write("selamat mencoba javascript<br>");
 document.write("semoga sukses");
 //-->
    </script>
</body>
</html>
 ```
 ![3 output](https://i.imgur.com/afyp5W3.png)

 ### Pemakaian Prompt
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language = "javascript">
 <!--
 var nama = prompt("siapa nama anda?","masukan nama anda");
 document.write("hai, " + nama);
 //-->
    </script>
</body>
</html>
```
![4](https://i.imgur.com/NtVKqAZ.png)
![4-2](https://i.imgur.com/1QcdVTC.png)

### Pembuatan fungsi dan cara pemanggilannya
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language = "javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```
![5](https://i.imgur.com/nYFvom1.png)

## Langkah 3 Dasar Pemrograman Di Javascript 
### Operasi dasar aritmatika
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language = "javascript">
    function test (val1,val2){
        document.write("<br>"+"perkalian : val1*val2"+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2"+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
</body>
</html>
```
![6-1](https://i.imgur.com/6GIcne2.png)
![6-2](https://i.imgur.com/4kHGNeE.png)

### Seleksi kondisi (if..else)
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
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
![7-1](https://i.imgur.com/vVdDxln.png)
![7-2](https://i.imgur.com/MIMqdsp.png)
![7-3](https://i.imgur.com/vvAjkAz.png)
### Penggunaan operator switch untuk seleksi kondisi
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh contoh javascript</title>
    <script language = "javascript">
        function test()
        {
            val1=window.prompt("input nilai (1-5):")
            switch (val1)
            {
                case "1" :
                    document.write("bilangan satu")
                    break
                case "2" :
                    document.write("bilangan dua")
                    break
                case "3" :
                    document.write("bilangan tiga")
                    break
                case "4" :
                    document.write("bilangan empat")
                    break
                case "5" :
                    document.write("bilangan lima")
                    break
                default :
                document.write("bilangan lainnya")
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```
![8-1](https://i.imgur.com/4yxYmut.png)
![8-2](https://i.imgur.com/b446nYL.png)
![8-3](https://i.imgur.com/j5buigI.png)
![8-4](https://i.imgur.com/31ZlffT.png)
## Langkah 4 Pembuatan Form
### Form Input
```
<!DOCTYPE html>
<html>
<head>
    <script language = "javascript">
        function test()
        {
            var val1=document.kirim.T1.value
            if (val1%2==0)
                document.kirim.T2.value="bilangan genap"
            else
                document.kirim.T2.value="bilangan ganjil"
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <INPUT TYPE="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```
![9-1](https://i.imgur.com/jLEIUC2.png)
![9-2](https://i.imgur.com/jMH3fQ9.png)

### Form Button
```
<!DOCTYPE html>
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language ="javascript">
        <!--
        function ubahWarnaLB(warna) {
            document.bgColor = warna;
        }
        function ubahWarnaLD(warna) {
            document.fgColor = warna;
        }
        //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language ="javascript">
        <!--
            document.write("Dimodifikasi terakhir pada " + document.lastModified);
        //-->
    </script>
</body>
</html>
```
![10-1](https://i.imgur.com/0yKhXJ0.png)
![10-2](https://i.imgur.com/14fl4vq.png)
![10-3](https://i.imgur.com/dZyxcVq.png)
![10-4](https://i.imgur.com/tkg81B8.png)
![10-5](https://i.imgur.com/dSTsObE.png)

### HTML DOM
### Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!DOCTYPE html>
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele){
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;
            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else{
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
    <label><input type="checkbox" value='5000' id="menu1" onclick="hitung(this);"/> Ayam Goreng Rp. 5.000</label><br/>
    <label><input type="checkbox" value='500' id="menu2" onclick="hitung(this);"/> Tempe Goreng Rp. 500</label><br/>
    <label><input type="checkbox" value='2500' id="menu3" onclick="hitung(this);"/> Telur Dadar Rp. 2.500</label><br/>
    <strong>Total Bayar: Rp. <input id='total' type="text"/></strong>
</body>
</html>
```
![11-1](https://i.imgur.com/wnBQPEk.png)
![11-2](https://i.imgur.com/9rzHzSr.png)
![11-3](https://i.imgur.com/ZbNvRzA.png)

## TUGAS
### Buat script untuk melakukan validasi pada isian form.
![12-1](https://i.imgur.com/GMAFBQO.png)
```
<!DOCTYPE HTML>
<html>
<head>
   <title>Validasi Isian Form</title>
</head>
<body>
   <h1>Validasi Isian Form</h1>
   <form>
      <fieldset>
       <legend>Formulir Pendaftaran</legend>
       Nama Lengkap:<br>
         <input type="text" name="nama" required><br>
       Alamat Email:<br>
         <input type="email" name="email" required><br>
       Sandi:<br>
         <input type="password" name="sandi1" required><br>
       Sandi (ulangi):<br>
         <input type="password" name="sandi2" required><br>
     <br>
         <input type="submit" value="Kirim">
    </fieldset>   
   </form>
</body>
</html>
```
![12-2](https://i.imgur.com/8d5hY1H.png)
![12-3](https://i.imgur.com/61i8TQY.png)