# TRƯỜNG ĐẠI HỌC ĐIỆN LỰC

## KHOA CÔNG NGHỆ THÔNG TIN



# BÁO CÁO CHUYÊN ĐỀ HỌC PHẦN

## MÔN CÔNG NGHỆ PHẦN MỀM

### ĐỀ TÀI: QUẢN LÝ MUA BÁN XE Ô TÔ



- Sinh viên thực hiện: BÙI XUÂN SƠN
- Giảng viên hướng dẫn: ThS. NGUYỄN THỊ TRANG LINH
- Ngành: CÔNG NGHỆ THÔNG TIN
- Chuyên ngành: CÔNG NGHỆ PHẦN MỀM
- Lớp: D15CNPM5
- Khóa: D15



Hà Nội, tháng …

---

## Mô tả tóm tắt đề tài

Xây dựng “Hệ thống phần mềm quản lý mua bán xe ô tô” cho một đại lý/showroom, với các chức năng chính giữ nguyên như bản gốc:

- Đăng nhập
- Quản lý nhân viên
- Quản lý nhà cung cấp (hãng xe/đối tác)
- Quản lý hóa đơn
- Quản lý sản phẩm (xe)
- Báo cáo thống kê

Phạm vi mở rộng theo miền ô tô: quản lý tồn kho theo VIN, quy trình báo giá–hợp đồng–hóa đơn–thanh toán, quy trình giao xe (PDI, đăng ký biển số, bảo hiểm), báo cáo doanh số và tồn kho.

### 1. Nội dung thực hiện

- Chương 1: Giới thiệu dự án phần mềm.
- Chương 2: Quản lý dự án.
- Chương 3: Phân tích hệ thống.
- Chương 4: Thiết kế.
- Chương 5: Lập trình.
- Chương 6: Kiểm thử phần mềm.
- Chương 7: Đóng gói và bảo trì phần mềm.

### 2. Kết quả đạt được

- Hoàn thành đề cương chuyên đề học phần môn: “Công nghệ phần mềm”.
- Xây dựng hệ thống mẫu phù hợp với quy trình mua bán ô tô, đáp ứng các chức năng cốt lõi và dễ sử dụng cho quản lý lẫn nhân viên.



Hà Nội, ngày … tháng … năm 2022

Giảng viên hướng dẫn (ký và ghi rõ họ tên)

Sinh viên thực hiện (ký và ghi rõ họ tên)

---

## PHIẾU CHẤM ĐIỂM

| STT | Họ và tên sinh viên | Nội dung thực hiện                                 | Điểm | Chữ ký |
|-----|----------------------|----------------------------------------------------|------|--------|
| 1   | Bùi Xuân Sơn         | Phần đầu, Chương 1, Chương 2, Chương 3.           |      |        |
| 2   |                      | Chương 4, Chương 5.                               |      |        |
| 3   |                      | Chương 6, Chương 7, Kết luận, Tài liệu tham khảo |      |        |



Họ và tên giảng viên: ………………………………………  |  Chữ ký: ………………………………………  |  Ghi chú: ………………………………………

Giảng viên chấm 1: ………………………………………………………………………………………………………

Giảng viên chấm 2: ………………………………………………………………………………………………………

---

## MỤC LỤC

- Lời nói đầu
- Chương 1: Giới thiệu dự án phần mềm
- Chương 2: Quản lý dự án
- Chương 3: Phân tích thiết kế hệ thống
- Chương 4: Thiết kế
- Chương 5: Lập trình
- Chương 6: Kiểm thử phần mềm
- Chương 7: Đóng gói và bảo trì phần mềm
- Kết luận
- Hướng phát triển
- Tài liệu tham khảo

---

# LỜI NÓI ĐẦU

Thị trường ô tô Việt Nam phát triển mạnh, đa dạng mẫu mã – phiên bản – chính sách bán hàng, kèm các dịch vụ tài chính, bảo hiểm, đăng ký, bảo dưỡng. Nhiều đại lý vẫn quản lý bằng sổ sách hoặc các file rời, khó theo dõi tồn kho theo VIN, khó kiểm soát quy trình giao xe và doanh số theo từng tư vấn bán hàng.

