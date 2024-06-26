# Manajemen Daftar Buku
Studi Kasus - Manajemen Daftar Buku

REST API untuk mengelola daftar buku dalam sebuah perpustakaan. API ini akan memungkinkan pengguna untuk menambahkan, mengambil daftar, mengambil detail, memperbarui, dan menghapus buku dari perpustakaan.

Fitur:
- Mendapatkan daftar semua buku dalam perpustakaan.
- Mendapatkan detail buku berdasarkan ID.
- Menambahkan buku baru ke dalam perpustakaan.
- Memperbarui informasi buku berdasarkan ID.
- Menghapus buku dari perpustakaan berdasarkan ID.

Endpoint:
- GET /books: Mendapatkan daftar semua buku dalam perpustakaan.
- GET /books/{id}: Mendapatkan detail buku berdasarkan ID.
- POST /books: Menambahkan buku baru ke dalam perpustakaan.
- PUT /books/{id}: Memperbarui informasi buku berdasarkan ID.
- DELETE /books/{id}: Menghapus buku dari perpustakaan berdasarkan ID.

Instalasi:
-  git clone https://github.com/deliaanggun/repo-case-study.git
-  cd repo-case-study
-  mvn clean install
-  mvn spring-boot:run

Persyaratan:
- Java JDK 19
- Maven (https://maven.apache.org/)
- Database MySQL
- Postman Desktop Agent karena dijalankan secara lokal

Konfigurasi pada application.properties:
- spring.application.name=Books
- spring.datasource.url=jdbc:mysql://localhost:3306/Books
- spring.datasource.username=root
- spring.datasource.password=7890
- spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

- spring.datasource.testWhileIdle=true
- spring.datasource.validationQuery=SELECT 1

- spring.jpa.show-sql=true
- spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
- spring.jpa.hibernate.ddl-auto=update

- spring.h2.console.enabled=true
- spring.h2.console.path=/h2

