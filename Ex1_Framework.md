# Framework

#### 1. Khái niệm
- **Framework** là một bộ khung phần mềm, cung cấp bộ công cụ và kiến trúc chuẩn để phát triển ứng dụng. Nó bao gồm các thư viện, công cụ, và các quy tắc để hỗ trợ lập trình viên phát triển phần mềm một cách dễ dàng và hiệu quả. Framework định nghĩa các nguyên tắc và luồng xử lý, giúp lập trình viên tập trung vào logic nghiệp vụ thay vì các chi tiết kỹ thuật.

#### 2. Đặc điểm
- **Kiến trúc chuẩn**: Framework cung cấp một cấu trúc chuẩn cho ứng dụng, giúp tổ chức mã nguồn theo một cách rõ ràng và nhất quán.
- **Tái sử dụng mã nguồn**: Framework chứa các đoạn mã sẵn có, thư viện, và các module có thể tái sử dụng, giúp giảm thiểu công sức phát triển.
- **Quản lý luồng điều khiển**: Framework thường kiểm soát luồng điều khiển của ứng dụng (Inversion of Control - IoC), nghĩa là lập trình viên phải tuân theo cấu trúc mà framework đặt ra.
- **Cấu hình và thiết lập sẵn**: Cung cấp các cấu hình và thiết lập mặc định, giúp giảm thời gian cấu hình cho các tác vụ thường gặp (ví dụ: kết nối cơ sở dữ liệu, xử lý yêu cầu HTTP).
- **Hỗ trợ mở rộng**: Framework thường có khả năng mở rộng thông qua các plugin hoặc module bổ sung, giúp linh hoạt trong việc phát triển ứng dụng.

#### 3. Tác dụng
- Tiết kiệm thời gian phát triển
- Giảm thiểu lỗi
- Cải thiện hiệu suất
- Đảm bảo tuân thủ chuẩn
- Dễ dàng bảo trì và mở rộng
- Hỗ trợ cộng đồng và tài liệu


# Spring framework
### Spring Framework là gì?

**Spring Framework** là một framework mã nguồn mở cho phát triển ứng dụng Java, đặc biệt là ứng dụng web và enterprise. Được thiết kế để giúp đơn giản hóa việc phát triển ứng dụng Java, Spring cung cấp một cơ sở hạ tầng toàn diện để quản lý các tác vụ phổ biến như quản lý phụ thuộc (Dependency Injection - DI), quản lý giao dịch (Transaction Management), bảo mật, truy xuất dữ liệu, và phát triển web.

### Tác dụng của Spring Framework

1. **Quản lý phụ thuộc (Dependency Injection - DI)**:
   - Giúp tách rời các thành phần của ứng dụng, làm cho mã dễ bảo trì và dễ kiểm thử.
   - Giảm bớt sự phụ thuộc cứng nhắc giữa các lớp và module trong ứng dụng.

2. **Hỗ trợ lập trình hướng khía cạnh (Aspect-Oriented Programming - AOP)**:
   - Cho phép bổ sung chức năng (như logging, bảo mật, quản lý giao dịch) vào các phần của ứng dụng mà không làm thay đổi mã nguồn của chúng.
   - Giúp tách biệt các vấn đề quan tâm chéo (cross-cutting concerns) ra khỏi logic nghiệp vụ chính.

3. **Quản lý giao dịch (Transaction Management)**:
   - Cung cấp một cơ chế quản lý giao dịch mạnh mẽ và dễ sử dụng, hỗ trợ cả giao dịch phân tán.
   - Hỗ trợ lập trình viên làm việc với nhiều loại hệ quản trị cơ sở dữ liệu và môi trường phân tán.

4. **Tích hợp dễ dàng với các framework và công nghệ khác**:
   - Spring có thể tích hợp với nhiều công nghệ khác nhau như Hibernate, MyBatis, JPA, Kafka, RabbitMQ, v.v.
   - Hỗ trợ kết nối với nhiều hệ quản trị cơ sở dữ liệu và các dịch vụ bên ngoài.

5. **Hỗ trợ phát triển ứng dụng web và RESTful**:
   - **Spring MVC** cung cấp một kiến trúc Model-View-Controller mạnh mẽ để phát triển ứng dụng web.
   - **Spring WebFlux** hỗ trợ lập trình phản ứng (reactive programming) để phát triển ứng dụng web không đồng bộ, hiệu suất cao.

