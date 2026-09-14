# Giai đoạn 1 — SWOT đối thủ và lựa chọn Core MVP

Cập nhật: 14/09/2026

## Kết luận chiến lược

Ngôi Nhà Số không cạnh tranh bằng việc có nhiều công cụ hơn. Nền tảng phải sở hữu **dòng công việc gia đình khép kín**: ghi nhận → giao người phụ trách → nhắc → hoàn thành → lưu vào hồ sơ ngôi nhà. Thiết bị thông minh chỉ phát sinh sự kiện cho dòng công việc này.

## Bản đồ đối thủ

| Nhóm | Đại diện | Điểm mạnh | Điểm yếu/khoảng trống | Phản ứng của Ngôi Nhà Số |
|---|---|---|---|---|
| Điều phối gia đình toàn cầu | Cozi, FamilyWall | Lịch chung, việc, mua sắm, mô hình freemium đã được xác thực | Bản địa hóa Việt Nam hạn chế; hồ sơ nhà và luồng xử lý sự cố chưa phải trọng tâm | Làm lịch/việc/danh sách thật gọn; khác biệt bằng hồ sơ nhà và hành động |
| Ứng dụng gia đình Việt | MyFamily, Fami | Tiếng Việt, lịch/chi tiêu/gia đình phù hợp văn hóa | Dễ trùng lặp tính năng; khó tạo lợi thế chỉ bằng lịch và chi tiêu | Không định vị như ứng dụng lịch hoặc sổ thu chi |
| Nền tảng hệ sinh thái lớn | Google Home, Apple Home, SmartThings | Thiết bị, tài khoản hộ, automation và hệ sinh thái toàn cầu | Tập trung điều khiển thiết bị; ít nghiệp vụ gia đình Việt | Đứng trên lớp đời sống; tích hợp thay vì đối đầu |
| Smart-home Việt Nam | Lumi, Vconnex, Rạng Đông, FPT Smart Home | Phần cứng, lắp đặt, đại lý, dịch vụ sau bán hàng | Đầu tư ban đầu và phụ thuộc hệ sinh thái; quản trị đời sống không phải lõi | Hardware-optional, đa hãng, không yêu cầu lắp đặt |
| Local-first/DIY | Home Assistant | Riêng tư, chạy cục bộ, nhiều tích hợp | Khó tiếp cận hộ phổ thông, cần kỹ thuật | Trải nghiệm đơn giản như sản phẩm tiêu dùng; local-first cho module IoT |
| Trợ lý AI tương lai | Gemini for Home và các trợ lý hệ điều hành | Hội thoại, tóm tắt, automation bằng ngôn ngữ tự nhiên | Phụ thuộc dữ liệu/hệ sinh thái; khó sở hữu ngữ cảnh gia đình Việt nếu dữ liệu phân tán | Xây Home Graph và dữ liệu có cấu trúc trước; AI là lớp hỗ trợ sau |

Nguồn chính: [Cozi](https://www.cozi.com/compare-plans/), [FamilyWall](https://www.familywall.com/premium.html), [MyFamily](https://www.myfamily.vn/), [Google Home](https://home.google.com/about-google-home/), [Apple Home](https://www.apple.com/home-app/), [Home Assistant](https://www.home-assistant.io/), [Lumi](https://lumi.vn/), [Vconnex](https://vconnex.vn/).

## SWOT của Ngôi Nhà Số

### Strengths — Điểm mạnh

- Tài sản ban đầu gồm 28 công cụ có thể dùng ngay và làm kênh thu hút người dùng.
- Giao diện web/PWA phù hợp điện thoại, máy tính và máy tính bảng cũ.
- Có khả năng phát triển cả phần mềm lẫn cơ điện tử/IoT.
- Có thể thiết kế riêng cho hộ gia đình Việt: lịch âm, gia đình nhiều thế hệ, nhà phố/căn hộ, ngôn ngữ dễ dùng.
- Không bị khóa vào phần cứng hoặc hệ sinh thái thiết bị từ đầu.

### Weaknesses — Điểm yếu

- Phiên bản 4.1 lưu cục bộ, chưa có tài khoản hộ gia đình, thành viên, đồng bộ và phân quyền.
- 28 công cụ đang rời rạc; kết quả chưa hội tụ thành hồ sơ hoặc dòng công việc.
- Chưa có lịch chung, danh sách mua sắm chung và mô hình tài sản/bảo trì.
- Chưa có dữ liệu sử dụng thực tế để chứng minh tiện ích nào tạo thói quen.
- Nguồn lực nhỏ hơn các hãng hệ sinh thái và ứng dụng quốc tế.

### Opportunities — Cơ hội

- Hộ gia đình cần một nơi chung để phối hợp, không nhất thiết mua phần cứng.
- Khoảng trống giữa “ứng dụng lịch/việc” và “ứng dụng điều khiển thiết bị”.
- Thiết bị Matter và API đa hãng giúp giảm chi phí tự xây hệ sinh thái.
- Máy tính bảng cũ có thể trở thành bảng điều hành đặt tại bếp/phòng khách.
- Dữ liệu Home Graph cho phép mở rộng sang bảo trì, chăm sóc, năng lượng và AI.

### Threats — Thách thức

- Google, Apple hoặc các ứng dụng AI có thể bổ sung nhanh tính năng gia đình.
- Người dùng không muốn nhập dữ liệu lặp lại hoặc cài thêm một ứng dụng.
- Super-app nhiều tính năng dễ gây quá tải, tỷ lệ quay lại thấp.
- Dữ liệu gia đình nhạy cảm; một sự cố bảo mật có thể phá hủy niềm tin.
- Tích hợp thiết bị đa hãng dễ phát sinh lỗi và chi phí hỗ trợ.

## Tiện ích Core được chọn

Áp dụng bốn tiêu chí: phổ quát, dùng lặp lại, tạo phối hợp nhiều người và không cần phần cứng.

1. **Hôm nay:** việc, lịch, nhắc và cảnh báo cần xử lý.
2. **Gia đình:** thành viên, vai trò, lịch chung, danh sách mua sắm.
3. **Ngôi nhà:** phòng, tài sản, bảo hành, bảo trì và sự cố.
4. **Thư viện:** giữ 28 công cụ nhưng chuyển thành lớp tiện ích, không phải màn hình chính.
5. **Cài đặt & dữ liệu:** riêng tư, sao lưu, sau này là đồng bộ và phân quyền.

## Những thứ không đưa vào Core MVP

- Camera, khóa, công tắc và tự động hóa thiết bị.
- Chat/mạng xã hội gia đình.
- Theo dõi vị trí thời gian thực.
- Kết nối ngân hàng.
- AI tạo nội dung chung chung.
- Marketplace dịch vụ.
- Tự phát triển đầu báo cháy/khí gas.

## Rủi ro cần kiểm chứng trong pilot

- Gia đình có cùng mở một không gian chung hay chỉ một người dùng?
- Người dùng quay lại vì “Hôm nay”, lịch chung hay danh sách mua sắm?
- Hồ sơ tài sản/bảo trì có đủ giá trị để tạo khác biệt không?
- Bao nhiêu thao tác nhập liệu là quá nhiều?
- Gia đình sẵn sàng trả tiền cho đồng bộ, lịch sử và nhắc nâng cao hay không?
