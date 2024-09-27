# Web Java

Project Java Web xây dựng một Shop Bán Sách
![Catalog](https://user-images.githubusercontent.com/60851390/228592444-282493ee-7ebd-4115-b40f-af23ec7dfa08.png)


## A. Java Web Project to build a Book Shop

### 1. Nạp hình ảnh

Tạo thư mục C:/var/webapp/images và giải nén tất cả hình từ file [var-webapp-images.zip](https://github.com/markiusphan/BookShopWeb/blob/main/init/var-webapp-images.zip) vào thư mục này.

### 2. Tạo database

Mở MySQL Workbench → Open SQL Script → Execute [bookshopdb.sql](https://github.com/markiusphan/BookShopWeb/blob/main/init/bookshopdb.sql)

### 3. Nạp project vào IDEA

Mở IDEA → Get from VCS (màn hình Welcome) hoặc File | New | Project from Version Control (màn hình bình thường) → Clone project theo URL: https://github.com/markiusphan/BookShopWeb.git

### 4. Cấu hình Tomcat

- [Add Configuration...] → [+] Tomcat Server Local
- [Fix] → BookShopWeb:war exploded

### 5. Run (Shift+F10)

## B. Cấu hình utils.ConstantUtils

- Mặc định, DB_NAME là bookshopdb, DB_USERNAME là root, DB_PASSWORD là 12345.
- Có thể thay đổi nếu như khác.

# Sơ đồ CSDL

![DatabaseDesignBSW](https://user-images.githubusercontent.com/60851390/184755435-bb97a62a-4cdd-408d-9a5a-526430f50c64.svg)
# Phần mềm

- IDEA 2022.1.2
- MySQL Workbench 8.0.25
- Tomcat 9.0.48

## Cài đặt Tomcat 9.0.48

- Tải ở: https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.48/bin/ (apache-tomcat-9.0.48.zip cho Windows và apache-tomcat-9.0.48.tar.gz cho Mac)
- Mở IDEA và thêm vào File | Settings | Build, Execution, Deployment | Application Servers > [+] Tomcat Server (Tomcat Home trỏ đến thư mục Tomcat, ví dụ: apache-tomcat-9.0.48)
