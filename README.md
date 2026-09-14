# Ngôi Nhà Số — Family Core Foundation V5

Nền tảng điều phối gia đình và quản trị ngôi nhà. Core hoạt động không cần thiết bị; cảm biến, năng lượng và tự động hóa là module tùy chọn.

## Foundation V5

- Dashboard Hôm nay: việc mở, lịch 7 ngày và tình trạng hồ sơ nhà
- Gia đình: hồ sơ hộ, thành viên, lịch chung và danh sách mua sắm
- Ngôi nhà: phòng, tài sản và ngày bảo trì tiếp theo
- Thư viện: giữ nguyên 28 công cụ thực dụng
- Module tùy chọn: Chăm sóc, An toàn, Năng lượng và Tự động hóa
- Migration an toàn từ dữ liệu V4 sang V5
- Sao lưu/khôi phục JSON và phát hiện xung đột giữa các tab

## Tài liệu Giai đoạn 1

- [SWOT đối thủ và lựa chọn Core MVP](docs/phase-1-swot.md)
- [Product Foundation V5](docs/phase-1-product-foundation.md)

## Trạng thái dữ liệu

Foundation hiện dùng localStorage để kiểm chứng luồng sản phẩm và giữ khả năng chạy ngoại tuyến. Bước backend tiếp theo sẽ bổ sung tài khoản hộ gia đình, đồng bộ nhiều thiết bị và phân quyền bằng Supabase Row Level Security.

Website production hiện tại: https://meicarevn.github.io/ngoi-nha-so/

Nhánh đang kiểm thử: `build/phase-1-core`