6. **Hỗ trợ phát triển microservices**:
   - **Spring Boot** và **Spring Cloud** giúp dễ dàng tạo và quản lý các microservices, hỗ trợ các công cụ cần thiết như discovery, gateway, config server, và circuit breaker.

### Các project trong Spring Framework và tác dụng của chúng

Spring Framework bao gồm nhiều project con (module) phục vụ cho các mục đích phát triển cụ thể. Dưới đây là một số project chính và tác dụng của chúng:

1. **Spring Core**:
   - **Tác dụng**: Cung cấp các tính năng cốt lõi của Spring như Dependency Injection (DI) và Inversion of Control (IoC). Đây là nền tảng của mọi module trong Spring Framework.
   - **Ứng dụng**: Tất cả các ứng dụng Spring đều sử dụng Spring Core để quản lý các đối tượng Java và các phụ thuộc của chúng.

2. **Spring MVC**:
   - **Tác dụng**: Cung cấp một framework Model-View-Controller (MVC) mạnh mẽ để phát triển các ứng dụng web dựa trên servlet.
   - **Ứng dụng**: Dùng để xây dựng các ứng dụng web dựa trên kiến trúc MVC truyền thống hoặc xây dựng RESTful API.

3. **Spring Boot**:
   - **Tác dụng**: Cung cấp cấu hình tự động, các dependencies mặc định, và embedded server để phát triển ứng dụng nhanh chóng và dễ dàng.
   - **Ứng dụng**: Dùng để phát triển các ứng dụng microservices và monolithic một cách nhanh chóng với ít cấu hình hơn.

4. **Spring Security**:
   - **Tác dụng**: Cung cấp các giải pháp bảo mật toàn diện cho ứng dụng như xác thực, phân quyền, bảo vệ chống tấn công CSRF (Cross-Site Request Forgery), và bảo vệ URL.
   - **Ứng dụng**: Dùng để bảo vệ các ứng dụng web, API, và microservices khỏi các mối đe dọa bảo mật.

5. **Spring Data**:
   - **Tác dụng**: Đơn giản hóa việc truy xuất và thao tác với dữ liệu từ các nguồn dữ liệu khác nhau (SQL, NoSQL, NewSQL, v.v.).
   - **Ứng dụng**: Dùng để tương tác với cơ sở dữ liệu một cách nhất quán và hiệu quả, hỗ trợ nhiều loại cơ sở dữ liệu.

6. **Spring Cloud**:
   - **Tác dụng**: Cung cấp các công cụ để phát triển và quản lý các ứng dụng phân tán, hỗ trợ microservices như service discovery, circuit breaker, config server, và API gateway.
   - **Ứng dụng**: Dùng để phát triển các hệ thống microservices phân tán và các ứng dụng đám mây.

7. **Spring WebFlux**:
   - **Tác dụng**: Cung cấp một framework lập trình phản ứng (reactive programming) cho các ứng dụng web, hỗ trợ các ứng dụng không đồng bộ và có hiệu suất cao.
   - **Ứng dụng**: Dùng để xây dựng các ứng dụng web và API không đồng bộ, tận dụng lập trình phản ứng cho hiệu suất cao.

8. **Spring Batch**:
   - **Tác dụng**: Hỗ trợ xử lý batch (xử lý khối lượng lớn dữ liệu theo lô), cung cấp các tính năng như job processing, chunk processing, và quản lý retry/skip.
   - **Ứng dụng**: Dùng trong các hệ thống cần xử lý dữ liệu lớn theo lô như ETL (Extract, Transform, Load), báo cáo, và xử lý batch.

9. **Spring Integration**:
   - **Tác dụng**: Cung cấp các công cụ để tích hợp các ứng dụng với nhau thông qua các mô hình tích hợp như messaging, data streaming, và event-driven architecture.
   - **Ứng dụng**: Dùng để tích hợp các hệ thống và dịch vụ khác nhau trong các ứng dụng doanh nghiệp.