Từ kiến thức môn Phân tích & Thiết kế hệ thống và Công nghệ phần mềm, em thực hiện đề tài “Quản lý mua bán xe ô tô” nhằm tin học hóa các nghiệp vụ cốt lõi: quản lý xe (sản phẩm), quản lý khách hàng – báo giá – hợp đồng – hóa đơn – thanh toán, quản lý nhà cung cấp/đối tác, quản lý nhân viên, báo cáo thống kê và quy trình giao xe.

Do thời gian hạn chế và kinh nghiệm thực tế còn ít, báo cáo khó tránh khỏi thiếu sót. Kính mong cô và các thầy cô góp ý để hoàn thiện hơn. Em xin chân thành cảm ơn!

---

# CHƯƠNG 1: GIỚI THIỆU DỰ ÁN PHẦN MỀM

## 1.1 Khảo sát hiện trạng

Công tác quản lý tại nhiều đại lý ô tô còn thủ công, phân tán: quản lý tồn kho xe theo VIN/màu/phiên bản, quản lý báo giá – hợp đồng – tiến độ thanh toán, phối hợp đăng ký biển số, bảo hiểm, PDI và lịch bàn giao xe. Điều này tốn thời gian, dễ sai sót, ảnh hưởng hiệu quả kinh doanh.

### 1.1.1 Tổng quan

- Tên đơn vị: Showroom/Đại lý Ô tô Kim Tiền
- Nhân sự: ~20 người (quản lý, tư vấn bán hàng, kho/giao xe, kế toán…)
- Thời gian làm việc: 8h00 – 18h00 (Thứ 2 – Chủ nhật)
- Doanh thu tháng tham chiếu: ~10.000.000.000 VNĐ
- Địa chỉ: 206 Kim Mã, Phường Kim Mã, Quận Ba Đình, Hà Nội
- Hotline: 09xx xxx xxx
- Hình thức kinh doanh: Bán xe ô tô mới, phụ kiện; dịch vụ tài chính – bảo hiểm – đăng kiểm; (tuỳ chọn) thu xe cũ đổi xe mới.

Hình 1.2: Showroom Ô tô Kim Tiền.

## 1.2 Xác định bài toán cần giải quyết

- Chuẩn hoá và số hoá toàn bộ quy trình mua bán ô tô tại đại lý.
- Theo dõi tồn kho theo VIN/màu/phiên bản; quản lý báo giá – hợp đồng – công nợ – hóa đơn.
- Quản lý đối tác: hãng xe, ngân hàng, bảo hiểm, đăng kiểm.
- Theo dõi quy trình giao xe (PDI, đăng ký, bảo hiểm, lịch bàn giao) và báo cáo.

## 1.3 Phân tích và đặc tả các hoạt động nghiệp vụ của hệ thống

### 1.3.1 Quy trình nhập xe (nhập kho)

- Cuối ngày/tuần, bộ phận bán hàng/kho đối chiếu nhu cầu – đặt cọc để đề xuất nhập xe.
- Quản lý đặt xe với hãng/nhà phân phối.
- Xe về đại lý: kiểm tra chứng từ, đối chiếu VIN, PDI; đạt yêu cầu thì nhập kho và cập nhật trạng thái.

Hàng đạt tiêu chuẩn:

- Xe: VIN trùng khớp, ngoại hình nguyên vẹn, hồ sơ hợp lệ.

Giá nhập kho = Σ đơn giá xe (+ chi phí liên quan nếu có).

### 1.3.2 Quy trình bán hàng

- Tư vấn nhu cầu, lái thử; lập báo giá theo model/phiên bản/màu và gói tài chính/bảo hiểm.
- Đặt cọc/giữ xe theo VIN; lập hợp đồng; thu tiền theo tiến độ; hoàn tất hồ sơ đăng ký.
- Bàn giao: nghiệm thu, xuất hóa đơn, cập nhật xe “đã bán”.

### 1.3.3 Quản lý nhân viên

- Cơ cấu tham chiếu: 1 quản lý, 8 tư vấn bán hàng, 4 kho/giao xe, 2 kế toán, 1 quản trị hệ thống…
- Chấm công theo ca/ngày; lương cơ bản + thưởng doanh số/đánh giá hiệu suất.
- Chính sách nghỉ phép, kỷ luật… quản lý trên hệ thống.

