# Lab9web
# Lab9Web
# Nama : Taufik eka albani
# NIM : 312210347
# Kelas : TI 22A3

# Lab9web
## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama lab9_php_modular pada docroot webserver(htdocs)
3. Ikuti langkah-langkah praktikum
## Jalankan XAMPP dan akses ```http://localhost/phpmyadmin/``` untuk membuat database.
![Screenshot 2024-01-15 111925](https://github.com/taufikalbani13/Lab1web/assets/115517181/11a9d236-7aa9-4c6f-a863-08ace21d6c50)
## Buat file ```lab9_php_modular``` pada root directory web server ```(c:\xampp\htdocs)```
![Screenshot 2024-01-15 113005](https://github.com/taufikalbani13/Lab1web/assets/115517181/4cf25e6a-f940-42ed-b026-8b3efc54fb01)
## Buat file baru dengan nama ```header.php```
```python
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Contoh Modularisasi</title>
    <link href="style.css" rel="stylesheet" type="text/stylesheet"media="screen" />
</head>
<body>
    <div class="container">
        <header>
            <h1>Modularisasi Menggunakan Require</h1>
        </header>
        <nav>
            <a href="home.php">Home</a>
            <a href="about.php">About</a>
            <a href="kontak.php">Kontak</a>
        </nav>
```
## Output
![Screenshot 2024-01-15 113025](https://github.com/taufikalbani13/Lab1web/assets/115517181/adeec9e5-70c9-4982-b6da-d19bafe6a29b)

## Buat file baru dengan nama ```footer.php```
```python
<footer>
    <p>&copy; 2023, Informatika, Universitas Pelita Bangsa</p>
</footer>
</div>
</body>
</html>
```
## Output
![Screenshot 2024-01-15 113036](https://github.com/taufikalbani13/Lab1web/assets/115517181/964cbecc-4505-4e4d-86d7-f8ce186907d5)
## Buat file baru dengan nama ```home.php```
```python
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman Home</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```
## Output
![Screenshot 2024-01-15 113047](https://github.com/taufikalbani13/Lab1web/assets/115517181/d64be784-8698-41a6-b445-69b79872e5b8)
## Buat file baru dengan nama ```about.php```
```python
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman About</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```
## Output
![Screenshot 2024-01-15 113104](https://github.com/taufikalbani13/Lab1web/assets/115517181/4e29f478-0d0f-47ea-a482-417ffb9d19fc)
## Pertanyaan dan Tugas
## Implementasikan konsep modularisasi pada kode program praktikum 8 tentang database, sehingga setiap halamannya memiliki template tampilan yang sama. Laporan Praktikum
## Membuat file baru dengan nama ```style.css```
```python
body {
    padding: 20px;
    background-color: #eee1aae8;
    font-family: Arial, Helvetica, sans-serif;
  }
  
  #header {
    background-color: 	#00FFFF;
    height: 120px;
  }
  
  #header h1 {
    color: #00125b;
    padding: 10px 0px 0px 20px;
    text-shadow: #fff 1px 1px 3px;
    float: left;
    color: #fff;
    font-family: "Exo", sans-serif;
    font-size: 35px;
    font-weight: 200;
  }
table{
    border-collapse:collapse;
    font:normal normal 12px Verdana,Arial,Sans-Serif;
    color:#333333;
}
table th {
    background:	#A52A2A;
    color:#DCDCDC;
    font-weight:bold;
    font-size:14px;
}
table th, td {
    vertical-align:top;
    padding:5px 10px;
    border:1px solid #696969;
}
table tr {
    background:#F5FFFA;
}
table tr:nth-child(even) {
    background:#F0F8FF;
}
form label {
    display: inline-block;
    width: 100px;
}
form input[type="submit"] {
    border: 1px solid #194a43;
    background-color: #197a43;
    color: #ffffff;
    font-weight: bold;
    padding: 10px 20px;
    position: relative;
}
form input[type="text"] {
    border: 1p solid #55213f;
}
nav {
    display: block;
    background-color: #0000FF;
    }
    nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
    }
    nav a.active,
    nav a:hover {
    background-color: #ea872b;
    }
  
  .content, .sidebar, .footer{
    padding: 1em;
  }
  
  nav ul {
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: space-between;
    text-align: center;
  }
  
  nav li{
    list-style: none;
    padding: 1em 0;
  }
  
  nav li a {
    color: white;
    font-weight: 700;
    opacity: 0.6;
    text-decoration: none;
    transition: 0.3s;
  }
  
  nav li a:hover {
    opacity: 1;
  }
  footer ul {
    max-width: 640px;
    margin: 2em auto;
    padding: 20px;
    text-align: center;
    display: flex;
    flex-direction: row;
    background-color: rgb(43, 33, 33);
    
    }
    
    footer ul li {
      list-style: none;
      align-self: flex-end;
    }
    
    footer ul li a{
      text-decoration: none;
      color: rgb(43, 33, 33);
    }
    
    footer ul li img {
      width: 30%;
    }
    
    footer p {
      font-size: 0.8em;
    }
```