# Framework Java khác
### 1. **Hibernate**
- **Loại**: Object-Relational Mapping (ORM) Framework, cung cấp một cách để ánh xạ các đối tượng Java đến các bảng cơ sở dữ liệu và ngược lại
- **Đặc điểm**:
  - **ORM mạnh mẽ**: Hibernate giúp chuyển đổi giữa các đối tượng Java và các bảng trong cơ sở dữ liệu quan hệ, cho phép thao tác với dữ liệu mà không cần viết mã SQL thủ công.
  - **Hỗ trợ caching**: Tích hợp cơ chế caching cấp 1 và cấp 2 để cải thiện hiệu suất khi truy vấn cơ sở dữ liệu.
  - **Query Language mạnh mẽ**: HQL (Hibernate Query Language) cho phép viết các truy vấn phức tạp và hỗ trợ đầy đủ các chức năng như join, group by, và các hàm tổng hợp.
  - **Hỗ trợ đa dạng cơ sở dữ liệu**: Hibernate có thể làm việc với nhiều loại cơ sở dữ liệu khác nhau thông qua cấu hình.

### 2. **Apache Struts**
- **Loại**: Web Application Framework (MVC) được sử dụng để phát triển các ứng dụng web Java
- **Đặc điểm**:
  - **Mô hình MVC**: Sử dụng mô hình Model-View-Controller giúp tách biệt rõ ràng giữa logic nghiệp vụ, giao diện người dùng, và điều hướng.
  - **Hỗ trợ mở rộng**: Dễ dàng mở rộng thông qua các plugin và thư viện hỗ trợ.
  - **Validation mạnh mẽ**: Cung cấp cơ chế validation dữ liệu đầu vào mạnh mẽ và linh hoạt.
  - **Hỗ trợ quốc tế hóa**: Tích hợp sẵn cơ chế hỗ trợ quốc tế hóa, giúp xây dựng ứng dụng đa ngôn ngữ dễ dàng.

### 3. **JavaServer Faces (JSF)**
- **Loại**: Web Application Framework (Component-Based) phát triển ứng dụng web dựa trên thành phần
- **Đặc điểm**:
  - **Component-based UI framework**: Cho phép phát triển các thành phần giao diện người dùng (UI components) tái sử dụng được.
  - **Event-driven programming**: Hỗ trợ lập trình dựa trên sự kiện, giúp xây dựng các giao diện người dùng tương tác.
  - **Tích hợp tốt với Java EE**: Là một phần của Java EE, JSF tích hợp dễ dàng với các công nghệ Java EE khác như EJB, JPA, và CDI.
  - **Hỗ trợ kéo-thả**: Nhiều IDE hỗ trợ JSF cho phép phát triển giao diện kéo-thả, giúp tăng tốc độ phát triển.

### 4. **Grails**
- **Loại**: Web Application Framework (Full-stack) dựa trên Groovy, ngôn ngữ có thể chạy trên JVM và tương thích với Java.
- **Đặc điểm**:
  - **Dựa trên Groovy**: Sử dụng ngôn ngữ Groovy, một ngôn ngữ động chạy trên JVM, giúp viết mã ngắn gọn và linh hoạt hơn.
  - **Convention over Configuration**: Sử dụng nguyên tắc "ưu tiên quy ước hơn cấu hình" giúp giảm thiểu cấu hình cần thiết, cho phép phát triển ứng dụng nhanh chóng.
  - **Tích hợp với Spring và Hibernate**: Grails sử dụng Spring Framework và Hibernate ORM trong backend, mang lại sự mạnh mẽ và tính năng phong phú.
  - **Plug-in ecosystem**: Cung cấp một hệ sinh thái plugin phong phú giúp mở rộng chức năng của ứng dụng một cách dễ dàng.

### 5. **Vaadin**
- **Loại**: Web Application Framework (Full-stack) phát triển ứng dụng web Java với trọng tâm là trải nghiệm người dùng (user experience - UX) và giao diện người dùng (user interface - UI).
- **Đặc điểm**:
  - **Server-side và Client-side**: Hỗ trợ cả lập trình phía server và phía client, giúp phát triển ứng dụng web phong phú với trải nghiệm người dùng tốt.
  - **Component-based**: Cung cấp nhiều thành phần giao diện người dùng UI (UI components) có sẵn, giúp xây dựng giao diện người dùng phức tạp một cách nhanh chóng.
  - **Two-way data binding**: Hỗ trợ ràng buộc dữ liệu hai chiều, giúp đồng bộ hóa dữ liệu giữa giao diện và backend một cách dễ dàng.
  - **Tích hợp với Spring Boot**: Dễ dàng tích hợp với Spring Boot để phát triển các ứng dụng web hiện đại.

