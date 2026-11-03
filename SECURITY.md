# Bảo mật

## Báo lỗ hổng

Vui lòng **không mở issue công khai**. Gửi riêng tới **kythuat@hvn.vn** hoặc qua
[GitHub Security Advisories](https://github.com/hvngroup/app-hvn-key-releases/security/advisories/new),
kèm phiên bản bị ảnh hưởng và các bước tái hiện. HVN GROUP phản hồi trong vài ngày làm việc và ghi công người báo
trong release notes nếu anh/chị muốn.

Không gửi kèm dữ liệu nội bộ, dữ liệu khách hàng, token hay mật khẩu.

## App xử lý dữ liệu thế nào

- **Phím gõ:** HVN Key đọc phím qua quyền Trợ năng (Accessibility) để đổi thành chữ tiếng Việt. Phím và chữ được xử
  lý ngay trên máy, không lưu và không gửi đi đâu. Trong ô mật khẩu, HVN Key để phím đi qua nguyên vẹn.
- **Địa chỉ trang web:** chỉ khi bạn bật **Nhớ theo trang web**, HVN Key đọc địa chỉ tab đang mở của trình duyệt (qua
  quyền Apple Events) để nhớ tiếng Anh hay tiếng Việt cho từng trang. Địa chỉ chỉ lưu trên máy.
- **Nhật ký gõ:** tắt mặc định. Khi bật ở menu **Gỡ lỗi**, nhật ký nằm ở
  `~/Library/Application Support/HVN Key/typing-log.jsonl` trên máy bạn, không ghi trong ô mật khẩu, trình quản lý
  mật khẩu hay Terminal.
- **Kết nối mạng:** HVN Key chỉ kết nối tới GitHub (`github.com` và máy chủ tải file của GitHub) để kiểm tra và tải
  bản cập nhật từ repo này. Bạn tắt được việc này ở **Mở HVN Key… › Chung › Tự động cập nhật**. App không gửi báo
  cáo lỗi hay số liệu sử dụng về máy chủ nào.
- **Cập nhật:** dùng Sparkle; mỗi bản cập nhật được ký EdDSA bằng khoá riêng của HVN GROUP, app kiểm chữ ký trước khi
  cài. Bản cài đặt được ký Developer ID của HVN GROUP và notarize bởi Apple.

## Phiên bản được hỗ trợ

Chỉ bản phát hành mới nhất được vá lỗi.

---

HVN GROUP · hvn.vn
