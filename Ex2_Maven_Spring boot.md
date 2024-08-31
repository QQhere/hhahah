# Spring Boot

**Spring Boot** là một phần của Spring Framework, được thiết kế để đơn giản hóa quá trình phát triển ứng dụng Spring. Nó cung cấp một bộ công cụ mạnh mẽ và cấu hình sẵn sàng giúp lập trình viên xây dựng ứng dụng Java dễ dàng và nhanh chóng hơn. Với Spring Boot, việc thiết lập một ứng dụng Spring từ đầu trở nên đơn giản hơn rất nhiều nhờ vào các cấu hình mặc định và một bộ công cụ mạnh mẽ.

#### Các đặc điểm nổi bật của Spring Boot:
1. **Auto-Configuration (Cấu hình tự động)**: Spring Boot tự động cấu hình ứng dụng dựa trên các thư viện và dependency đã thêm vào project. Điều này giúp giảm thiểu công việc cấu hình thủ công.

2. **Embedded Server (Máy chủ nhúng)**: Spring Boot đi kèm với máy chủ nhúng (như Tomcat, Jetty, hoặc Undertow), giúp dễ dàng chạy ứng dụng mà không cần cài đặt máy chủ web riêng biệt.

3. **Spring Boot Starter**: Đây là các dependency module đóng gói sẵn, giúp dễ dàng thêm các tính năng phổ biến vào ứng dụng Spring của mình mà không cần phải thêm từng dependency riêng lẻ.

4. **Spring Boot CLI**: Công cụ dòng lệnh này giúp nhanh chóng tạo và chạy các ứng dụng Spring bằng cách sử dụng Groovy.

5. **Production-ready Features**: Cung cấp các tính năng hữu ích như giám sát (monitoring), quản lý và kiểm tra tình trạng (health checks), tất cả đều được tích hợp sẵn để chuẩn bị cho việc triển khai trong môi trường sản xuất.

### Khởi tạo Project Spring Boot

Có nhiều cách để khởi tạo một dự án Spring Boot, bao gồm sử dụng Spring Initializr (một công cụ trực tuyến), Spring Boot CLI, hoặc trực tiếp từ các IDE như IntelliJ IDEA, Eclipse hoặc VS Code.

#### Cách khởi tạo Project Spring Boot bằng Spring Initializr:

1. **Truy cập Spring Initializr**:
   - Mở trình duyệt và truy cập [Spring Initializr](https://start.spring.io).

2. **Cấu hình dự án**:
   - **Project**: Chọn Maven Project (hoặc Gradle).
   - **Language**: Chọn Java.
   - **Spring Boot Version**: Chọn phiên bản Spring Boot.
   - **Project Metadata**: Nhập các thông tin như Group (ví dụ: `com.example`), Artifact (ví dụ: `demo`), và các thông tin khác.

3. **Chọn Dependencies (Thư viện phụ thuộc)**:
   - Chọn các dependency cho dự án. Ví dụ: `Spring Web`, `Spring Data JPA`, `Spring Security`, v.v.

4. **Generate Project**:
   - Nhấn nút "Generate" để tải về một file `.zip` chứa mã nguồn của dự án.

5. **Import Project vào IDE**:
   - Giải nén file `.zip` và import dự án vào IDE.

#### Chạy Project Spring Boot:
- Sau khi import vào IDE, chạy dự án bằng cách tìm class có chứa phương thức `main()` (thường nằm trong file có tên `Application.java`) và chạy nó như một ứng dụng Java thông thường. Spring Boot sẽ tự động khởi động server nhúng (như Tomcat).

### Hiểu về Maven và Cách Thêm Thư viện Maven

**Maven** là một công cụ quản lý dự án và build automation cho Java. Nó giúp quản lý các thư viện phụ thuộc (dependencies), xây dựng dự án, và đóng gói ứng dụng.

#### Các khái niệm cơ bản về Maven:

1. **POM (Project Object Model)**: File `pom.xml` là trung tâm của dự án Maven. Nó chứa thông tin cấu hình dự án và khai báo các thư viện phụ thuộc (dependencies), plugins, và các cấu hình build khác.

2. **Dependencies**: Maven quản lý các thư viện mà dự án phụ thuộc vào. Chỉ cần khai báo các thư viện này trong file `pom.xml` và Maven sẽ tự động tải về các thư viện cần thiết từ kho lưu trữ (mặc định Central Repository).

3. **Build Lifecycle**: Maven có một chu trình build lifecycle định nghĩa các bước build như `compile`, `test`, `package`, `install`, và `deploy`.

#### Cách thêm thư viện vào Maven:

Thêm phần khai báo dependency vào file `pom.xml` của dự án.

Ví dụ: Thêm thư viện `Spring Web`, trong file `pom.xml` thêm đoạn sau vào thẻ `dependencies`:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

- **groupId**: Xác định tổ chức hoặc nhóm của thư viện (vd: `org.springframework.boot`).
- **artifactId**: Tên của thư viện cụ thể (vd: `spring-boot-starter-web`).
- **version**: Phiên bản của thư viện (mặc định là phiên bản mới nhất).

#### Cập nhật dependencies:

- Sau khi thêm các dependencies vào `pom.xml`, cần cập nhật dự án để Maven tải về các thư viện mới.
