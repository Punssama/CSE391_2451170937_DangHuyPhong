# 10 input types khác nhau trong HTML5

| Input type | Giao diện hiển thị | Validation tự động | Use case trong trang E-Commerce |
|---|---|---|---|
| `text` | Ô nhập một dòng văn bản, hiển thị đơn giản | Không kiểm tra định dạng cụ thể, nhưng có thể dùng `required`, `minlength`, `maxlength` | Nhập họ tên khách hàng, tên người nhận |
| `email` | Ô nhập văn bản một dòng, thường có biểu tượng/kiểu nhập phù hợp cho email | Kiểm tra đúng định dạng email, ví dụ có ký tự `@` | Nhập email đăng ký, nhận đơn hàng, khôi phục mật khẩu |
| `password` | Ô nhập bị che ký tự bằng dấu chấm hoặc sao | Không kiểm tra độ mạnh mật khẩu, nhưng có thể kết hợp `required`, `minlength` | Tạo tài khoản, đăng nhập, đổi mật khẩu |
| `number` | Ô nhập số, thường có nút tăng/giảm | Chỉ cho nhập số, hỗ trợ `min`, `max`, `step` | Nhập số lượng sản phẩm, mã giảm giá dạng số, tuổi khách hàng |
| `tel` | Ô nhập số điện thoại, giao diện tương tự text | Không tự kiểm tra định dạng chuẩn quốc tế, nhưng có thể dùng `pattern` | Nhập số điện thoại giao hàng hoặc xác minh OTP |
| `date` | Bộ chọn ngày tháng, thường là lịch | Kiểm tra giá trị ngày hợp lệ, hỗ trợ `min`, `max` | Chọn ngày giao hàng, ngày sinh khách hàng |
| `time` | Bộ chọn giờ phút | Kiểm tra giá trị thời gian hợp lệ | Chọn khung giờ nhận hàng hoặc giờ hẹn giao |
| `file` | Nút chọn tệp từ thiết bị | Có thể giới hạn bằng `accept`, `multiple` | Tải ảnh sản phẩm, ảnh hóa đơn, ảnh xác minh đơn hàng |
| `checkbox` | Ô chọn bật/tắt, có thể chọn nhiều mục | Có thể bắt buộc chọn bằng `required` | Chọn đồng ý điều khoản, chọn nhiều sở thích hoặc phương thức nhận tin |
| `radio` | Nhiều nút chọn một trong nhiều lựa chọn | Trong cùng nhóm chỉ chọn được một giá trị, có thể `required` | Chọn phương thức thanh toán, chọn kích cỡ sản phẩm, chọn giới tính trong hồ sơ |

## Ghi chú

- HTML5 đã hỗ trợ nhiều kiểu input giúp giảm lỗi nhập liệu.
- Kết hợp thêm các thuộc tính như `required`, `min`, `max`, `pattern`, `step`, `maxlength` để kiểm soát dữ liệu tốt hơn.
