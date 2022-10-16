# TUTORIAL CARA PENGGUNAAN GIT
## 1. Instal software [GIT](https://git-scm.com/downloads) terlebih dahulu
![Screenshot 2022-10-16 162228](https://user-images.githubusercontent.com/94947436/196030518-384ea109-1c32-488a-aed8-8274e110da1a.png)

## 2. Buat Folder baru 
Buat Folder yang ingin kalian jadikan untuk tempat menaruh tugas praktikum dan klik kanan pada Folder teresbut. lalu klik ***"GIT Bash Here"***

![Screenshot (45)](https://user-images.githubusercontent.com/94947436/196030797-a4efc7fa-413f-489c-91f5-63e77af1a8d1.png)

## 3. Menambahkan Global Config
• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan
saat menjalankan perintah git commit
> ***$ git config --global user.name "UsernameAnda"***
> 
> ***$ git config --global user.email "email anda"***

![Screenshot (46)](https://user-images.githubusercontent.com/94947436/196031262-f3192111-77d2-4948-bd93-2516844b0f64.png)

## 4. Membuat Repository Local
• Buat Folder project praktikum pertama dengan nama ***latihan1*** dan masuk ke dalam Foldernya dengan perintah ***cd*** (Change Directory)
> ***$ mkdir latihan1***
> 
> ***$ cd latihan1***

>note : lihat perubahannya di bagian text berwarna kuning, yang awalnya **../LatihanVCS** menjadi **../LatihanVCS/latihan1**

![Screenshot (47)](https://user-images.githubusercontent.com/94947436/196032306-9dba0c31-6977-4d5f-ba4b-34888f0c6710.png)

• Jalankan perintah ***git init***, untuk membuat repository local.
> ***$ git init***

>note : lihat perubahannya di bagian text berwarna kuning. di akhir nya terdapat text berwarna biru dengan tulisan (master). artinya ***GIT*** akan merekam seluruh aktifitas yang kalian lakukan di dalam folder tersebut.

![Screenshot (48)](https://user-images.githubusercontent.com/94947436/196033378-244af89f-3e79-415f-a9eb-ef3b5941551b.png)

• Repository baru berhasil di inisialisasi, dengan terbentuknya satu
direktori hidden dengan nama .git

![Screenshot (53)](https://user-images.githubusercontent.com/94947436/196033388-8a5b7908-5918-41ef-9d23-09f78b029414.png)


## 5. Menambah File Baru di Repository
• Untuk membuat file baru dapat menggunakan text editor seperti VS Code, lalu menyimpan filenya pada direktori aktif (repository)

• Disini kita akan coba buat satu file menggunakan ***GIT*** bernama README.md (text file) yang didalamnya terdapat kalimat ***"# Saya sedang belajar GIT"***

> ***$ echo “# Saya sedang belajar GIT” >> README.md***

![Screenshot (52)](https://user-images.githubusercontent.com/94947436/196034177-c6afce95-ab5b-4fdb-b042-841d3b531aa1.png)

## 6. Menyimpan Perubahan Ke Database
• Untuk menambahkan file yang baru saja dibuat tersebut, gunakan perintah ***git add***.

> ***$ git add README.md***

![Screenshot (54)](https://user-images.githubusercontent.com/94947436/196034694-053fb1b3-e171-4cdf-932a-09e187c17d2c.png)

>note : jika ingin melihat statusnya sudah berhasil atau belum bisa ketik perintah ***$git status***. Jika file berhasil ditambah, statusnya akan berwarna hijau, jika belum akan berwarna merah.

![Screenshot (56)](https://user-images.githubusercontent.com/94947436/196034973-3c1c22a1-8bb1-4c7a-95ae-4ca8c9405ab0.png)

• Untuk menyimpan perubahan yang ada ke dalam database repository local, gunakan perintah ***git commit -m “komentar commit”***

> ***$ git commit -m "File pertama saya :D"***

![Screenshot (57)](https://user-images.githubusercontent.com/94947436/196035307-e75752ef-8a42-4e8b-ab46-22e921fdb745.png)

## 7. Membuat repository server
• Server repository yang akan kita gunakan adalah ***GITHUB***

• Anda harus membuat akun terlebih dahulu di ***[GITHUB](http://github.com)***

• Setelah membuat akun, dari menu home klik ikon **(+)** lalu klik ***New Repository***

![Screenshot (59)](https://user-images.githubusercontent.com/94947436/196035496-10c21207-e789-4e80-9bf4-5054398e40c0.png)

• Isi nama repositorynya lalu klik create repository 

![Screenshot (60)](https://user-images.githubusercontent.com/94947436/196035591-4f500bb5-c8c5-429a-a77b-d2a649aa0cb5.png)

## 8. Menambahkan Remote Repository
• Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

• Gunakan perintah
> ***$ git remote add origin [url]***

![Screenshot (63)](https://user-images.githubusercontent.com/94947436/196036003-afdc379e-5048-4350-96d2-d5b148211ef3.png)

• Untuk mendapatkan URL nya klik copy pada web github yang terakhir kali kita lihat setelah membuat repository

![Screenshot (61)](https://user-images.githubusercontent.com/94947436/196036070-c34df9ef-30c2-4d9b-9ffb-7342c5353127.png)

## 9. Mengirim Perubahan ke server
• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push
> ***$ git push -u origin master***

![Screenshot (64)](https://user-images.githubusercontent.com/94947436/196036252-2e137ebd-21e4-4e05-bcbc-5acc4031bfee.png)

