![Screenshot (5)](https://github.com/Najwaiffa/Lab3web/assets/115856206/daa00404-743d-42aa-b29e-0f979618402b)# Praktikum 3 web: Membuat List, Table dan Form

## Langkah-langkah Praktikum
-Persiapan membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

![Screenshot (1)](https://github.com/Najwaiffa/Lab3web/assets/115856206/bebf8c6e-e7c9-4ca7-85b1-4eb778b1a9c5)


### Membuat Ordered List
- Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
    </ol>
</section>
```
![Screenshot (2)](https://github.com/Najwaiffa/Lab3web/assets/115856206/4dd8ce9d-8464-4e37-b1dd-9f0c92cc3a49)


### Membuat Unorderd List
- Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada section unordered-list, seperti berikut.
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
      <li>Jaringan Komputer</li>
      <li>Struktur Data</li>
      <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

![Screenshot (3)](https://github.com/Najwaiffa/Lab3web/assets/115856206/523011c5-13df-49bc-a748-a1d309045682)



### Membuat Description List
- Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```
<section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industi</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntasi</dd>
            <dd>Manajemen</dd>
            <dd>BisnIS Digital</dd>
        </dl>
    </section>
```


![Screenshot (4)](https://github.com/Najwaiffa/Lab3web/assets/115856206/a812fde2-846f-40e9-97d6-4402ecf66c5e)



### Membuat Tabel
- Buat file baru dengan nama lab3_tabel.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML lanjutan</title>
</head>
<body>
  <header>
    <h1>Membuat table</h1>
  </header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<table border="1" cellpadding="4" cellspacing="3">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```

![Screenshot (5)](https://github.com/Najwaiffa/Lab3web/assets/115856206/b390f7fd-6d73-440a-b1ba-9c18cc4e24c6)


### Mengatur Margin dan Padding
- Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan cellspacing pada tag table.

```
<table border="1" cellpadding="4" cellspacing="3">
```

![Screenshot (9)](https://github.com/Najwaiffa/Lab3web/assets/115856206/04cd3ed9-821d-4d25-aadb-fb41db444681)



### Menggabungkan Sel Data
- Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara horizontal).
```
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td rowspan="3">Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```
![Screenshot (6)](https://github.com/Najwaiffa/Lab3web/assets/115856206/87c571be-d256-4a23-90c4-7f737b585ca8)


### Membuat Form
- Buat file baru dengan nama lab3_form.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>Membuat From</header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut.

```
form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
    <p>
        <label for="nama">Nama</label>
        <input type="text" id="nama" name="nama">
    </p>
    <p>
        <label for="alamat">Alamat</label>
        <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
        <label>Jenis Kelamin</label>
        <input id="jk_l" type="radio" name="kelamin" value="L" /><label
        for="jk_l">Laki-laki</label>
        <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        for="jk_p">Perempuan</label>
    </p>
        <p><input type="submit" value="Login"></p>
        </fieldset>
</form>
```

![Screenshot (7)](https://github.com/Najwaiffa/Lab3web/assets/115856206/0141cd91-b39e-44d8-ad17-91cfb583d68c)


### Menabahkan Style pada Form
- Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```
 <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```

![Screenshot (12)](https://github.com/Najwaiffa/Lab3web/assets/115856206/deb2cce6-3e2c-42a7-be65-39cb5217648d)


### Pertanyaan dan Tugas
- Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.


