# Spring Boot REST API - Manajemen Produk

Repositori ini merupakan implementasi sederhana REST API menggunakan **Spring Boot**, yang mendukung operasi CRUD (Create, Read, Update, Delete) untuk entitas **Product**.

#Teknologi yang Digunakan:
- Java 21 / 24
- Spring Boot 3.2.x
- Maven
- MySQL / MariaDB
- Jakarta Persistence (JPA)
- Spring Web
- Spring Data JPA

#Konfigurasi Database

1. Pastikan `application.properties` berisi konfigurasi berikut:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/penjualan
spring.datasource.username=root
spring.datasource.password=12345
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

ndpoint REST API
1. GET /api/products
Mendapatkan semua produk.

2. GET /api/products/{id}
Mendapatkan produk berdasarkan ID.

3. POST /api/products
Menambahkan produk baru.

json
Copy
Edit
{
  "name": "Keyboard",
  "price": 300000
}
4. PUT /api/products/{id}
Memperbarui data produk berdasarkan ID.

json
Copy
Edit
{
  "name": "Keyboard Gaming",
  "price": 500000
}
5. DELETE /api/products/{id}
Menghapus produk berdasarkan ID.

📁 Struktur Project
css
Copy
Edit
src/
└── main/
    ├── java/com/example/restapi/
    │   ├── controller/
    │   ├── model/
    │   ├── repository/
    │   ├── service/
    │   └── RestApiApplication.java
    └── resources/
        └── application.properties
