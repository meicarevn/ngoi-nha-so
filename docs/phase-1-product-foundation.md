# Giai đoạn 1 — Product Foundation V5

## Product thesis

Ngôi Nhà Số là hệ điều hành nhẹ cho gia đình Việt. Core hoạt động đầy đủ khi không có thiết bị. Mỗi module tùy chọn chỉ được phép:

1. Đọc ngữ cảnh từ Home Graph.
2. Phát sinh event/cảnh báo.
3. Tạo hoặc cập nhật task.
4. Không phá vỡ trải nghiệm Core khi module bị tắt.

## Home Graph tối thiểu

- Household: tên hộ, múi giờ, thiết lập.
- Member: tên, vai trò, màu, trạng thái.
- Room: tên phòng, loại phòng.
- Asset: tài sản/thiết bị, phòng, ngày mua, hạn bảo hành, chu kỳ bảo trì.
- Task: nội dung, người phụ trách, hạn, mức ưu tiên, trạng thái.
- Event: lịch chung hoặc sự kiện do module phát sinh.
- List: danh sách mua sắm/chung.
- Module: trạng thái bật/tắt và quyền truy cập.

## Nguyên tắc UX

- Màn hình Hôm nay trả lời trong 5 giây: “Hôm nay nhà mình cần làm gì?”
- Một hành động chính trên mỗi khu vực.
- Thiết lập ban đầu dưới 3 phút; không bắt khai báo đầy đủ hồ sơ.
- Progressive disclosure: chỉ hiện module đã bật.
- Mọi dữ liệu quan trọng đều có người phụ trách, thời hạn hoặc ngữ cảnh phòng/tài sản.
- Mobile-first; tablet mode là màn hình dùng chung, dữ liệu riêng tư được che mặc định.

## Phạm vi bản Foundation hiện tại

- Nâng schema dữ liệu cục bộ từ V4 lên V5 nhưng giữ dữ liệu cũ.
- Thêm Household, Members, Calendar, Shopping, Rooms và Assets.
- Tái cấu trúc điều hướng thành Hôm nay / Gia đình / Ngôi nhà / Công cụ / Cài đặt.
- Giữ nguyên thư viện 28 công cụ.
- Đưa các module IoT vào trạng thái “tùy chọn/sắp ra mắt”, chưa yêu cầu thiết bị.

## Definition of Done cho Giai đoạn 1

- Người dùng tạo được hồ sơ hộ gia đình.
- Thêm/xóa được thành viên.
- Tạo được sự kiện chung và danh sách mua sắm.
- Tạo được phòng, tài sản và ngày bảo trì.
- Dashboard hiển thị việc hôm nay và sự kiện sắp tới.
- Dữ liệu V4 được đọc/migrate an toàn.
- Chức năng sao lưu/khôi phục vẫn hoạt động.
- Giao diện dùng được trên desktop, tablet và mobile.

## Cổng chuyển sang backend

Bản Foundation dùng localStorage để xác thực luồng nghiệp vụ. Chỉ chuyển sang Supabase khi các luồng lõi đã được kiểm thử. Schema backend tương lai phải có household_id trên mọi bảng dùng chung và Row Level Security để cô lập từng hộ.