### 1.3.4 Báo cáo thống kê

- Doanh số theo thời gian/nhân viên/sản phẩm; tồn kho theo VIN; vòng quay tồn kho; lợi nhuận gộp.

Doanh thu = ∑ Tiền bán – ∑ Tiền nhập/chi phí.

## 1.4 Xác định yêu cầu của hệ thống

### 1.4.1 Yêu cầu chức năng (giữ nguyên)

- Đăng nhập.
- Quản lý nhân viên.
- Quản lý nhà cung cấp/đối tác.
- Quản lý hóa đơn.
- Quản lý sản phẩm (xe).
- Báo cáo thống kê.

### 1.4.2 Yêu cầu phi chức năng

#### 1.4.2.1 Yêu cầu hiệu năng

- Tra cứu nhanh theo VIN/model, phản hồi kịp thời.

#### 1.4.2.2 Khả năng tương tác

- Giao diện phù hợp quy trình bán hàng, dễ sử dụng.

#### 1.4.2.3 Tính năng sử dụng

- Đủ chức năng cơ bản, hỗ trợ tìm kiếm, lọc, xuất báo cáo.

#### 1.4.2.4 Ràng buộc thiết kế

- Kiến trúc đơn giản, dữ liệu chuẩn hoá; theo dõi trạng thái theo VIN.

---

# CHƯƠNG 2: QUẢN LÝ DỰ ÁN

## 2.1 Ước lượng dự án

### 2.1.1 Ước lượng chi phí

Giai đoạn | Công việc | Mô tả | Chi phí
---|---|---|---
Quản lý dự án | Khảo sát yêu cầu | Thu thập yêu cầu tổng quan | 500.000–1.000.000 VND
Quản lý dự án | Khởi tạo dự án | Thông báo triển khai, lập project charter | 2.000.000–2.500.000 VND
Quản lý dự án | Kế hoạch phạm vi | Lập kế hoạch phạm vi | 2.000.000–2.500.000 VND
Quản lý dự án | Báo cáo tổng kết | Tổng kết toàn bộ công việc | 0
Quản lý dự án | Rút kinh nghiệm | Bài học kinh nghiệm | 0
Phân tích & thiết kế | Đặc tả yêu cầu | Mô tả cụ thể yêu cầu | 2.000.000–2.500.000 VND
Phân tích & thiết kế | UML | Use case, trình tự, hoạt động | 2.000.000–2.500.000 VND
Phân tích & thiết kế | Thiết kế CSDL | Bảng xe, khách hàng, hợp đồng, hóa đơn… | 5.000.000–6.500.000 VND
Phân tích & thiết kế | Thiết kế giao diện | Form đăng nhập, xe, hợp đồng, báo cáo | 5.000.000–6.500.000 VND
Phân tích & thiết kế | Báo cáo phân tích | Hoàn chỉnh tài liệu | 500.000–1.000.000 VND
Module bán hàng | Phân tích yêu cầu | Báo giá–hợp đồng–hóa đơn | 500.000–1.000.000 VND
Module bán hàng | Thiết kế module | Form đăng nhập, hợp đồng/hóa đơn | 5.000.000–6.500.000 VND
Module bán hàng | Code module | Luồng báo giá–hợp đồng–thanh toán | 10.000.000–13.000.000 VND
Module bán hàng | Cài đặt | Chạy thử module | 0
Module bán hàng | Kiểm thử module | Giao diện, nghiệp vụ, dữ liệu | 2.000.000–2.500.000 VND
Module bán hàng | Báo cáo module | Mô tả chi tiết | 0
Tích hợp | Tích hợp hệ thống | Lắp ráp module | 2.000.000–2.500.000 VND
Tích hợp | Kiểm thử tích hợp | Test tổng quan | 2.000.000–2.500.000 VND
Tích hợp | Fix lỗi | Sửa lỗi phát sinh | 4.000.000–5.500.000 VND
Chuyển giao | Hướng dẫn sử dụng | Tài liệu người dùng | 0
Chuyển giao | Kế hoạch bảo trì | Bàn giao & kế hoạch | 0
Kết thúc | Tổng kết dự án | Tổng kết & bàn giao | 0

