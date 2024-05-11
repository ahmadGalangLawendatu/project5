# project5 # Create CRUD API Using Flask and Docker

Tools yang harus disiapkan:

- docker
- postman
- visual code

API yang dibuat:

- create user
- update user
- get user
- delete user


Step 1 Pastikan telah menginstal Docker, Postman, dan Visual Studio Code.

Step 2 Buat direktori untuk proyek Anda. Di dalamnya, buat file-file berikut:
app.py: File utama Flask yang akan berisi kode untuk API CRUD. Dockerfile: File konfigurasi Docker untuk mengatur container Docker. requirements bxt: File yang berisi daftar dependensi Python yang dibutuhkan.

Step 3 Kode Flask CRUD API (app.py) Berisi database untuk menyimpan data user seperti create user, update user, get user, delete user.

Step 4 Dockerfile
File konfigurasi Docker (Dockerfile) untuk Flask yang berisi base image Python, Set working directory, Copy requirements file, Install dependencies, Copy kode Flask, Expose port 5000, Menjalankan aplikasi Flask. 

Step 5 Persiapan Docker
Pada terminal, masuk ke direktori proyek dan jalankan perintah-perintah berikut:
Build Docker image
docker build -t flask-crud .
Run Docker container
docker run -d -p 5000:5000 --name flask-crud-app flask-crud

Step 6 connect database sample di DBeaver

Step 7 Testing API menggunakan Postman
Buka Postman.
Gunakan URL http://localhost:5000/user untuk membuat, mengupdate, atau menghapus user.
Gunakan metode HTTP yang sesuai (POST, PUT, GET, DELETE) untuk menguji masing-masing operasi.

