# VWW Invitation Manager

WordPress plugin quản lý đăng ký, vé mời, email, QR và check-in cho Vietnam Wedding Week.

## Current release candidate

- Version: **1.21.0**
- Branch: `release/v1.21.0`
- Package: `releases/vww-invitation-manager-v1.21.0.zip`

## v1.21.0 highlights

- Staff Check-in Center frontend cho role Nhân viên Check-in VWW.
- Camera mặc định tắt, scanner local và Check-in gần nhất.
- Danh sách khách có search, filter, selection, bulk cơ bản và lọc ngày check-in.
- Export Excel Staff/Admin theo direct POST download, hỗ trợ chọn field và phạm vi dữ liệu.
- Admin Export và Staff Export dùng cùng hướng xử lý cốt lõi.
- QR được tạo local, không gửi ticket token tới dịch vụ QR bên ngoài.
- Siết permission: Editor không tự động có quyền VWW.
- CF7 ticket creation chạy server-side sau submission hợp lệ; không còn public REST ticket-creation flow riêng.
- Duplicate registration không trả lại URL/token vé cũ.
- Email queue có retry cơ bản.
- Bổ sung database indexes cho status/date/check-in và chuẩn hóa timezone attribution.

## Release policy

`main` là mốc ổn định. Mỗi bản nâng cấp lớn được phát triển trên branch `release/vX.Y.Z` và review bằng Pull Request trước khi nhập vào `main`.

## Notes

Repository này hiện đang ở chế độ **public**. Không commit API keys, SMTP credentials, access tokens, dữ liệu khách hoặc file export thực tế vào repository.
