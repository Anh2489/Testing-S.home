## NGHIÊN CỨU NGHIỆP VỤ VÀ SRS

**1. Mục đích**

Nghiên cứu nghiệp vụ và tài liệu SRS nhằm hiểu rõ yêu cầu của hệ thống,
từ đó xác định những nội dung cần kiểm tra trong quá trình kiểm thử.

**2. Nội dung nghiên cứu**

Tập trung phân tích:

- Actor thực hiện chức năng.
- Điều kiện trước khi thực hiện.
- Điều kiện sau khi thực hiện.
- Luồng nghiệp vụ chính.
- Các trường hợp ngoại lệ.
- Dữ liệu đầu vào.
- Quy tắc nghiệp vụ.
- Kết quả mong đợi.

**3. Phân tích Use Case "Tạo thương hiệu mới"**

***Thông tin chung***

- **Actor:** Quản trị viên.
- **Priority:** Cao.
- **Pre-condition:** Đã đăng nhập và có quyền tạo thương hiệu.

***Thông tin cần nhập***

| Trường | Yêu cầu |
|---|---|
| Tên thương hiệu | Bắt buộc, không được trùng |
| Slug | Không bắt buộc, tự sinh nếu bỏ trống |
| Logo | Không bắt buộc, JPG/PNG |
| Thứ tự hiển thị | Mặc định 0, số nguyên không âm |
| Trạng thái | Mặc định "Kích hoạt" |

***Luồng nghiệp vụ***

1. Quản trị viên mở chức năng tạo thương hiệu.
2. Hệ thống hiển thị form.
3. Nhập thông tin thương hiệu.
4. Nhấn "Tạo thương hiệu mới".
5. Hệ thống kiểm tra dữ liệu.
6. Nếu hợp lệ, thương hiệu được tạo thành công.
7. Dữ liệu được lưu và hiển thị trong danh sách.

***Các trường hợp cần chú ý***

- Bỏ trống tên thương hiệu.
- Tên thương hiệu bị trùng.
- Slug bị trùng hoặc sai định dạng.
- Logo không đúng định dạng.
- Thứ tự hiển thị không hợp lệ.
- Nhấn nút tạo nhiều lần.

**4. Kết quả nghiên cứu**

Em đã hiểu được cách đọc và phân tích một Use Case từ tài liệu SRS,
đồng thời xác định được các điều kiện và quy tắc nghiệp vụ cần
chuyển thành nội dung kiểm thử ở các tuần sau.
