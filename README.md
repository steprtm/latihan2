
# LAPORAN PRAKTIKUM BASIS DATA
Stephen Pratama Kurnia 312210635 TI.22.A.5

## BAB I PENDAHULUAN
1.1. Latar Belakang

MySQL adalah sistem basis data open source yang populer dan banyak digunakan dalam industri teknologi. Praktikum membuat tabel basis data MySQL bertujuan untuk mengajarkan peserta cara membuat dan mengelola tabel dalam sistem basis data MySQL, serta meningkatkan keterampilan teknis dalam pengelolaan basis data. Praktikum ini juga mempersiapkan peserta untuk bekerja dengan sistem basis data MySQL dalam pengembangan aplikasi web dan desktop.

1.2. Tujuan

Tujuan praktikum membuat tabel basis data MySQL adalah untuk mengajarkan peserta cara membuat dan mengelola tabel dalam sistem basis data MySQL, serta meningkatkan keterampilan teknis dalam pengelolaan basis data. Praktikum ini juga mempersiapkan peserta untuk bekerja dengan sistem basis data MySQL dalam pengembangan aplikasi web dan desktop.
## BAB II DASAR TEORI


Dasar teori praktikum membuat tabel basis data MySQL meliputi sistem basis data MySQL, tabel, field, record, primary key, foreign key, dan normalisasi. Hal ini penting untuk dipahami agar peserta dapat memahami konsep-konsep dasar dalam pembuatan dan pengelolaan tabel dalam sistem basis data MySQL.

2.1. Commands yang dipakai.

    1. SHOW
    2. CREATE
    3. DROP
    4. USE
    5. DESC / DESCRIBE
    6. ALTER
2.2. Contoh Pemakaian Commands diatas.

Untuk membuat Database


CREATE DATABASE [nama database];

Memakai tabel yang baru dibuat

USE [nama database];

Membuat tabel

CREATE TABLE [nama tabel] (nama VARCHAR(100), alamat TEXT);

Menambahkan kolom

ALTER TABLE [nama tabel] ADD COLUMN [nama kolom] [tipe data];

Menambah kolom diawal

ALTER TABLE [nama tabel] ADD COLUMN [nama kolom] [tipe data] FIRST;

Mengubah nama kolom

ALTER TABLE [nama tabel] CHANGE [nama kolom lama] [nama kolom baru] [tipe data];

Mengubah tipe data

ALTER TABLE [nama tabel] MODIFY COLUMN [nama kolom] [tipe data];

Menghapus kolom

ALTER TABLE [nama tabel] DROP COLUMN [nama kolom];

Menambahkan PRIMARY KEY

ALTER TABLE [nama tabel] ADD PRIMARY KEY([nama kolom]);

Menambahkan CONSTRAINT

ALTER TABLE [nama tabel] ADD CONSTRAINT [nama constraint] PRIMARY KEY ([nama kolom]);

Menghapus PRIMARY KEY

ALTER TABLE [nama tabel] DROP PRIMARY KEY;

Menghapus CONSTRAINT

ALTER TABLE [nama tabel] DROP CONSTRAINT [nama constraint];

## BAB III LANGKAH-LANGKAH PEMBUATAN

3.1. LANGKAH-LANGKAH


CREATE DATABASE latihan2;

USE latihan2;

CREATE TABLE biodata (mama varchar(100), alamat text);

ALTER TABLE biodata ADD COLUMN keterangan varchar(15);

ALTER TABLE biodata ADD COLUMN id int(11) FIRST;

ALTER TABLE biodata ADD COLUMN phone varchar(15) AFTER alamat;

ALTER TABLE biodata MODIFY COLUMN id char(11);

ALTER TABLE biodata CHANGE phone hp varchar(20);

ALTER TABLE biodata ADD COLUMN email varchar(40) AFTER hp;

ALTER TABLE biodata DROP COLUMN keterangan;

RENAME TABLE biodata TO data_mahasiswa;

ALTER TABLE data_mahasiswa CHANGE id nim varchar(255);

ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);

ALTER TABLE data_mahasiswa ADD CONSTRAINT unique_email unique (email);

3.2. SCREENSHOT OUTPUT

https://ibb.co/QkHM97B

https://ibb.co/fNLptLT
## BAB III LANGKAH-LANGKAH PEMBUATAN

3.1. LANGKAH-LANGKAH


CREATE DATABASE latihan2;

USE latihan2;

CREATE TABLE biodata (mama varchar(100), alamat text);

ALTER TABLE biodata ADD COLUMN keterangan varchar(15);

ALTER TABLE biodata ADD COLUMN id int(11) FIRST;

ALTER TABLE biodata ADD COLUMN phone varchar(15) AFTER alamat;

ALTER TABLE biodata MODIFY COLUMN id char(11);

ALTER TABLE biodata CHANGE phone hp varchar(20);

ALTER TABLE biodata ADD COLUMN email varchar(40) AFTER hp;

ALTER TABLE biodata DROP COLUMN keterangan;

RENAME TABLE biodata TO data_mahasiswa;

ALTER TABLE data_mahasiswa CHANGE id nim varchar(255);

ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);

ALTER TABLE data_mahasiswa ADD CONSTRAINT unique_email unique (email);

3.2. SCREENSHOT OUTPUT

https://ibb.co/QkHM97B

https://ibb.co/fNLptLT

## BAB IV PENUTUP
4.1. KESIMPULAN


 Praktikum membuat tabel dalam MySQL menggunakan XAMPP dan Git merupakan salah satu cara untuk memperoleh pemahaman dasar tentang cara membuat tabel dalam database MySQL. Dalam praktikum ini, peserta mempelajari bahwa MySQL adalah salah satu database management system (DBMS) yang paling populer dan banyak digunakan di seluruh dunia. XAMPP adalah salah satu paket software yang memungkinkan penggunaan MySQL, PHP, dan Apache dalam lingkungan lokal.

Selama praktikum, peserta belajar bagaimana membuat tabel dalam MySQL menggunakan perintah CREATE TABLE. Namun, sebelum membuat tabel, pengguna harus terlebih dahulu membuat database. Setelah database dibuat, pengguna dapat memulai membuat tabel dengan mengidentifikasi kolom atau field yang dibutuhkan dan jenis data yang cocok untuk setiap kolom tersebut.

Peserta juga diajarkan tentang konsep dasar database, seperti primary key, foreign key, dan indeks. Primary key adalah kolom yang unik dan dapat dijadikan sebagai identitas untuk setiap baris atau record dalam tabel. Foreign key digunakan untuk menghubungkan dua tabel dalam database, sedangkan indeks digunakan untuk mempercepat proses pencarian data dalam tabel.

Selain itu, peserta juga mempelajari cara menggunakan Git untuk melakukan version control dalam proyek pembuatan tabel. Dengan menggunakan Git, peserta dapat melacak perubahan dalam kode dan memastikan bahwa semua anggota tim memiliki akses ke versi terbaru dari proyek.

Secara keseluruhan, praktikum membuat tabel dalam MySQL menggunakan XAMPP dan Git merupakan langkah awal untuk memahami bagaimana cara bekerja dengan database, termasuk membuat tabel, mengelola data, dan melacak perubahan dalam proyek.