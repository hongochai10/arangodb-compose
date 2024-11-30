# Giới thiệu
Dự án này sử dụng Docker Compose để triển khai ArangoDB, một cơ sở dữ liệu NoSQL mạnh mẽ. Tệp `compose.yaml` định nghĩa cấu hình cho dịch vụ ArangoDB, bao gồm các thông số như phiên bản, tài nguyên, biến môi trường và mạng.

# Cấu trúc thư mục
- `compose.yaml`: Tệp cấu hình cho Docker Compose.
- `.env`: Tệp chứa các biến môi trường cần thiết cho việc cấu hình dịch vụ.
- `.gitignore`: Tệp để xác định các tệp không cần thiết cho hệ thống kiểm soát phiên bản.

# Cách sử dụng
1. **Cài đặt Docker và Docker Compose**: Đảm bảo rằng bạn đã cài đặt Docker và Docker Compose trên máy của mình.
2. **Tạo mạng Docker**: Trước khi khởi động dịch vụ, bạn cần tạo mạng `baota_net` bằng lệnh sau:
   ```bash
   docker network create baota_net
   ```
3. **Cấu hình biến môi trường**: Mở tệp `.env` và điều chỉnh các biến như `VERSION`, `HOST_IP`, `PORT`, và `PASSWORD` theo nhu cầu của bạn.
4. **Khởi động dịch vụ**: Chạy lệnh sau trong thư mục chứa tệp `compose.yaml`:
   ```bash
   docker-compose up -d
   ```
5. **Truy cập ArangoDB**: Sau khi dịch vụ khởi động, bạn có thể truy cập ArangoDB thông qua trình duyệt tại địa chỉ `http://<HOST_IP>:<PORT>`.

# Lưu ý
- Đảm bảo rằng bạn đã tạo mạng `baota_net` trước khi khởi động dịch vụ.
- Kiểm tra tài nguyên hệ thống của bạn để đảm bảo rằng nó có thể đáp ứng các giới hạn đã chỉ định trong tệp `compose.yaml`.

# Liên hệ
Nếu bạn gặp bất kỳ vấn đề nào, vui lòng liên hệ với tác giả Ho Ngoc Hai hoặc mở một vấn đề trên kho lưu trữ GitHub của dự án.

# Giấy phép
Dự án này được cấp phép theo Giấy phép MIT. Bạn có thể tự do sử dụng, sao chép, sửa đổi và phân phối mã nguồn, miễn là bạn bao gồm thông báo bản quyền và giấy phép trong tất cả các bản sao hoặc phần của phần mềm.

# Cảm ơn bạn đã sử dụng ArangoDB!