> Bảng 2.1.1 Ước lượng chi phí

### 2.1.2 Ước lượng thời gian

Giai đoạn | Công việc | Mô tả | Thời gian
---|---|---|---
Quản lý dự án | Khảo sát yêu cầu | Thu thập yêu cầu | 1 ngày
Quản lý dự án | Khởi tạo dự án | Project charter | 1 ngày
Quản lý dự án | Kế hoạch phạm vi | Lập kế hoạch | 5 ngày
Quản lý dự án | Báo cáo tổng kết | Cuối dự án | Cuối dự án
Quản lý dự án | Rút kinh nghiệm | Cuối dự án | Cuối dự án
Phân tích & thiết kế | Đặc tả yêu cầu | Mô tả chi tiết | 2 ngày
Phân tích & thiết kế | UML | Use case, trình tự, hoạt động | 5 ngày
Phân tích & thiết kế | Thiết kế CSDL | Cấu trúc dữ liệu | 3 ngày
Phân tích & thiết kế | Thiết kế giao diện | Form cốt lõi | 4 ngày
Phân tích & thiết kế | Báo cáo phân tích | Hoàn chỉnh | 2 ngày
Module bán hàng | Phân tích yêu cầu | Kế hoạch chi tiết | 2 ngày
Module bán hàng | Thiết kế | Đăng nhập; hợp đồng; hóa đơn | 3 ngày
Module bán hàng | Lập trình | Báo giá–hợp đồng–thanh toán | 5 ngày
Module bán hàng | Cài đặt | Chạy thử | 1 ngày
Module bán hàng | Kiểm thử | Giao diện & dữ liệu | 3 ngày
Module bán hàng | Báo cáo | Mô tả module | 1 ngày
Tích hợp | Tích hợp | Lắp ráp module | 1 ngày
Tích hợp | Kiểm thử tích hợp | Test tổng quan | 1 ngày
Tích hợp | Fix lỗi | Sửa lỗi | 2 ngày
Chuyển giao | Hướng dẫn | Soạn tài liệu | 1 ngày
Chuyển giao | Kế hoạch bảo trì | Bàn giao | 1 ngày
Kết thúc | Tổng kết dự án | Tổng kết | 1 ngày

> Bảng 2.1.2 Ước lượng thời gian

### 2.1.3 Ước lượng người tham gia

- Số lượng: 3 người (1 PM/BA, 1 Dev fullstack, 1 Tester)

> Bảng 2.1.3 Ước lượng người tham gia

## 2.2 Lập lịch và theo dõi

WBS (rút gọn) giữ nguyên cấu trúc bản gốc, điều chỉnh theo miền ô tô.

---

# CHƯƠNG 3: PHÂN TÍCH THIẾT KẾ HỆ THỐNG

## 3.1 Các tác nhân chính tham gia hệ thống

### 3.1.1 Khách hàng

- Người mua xe; nhận báo giá, ký hợp đồng, thanh toán, nhận hóa đơn và bàn giao xe; được hỗ trợ đăng ký biển số, bảo hiểm, phụ kiện.

### 3.1.2 Nhân viên bán hàng

- Tư vấn model/phiên bản/màu, lập báo giá, tạo hợp đồng/đặt cọc, cập nhật tiến độ, phối hợp giao xe đúng hẹn.

### 3.1.3 Người quản lý

- Nắm tình hình doanh số, tồn kho theo VIN, quản lý nhân viên, nhà cung cấp/đối tác, báo cáo định kỳ.

## 3.2 Các use case chính tham gia hệ thống

- Nhân viên bán hàng:
  - Quản lý hóa đơn (bán xe)
- Quản lý:
  - Quản lý nhân viên
  - Quản lý sản phẩm (xe)
  - Quản lý nhà cung cấp/đối tác
  - Thống kê

## 3.3 Sơ đồ tổng quan các chức năng chính (mô tả văn bản)

### 3.3.1 Use case tổng quát

