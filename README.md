# HVN Key — bản phát hành

HVN Key là bộ gõ tiếng Việt cho máy Mac chip Apple. Bạn gõ Telex như bình thường; khi gõ một từ tiếng Anh lúc đang ở
chế độ tiếng Việt (hoặc ngược lại), HVN Key tự sửa từ đó và tự chuyển ngôn ngữ cho bạn.

Repo này chỉ chứa bản phát hành và kênh cập nhật của ứng dụng. Mã nguồn được quản lý riêng tại HVN GROUP; gói mã
nguồn của từng phiên bản được đính kèm trong chính bản phát hành đó (xem mục **Giấy phép**).

## Tải về

Tải bản mới nhất tại **[Releases › Latest](https://github.com/hvngroup/app-hvn-key-releases/releases/latest)**.

| Máy | File |
|---|---|
| Mac chip Apple (M1 trở lên), macOS 13 Ventura trở lên | `HVNKey.dmg` |

- Mỗi file có một file `.sha256` đi kèm để kiểm tra file tải về còn nguyên vẹn:
  `shasum -a 256 -c HVNKey.dmg.sha256`.
- `HVNKey.zip` và `appcast.xml` dành cho trình cập nhật trong app. Bạn không cần tải hai file này.
- `HVNKey-<phiên bản>-source.tar.gz` là mã nguồn tương ứng với bản phát hành đó.
- HVN Key không chạy trên Mac dùng chip Intel.

## Cài đặt

1. Mở `HVNKey.dmg`, kéo **HVN Key** vào thư mục **Applications**.
2. Mở **HVN Key** từ **Applications**. Bản phát hành được ký Developer ID của HVN GROUP và đã được Apple kiểm tra
   (notarize), nên macOS mở bình thường.
3. Làm theo màn hình hướng dẫn: bấm **Mở Cài đặt hệ thống**, bật **HVN Key** trong **Quyền riêng tư & Bảo mật ›
   Trợ năng**, rồi quay lại app. HVN Key cần quyền này để đổi phím bạn gõ thành chữ tiếng Việt; mọi xử lý diễn ra
   ngay trên máy.
4. Nếu bật **Nhớ theo trang web**, macOS hỏi thêm quyền điều khiển trình duyệt để HVN Key đọc địa chỉ tab đang mở.
   Địa chỉ này chỉ dùng trên máy bạn.

Nếu máy đang cài một bộ gõ khác (Vikey, OpenKey, EVKey, Unikey…), hãy tắt bộ gõ đó để hai bộ gõ không cùng xử lý
phím.

## Cập nhật

HVN Key tự kiểm tra bản mới mỗi ngày từ repo này, tải về và cài khi bạn thoát app hoặc tắt máy. Bạn có thể tắt tự động
cập nhật ở **Mở HVN Key… › Chung › Tự động cập nhật**, hoặc kiểm tra thủ công bằng **Kiểm tra cập nhật…** trên menu.
Mọi bản cập nhật đều được ký bằng khoá riêng của HVN GROUP; app từ chối bản cập nhật không đúng chữ ký.

## Báo lỗi và hỗ trợ

- Báo lỗi hoặc góp ý: [mở issue mới](https://github.com/hvngroup/app-hvn-key-releases/issues/new/choose). Ghi lại
  phím bạn đã gõ, chữ hiện ra, chữ bạn mong muốn và phiên bản app (menu **Giới thiệu HVN Key**).
- Nếu app bị thoát đột ngột, đính kèm báo cáo lỗi trong `~/Library/Logs/DiagnosticReports` (file bắt đầu bằng
  `HVNKey`). Báo cáo không chứa chữ bạn đã gõ.
- Lỗ hổng bảo mật: gửi riêng qua
  [Security Advisories](https://github.com/hvngroup/app-hvn-key-releases/security/advisories/new), không mở issue
  công khai.
- Hỗ trợ kỹ thuật: kythuat@hvn.vn · Hotline 024.9999.7777.

## Giấy phép

HVN Key là phần mềm tự do theo giấy phép [GNU GPL-3.0](LICENSE): bạn được dùng, sao chép, sửa đổi và phân phối lại,
với điều kiện bản phân phối lại cũng theo GPL-3.0 và kèm mã nguồn. HVN Key dựa trên
[Vikey](https://github.com/tonyminibot/Vikey) của Tony Dinh và [OpenKey](https://github.com/tuyenvm/OpenKey) của
Tuyen Mai.

---

HVN GROUP · [hvn.vn](https://hvn.vn)
