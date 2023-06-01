**Mạng bridge mặc định:**

Mạng bridge mặc định là một mạng mặc định được Docker cung cấp khi bạn cài đặt Docker.
Khi bạn tạo một container mới mà không chỉ định mạng, Docker sẽ tự động gán container đó vào mạng bridge mặc định.
Mạng bridge mặc định cho phép các container trên cùng mạng bridge giao tiếp với nhau bằng cách sử dụng tên container làm hostname. Các container được gán địa chỉ IP trong dải mạng bridge mặc định.
Mạng bridge mặc định không có sự cấu hình hoặc tùy chỉnh từ người dùng và cung cấp một môi trường đơn giản để chạy các container.

**Mạng bridge do người dùng tự tạo:**

Bên cạnh mạng bridge mặc định, Docker cũng cho phép người dùng tự tạo các mạng bridge tùy chỉnh.
Khi bạn tạo một mạng bridge mới, Docker sẽ tạo một mạng riêng biệt với các cài đặt mạng và cấu hình tùy chỉnh do bạn chỉ định.
Mạng bridge do người dùng tự tạo cho phép bạn kiểm soát và tùy chỉnh các cài đặt mạng như địa chỉ IP, dải mạng, DNS, tên miền và các cài đặt mạng khác.
Mạng bridge tùy chỉnh cho phép bạn tạo ra các mạng riêng biệt để phân chia các container thành các nhóm riêng biệt và tăng tính bảo mật và cách ly giữa chúng.