- Phạm vi: đăng nhập, quản lý danh mục (nhân viên, xe, nhà cung cấp), hóa đơn, báo cáo.

### 3.3.2 Đăng nhập

#### Đặc tả use case đăng nhập

- Tác nhân: Quản lý, Nhân viên bán hàng, Kế toán, Kho
- Mô tả: Đăng nhập để sử dụng chức năng theo vai trò; đăng xuất khi kết thúc.
- Dòng sự kiện chính: mở giao diện -> nhập tên/mật khẩu -> kiểm tra -> thành công vào hệ thống/chưa thành công thì nhập lại.

### 3.3.3 Quản lý nhân viên

#### Đặc tả use case quản lý nhân viên

- Tác nhân: Quản lý
- Mô tả: Thêm/Sửa/Xoá/Làm mới; thông tin: mã NV, tên, ngày sinh, giới tính, địa chỉ, số điện thoại, chức vụ.

### 3.3.4 Quản lý nhà cung cấp/đối tác

#### Đặc tả use case quản lý nhà cung cấp/đối tác

- Tác nhân: Quản lý
- Mô tả: Quản lý hãng xe, ngân hàng, bảo hiểm, đăng kiểm; thông tin: mã, tên, địa chỉ, số điện thoại, loại đối tác.

### 3.3.5 Quản lý hóa đơn (bán xe)

#### Đặc tả use case quản lý hóa đơn

- Tác nhân: Nhân viên bán hàng, Kế toán
- Mô tả: Lập báo giá -> hợp đồng/đặt cọc -> hóa đơn -> thanh toán -> bàn giao; lưu CSDL và cập nhật trạng thái xe.

### 3.3.6 Quản lý sản phẩm (xe)

#### Đặc tả use case quản lý xe

- Tác nhân: Quản lý, Kho
- Mô tả: Quản lý model/phiên bản/màu/VIN/giá/trạng thái; Thêm/Sửa/Xoá, tìm kiếm theo VIN.

### 3.3.7 Báo cáo thống kê

#### Đặc tả use case báo cáo

- Tác nhân: Quản lý
- Mô tả: Doanh số theo thời gian/nhân viên/sản phẩm; tồn kho theo VIN; xuất báo cáo.

---

# CHƯƠNG 4: THIẾT KẾ

## 4.1 Thiết kế giao diện

### 4.1.1 Giao diện đăng nhập

- Kiểm tra tên đăng nhập/mật khẩu; đúng vào trang chủ, sai thông báo.

### 4.1.2 Giao diện hệ thống (trang chủ)

- Menu: Nhân viên, Xe (sản phẩm), Nhà cung cấp/Đối tác, Hóa đơn, Báo cáo, Đăng xuất.

### 4.1.3 Giao diện quản lý

#### 4.1.3.1 Quản lý nhân viên

- Thêm/Sửa/Xoá/Làm mới; hiển thị danh sách.

#### 4.1.3.2 Quản lý xe (sản phẩm)

- Thêm xe với các thông tin: mã xe, model, phiên bản, màu, VIN, giá, mô tả, mã nhà cung cấp, trạng thái (còn hàng/giữ chỗ/đã bán/đang bàn giao); Sửa/Xoá/Làm mới.

#### 4.1.3.3 Quản lý nhà cung cấp/đối tác

- Hãng xe, ngân hàng, bảo hiểm, đăng kiểm; Thêm/Sửa/Xoá/Làm mới.

#### 4.1.3.4 Quản lý hóa đơn

- Lập hóa đơn bán xe, liên kết hợp đồng/đặt cọc; Sửa/Xoá; in/xuất file.

#### 4.1.3.5 Báo cáo thống kê

- Chọn mốc thời gian -> xem doanh số, tồn kho, lợi nhuận; xuất báo cáo.

## 4.2 Thiết kế lưu trữ

### 4.2.1 Bảng đăng nhập (Users)

- MaUser, Username, PasswordHash, Role, TrangThai, CreatedAt

### 4.2.2 Bảng nhân viên (NhanVien)

- MaNV, HoTen, NgaySinh, GioiTinh, DiaChi, DienThoai, ChucVu, TrangThai

### 4.2.3 Bảng xe (SanPhamXe)

