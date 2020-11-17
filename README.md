# Tugas 11 MySQL
#### 1. Buatlah user baru dengan nama Niomic dengan password c0b4d1b4c4!
```
CREATE USER 'Niomic@localhost' IDENTIFIED BY 'c0b4d1b4c4';
```

#### 2. Ubah password menjadi indonesiaku dengan perintah update set
```
UPDATE USER SET Password = PASSWORD('indonesiaku') WHERE User = "Budi";
FLUSH PRIVILEGES;
```

#### 3. Berikan hak akses ke user Niomic untuk tabel mahasiswa pada database belajar
```
GRANT ALL ON belajar.mahasiswa TO Niomic@localhost;
```

#### 4. Hapus user Niomic
```
DROP USER 'Niomic';
```