### 6. **Play Framework**
- **Loại**: Web Application Framework (Reactive) nhấn mạnh vào hiệu suất và khả năng mở rộng
- **Đặc điểm**:
  - **Reactive Programming**: Hỗ trợ lập trình phản ứng (reactive programming), giúp phát triển các ứng dụng không đồng bộ và có hiệu suất cao.
  - **Stateless and Scalable**: Thiết kế không trạng thái (stateless), giúp dễ dàng mở rộng quy mô ứng dụng.
  - **Hot Reloading**: Hỗ trợ hot reloading, giúp nhà phát triển thấy ngay các thay đổi trong mã mà không cần khởi động lại server.
  - **Full-stack capabilities**: Cung cấp tất cả những gì cần thiết để phát triển ứng dụng từ frontend đến backend, bao gồm cả templating, validation, và routing.

### 7. **Apache Wicket**
- **Loại**: Web Application Framework (Component-Based) phát triển ứng dụng web Java dựa trên thành phần (component-based) và hướng đối tượng (object-oriented).
- **Đặc điểm**:
  - **Component-oriented**: Tập trung vào phát triển ứng dụng web dựa trên các thành phần (components), giúp tái sử dụng mã và tăng tính modular.
  - **Plain HTML**: Hỗ trợ sử dụng các file HTML tĩnh cho các view, giúp tách biệt rõ ràng giữa logic và giao diện.
  - **Stateful framework**: Hỗ trợ quản lý trạng thái server-side, giúp phát triển các ứng dụng có giao diện phức tạp mà không cần sử dụng quá nhiều mã JavaScript.
  - **Secure by default**: Tích hợp các tính năng bảo mật mặc định như bảo vệ chống tấn công CSRF và XSS.

### 8. **Dropwizard**
- **Loại**: Web Service Framework (Microservices) phát triển dịch vụ RESTful dựa trên Java, tập trung vào đơn giản hóa quá trình phát triển và triển khai ứng dụng
- **Đặc điểm**:
  - **Lightweight**: Tập trung vào phát triển các ứng dụng web và microservices nhẹ, giúp triển khai và bảo trì dễ dàng.
  - **Production-ready**: Được cấu hình sẵn để sẵn sàng triển khai trên môi trường production với các tính năng như logging, metrics, và health checks.
  - **RESTful API development**: Được thiết kế để xây dựng RESTful APIs với cấu trúc và conventions đơn giản.
  - **Tích hợp với nhiều thư viện phổ biến**: Sử dụng Jackson cho JSON, Jersey cho REST, Jetty cho server-side.

### 9. **Apache Spark (Java API)**
- **Loại**: Big Data Framework xử lý dữ liệu phân tán (distributed data processing) mã nguồn mở, được thiết kế để xử lý các khối lượng dữ liệu lớn một cách nhanh chóng và hiệu quả
- **Đặc điểm**:
  - **Data Processing**: Hỗ trợ xử lý dữ liệu lớn trên phân tán với hiệu suất cao thông qua cơ chế in-memory computing.
  - **API phong phú**: Cung cấp API phong phú cho nhiều ngôn ngữ lập trình như Java, Scala, Python, và R.
  - **Machine Learning and Graph Processing**: Hỗ trợ các thư viện tích hợp cho học máy (MLlib) và xử lý đồ thị (GraphX).
  - **Integration with Hadoop**: Dễ dàng tích hợp với hệ sinh thái Hadoop và các công cụ dữ liệu lớn khác.

### 10. **Micronaut**
- **Loại**: Microservices Framework phát triển microservices và ứng dụng serverless với bộ nhớ nhỏ và khởi động nhanh. Tối ưu cho các dự án cần phát triển dịch vụ microservices hiệu suất cao với khả năng mở rộng tốt
- **Đặc điểm**:
  - **Low memory footprint**: Thiết kế nhẹ và tối ưu cho các ứng dụng microservices, sử dụng ít bộ nhớ hơn so với các framework khác.
  - **Compile-time Dependency Injection**: Tối ưu hóa DI và AOP trong quá trình biên dịch, giúp tăng tốc độ khởi động ứng dụng.
  - **Reactive programming support**: Hỗ trợ lập trình phản ứng, giúp xây dựng các ứng dụng có khả năng đáp ứng nhanh.
  - **Native cloud support**: Hỗ trợ native cho các dịch vụ đám mây và serverless, dễ dàng triển khai trên các nền tảng như AWS Lambda, Azure Functions.