- MaXe, Model, PhienBan, Mau, VIN, Gia, MoTa, MaNCC, TrangThai

### 4.2.4 Bảng nhà cung cấp/đối tác (NhaCungCap)

- MaNCC, TenNCC, DiaChi, DienThoai, LoaiDoiTac (HangXe/NgNganHang/BaoHiem/DangKiem)

### 4.2.5 Bảng hóa đơn (HoaDon)

- MaHD, NgayLap, MaKH, MaNV, MaXe/VIN, TongTien, TrangThaiThanhToan

### 4.2.6 Bảng báo cáo (BaoCao)

- MaBC, ThoiGian, ChiTieu, GiaTri, GhiChu

### 4.2.7 Sơ đồ quan hệ (Diagram)

- Users(1–n)NhanVien; NhaCungCap(1–n)SanPhamXe; SanPhamXe(1–n)HoaDon; NhanVien(1–n)HoaDon; BaoCao tổng hợp từ HoaDon & SanPhamXe.

---

# CHƯƠNG 5: LẬP TRÌNH

## 5.1 Ngôn ngữ và công cụ

- Java Swing; NetBeans IDE 8.2; Hệ quản trị CSDL: SQL Server (hoặc MySQL tuỳ chọn).

## 5.2 Mô tả mã nguồn (tóm tắt)

- Xử lý đăng nhập: kiểm tra thông tin, phân quyền.
- Kết nối CSDL: JDBC; tầng DAO cho các bảng Users, NhanVien, SanPhamXe, NhaCungCap, HoaDon, BaoCao.

---

# CHƯƠNG 6: KIỂM THỬ PHẦN MỀM

## 6.1 Phương pháp kiểm thử

- Hộp đen: dựa theo yêu cầu và giao diện, không can thiệp code.

## 6.2 Kịch bản kiểm thử (tóm tắt)

- Kiểm tra bố cục giao diện, điều hướng Tab/Enter, chọn giá trị danh sách.
- Chức năng đăng nhập: nhập tài khoản/mật khẩu -> vào menu.
- Chức năng quản lý: thêm/sửa/xoá nhân viên, xe, nhà cung cấp; lập/sửa/xoá hoá đơn; dữ liệu hiển thị đúng sau cập nhật.

---

# CHƯƠNG 7: ĐÓNG GÓI VÀ BẢO TRÌ PHẦN MỀM

## 7.1 Đóng gói

- Đóng gói dưới định dạng JAR/installer để dễ cài đặt.

## 7.2 Bảo trì

- Sửa lỗi, thích ứng môi trường, bổ sung yêu cầu mới; kiểm soát chi phí bảo trì theo độ phức tạp và số lượng thay đổi.

---

# KẾT LUẬN

Đề tài “Quản lý mua bán xe ô tô” đã chuyển đổi thành công từ miền cũ sang miền ô tô trong khi giữ nguyên các chức năng cốt lõi (đăng nhập, quản lý nhân viên, nhà cung cấp, sản phẩm/xe, hóa đơn, báo cáo). Hệ thống hỗ trợ quản lý tồn kho theo VIN, quy trình báo giá–hợp đồng–hóa đơn–thanh toán, giao xe và báo cáo vận hành.

Do hạn chế về thời gian và dữ liệu thực tế, một số phần (tích hợp tài chính/bảo hiểm, đăng ký biển số trực tuyến) mới mô tả ở mức khái quát. Rất mong nhận được góp ý để hoàn thiện.

## Hướng phát triển

- Tích hợp CRM, lịch hẹn lái thử; App di động cho tư vấn.
- Tích hợp ngân hàng/bảo hiểm (tính vay, duyệt hồ sơ, hợp đồng điện tử).
- Theo dõi trạng thái đăng ký biển số; dashboard BI.
- Mở rộng sang dịch vụ sau bán hàng (bảo dưỡng, phụ tùng).

## Tài liệu tham khảo

1. Giáo trình Công nghệ phần mềm.
2. Giáo trình Phân tích thiết kế hướng đối tượng (UML).
3. Tài liệu Java/SQL và mẫu kiến trúc ứng dụng quản lý.
