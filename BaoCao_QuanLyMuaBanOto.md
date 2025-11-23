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

Xây dựng “Hệ thống phần mềm quản lý mua bán xe ô tô” cho một đại lý/ showroom, bao gồm các chức năng chính:

- Quản lý nhân viên (tư vấn bán hàng, kế toán, kho, quản lý)
- Quản lý nhà cung cấp/đối tác (hãng xe, ngân hàng, bảo hiểm, đăng kiểm)
- Quản lý sản phẩm (xe, phiên bản, màu, VIN, trạng thái tồn kho)
- Quản lý khách hàng, báo giá, hợp đồng, hóa đơn và thanh toán
- Quản lý quy trình giao xe (đăng ký biển số, bảo hiểm, PDI, bàn giao)
- Báo cáo thống kê (doanh số, tồn kho, lợi nhuận, hiệu suất nhân viên)

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
- Xây dựng được phần mềm với các chức năng cốt lõi, đơn giản và phù hợp với người quản lý và người sử dụng tại đại lý ô tô.



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
- Kết luận
- Hướng phát triển
- Tài liệu tham khảo

---

# LỜI NÓI ĐẦU

Trong bối cảnh kinh tế phát triển và nhu cầu di chuyển ngày càng tăng, thị trường ô tô tại Việt Nam chứng kiến sự tăng trưởng mạnh mẽ về số lượng mẫu xe, phiên bản, chính sách bán hàng và các dịch vụ đi kèm (tài chính, bảo hiểm, đăng ký, bảo dưỡng). Nhiều đại lý vẫn quản lý bằng sổ sách hoặc các file rời rạc, dẫn đến sai sót, thiếu đồng bộ, khó theo dõi tồn kho theo VIN, khó kiểm soát quy trình giao xe và doanh số theo từng tư vấn bán hàng.

Dựa trên kiến thức đã học về phân tích thiết kế hệ thống và kỹ thuật lập trình, em xây dựng đề tài “Hệ thống quản lý mua bán xe ô tô” nhằm tin học hóa các nghiệp vụ cốt lõi của một đại lý/showroom: quản lý xe, khách hàng, báo giá – hợp đồng – hóa đơn, quản lý nhà cung cấp/đối tác, quản lý nhân sự, báo cáo thống kê và quy trình giao xe.

Mặc dù đã nỗ lực khảo sát và tổng hợp, do thời gian và kinh nghiệm thực tế còn hạn chế, báo cáo khó tránh khỏi thiếu sót. Kính mong cô giáo và các thầy cô góp ý để hoàn thiện hơn. Em xin chân thành cảm ơn!

---

# CHƯƠNG 1: GIỚI THIỆU DỰ ÁN PHẦN MỀM

## 1.1 Khảo sát hiện trạng

Nhiều đại lý ô tô vận hành theo quy trình bán hàng truyền thống, dựa nhiều vào con người và các bảng tính rời rạc. Việc theo dõi tồn kho theo VIN/màu/phiên bản, quản lý báo giá – hợp đồng – tiến độ thanh toán, phối hợp đăng ký biển số, bảo hiểm, PDI và lịch bàn giao thường mất thời gian và dễ phát sinh sai sót, ảnh hưởng trải nghiệm khách hàng và hiệu quả kinh doanh.

### 1.1.1 Tổng quan (mẫu tham chiếu)

- Tên đại lý: Đại lý Ô tô Kim Tiền
- Tổng số nhân viên: 20
- Thời gian làm việc: 8:00 – 18:00 (Thứ 2 – Chủ nhật)
- Doanh thu bình quân/tháng: ~10.000.000.000 VNĐ
- Địa chỉ: 206 Kim Mã, Phường Kim Mã, Quận Ba Đình, Hà Nội
- Hotline: 09xx xxx xxx
- Hình thức kinh doanh: Bán xe ô tô mới, phụ kiện; dịch vụ tài chính – bảo hiểm – đăng kiểm; thu xe cũ đổi xe mới (nếu có)

## 1.2 Xác định bài toán cần giải quyết

Mục tiêu là xây dựng hệ thống phần mềm giúp:

- Quản lý danh mục xe (model, phiên bản, màu, số khung VIN, trạng thái: đặt cọc/giữ chỗ/còn hàng/đã bán/đang bàn giao)
- Quản lý khách hàng và lịch sử giao dịch, báo giá – hợp đồng – hóa đơn – công nợ
- Quản lý nhà cung cấp/đối tác (hãng xe, ngân hàng, bảo hiểm, đăng kiểm)
- Quản lý nhân viên và hiệu suất bán hàng
- Theo dõi quy trình giao xe (PDI, đăng ký, bảo hiểm, lịch bàn giao) và tồn kho
- Tổng hợp báo cáo doanh số, lợi nhuận, tồn kho theo thời gian/nhân viên/sản phẩm

## 1.3 Phân tích và đặc tả các hoạt động nghiệp vụ của hệ thống

### 1.3.1 Quy trình nhập xe (nhập kho)

1) Bộ phận bán hàng/kho lập đề nghị nhập xe theo nhu cầu và các đơn đặt cọc.
2) Quản lý duyệt và đặt xe từ hãng/nhà phân phối.
3) Xe về đại lý: kiểm tra chứng từ (CO, invoice, phiếu xuất), đối chiếu VIN, kiểm tra ngoại hình – tình trạng (PDI), cập nhật tồn kho và trạng thái.
4) Hàng đạt tiêu chuẩn nhập kho: hồ sơ hợp lệ, VIN trùng khớp, xe nguyên trạng.

Giá nhập kho = Σ(đơn giá từng xe) + chi phí liên quan (nếu có).

### 1.3.2 Quy trình bán hàng

1) Tư vấn nhu cầu, lái thử (nếu có), lập báo giá theo model/phiên bản/màu và các gói tài chính/bảo hiểm.
2) Khách đặt cọc: tạo hợp đồng/phiếu đặt cọc, giữ xe theo VIN.
3) Thanh toán theo tiến độ, hoàn tất hồ sơ đăng ký biển số, bảo hiểm, phụ kiện.
4) Bàn giao: nghiệm thu xe, ký biên bản bàn giao, xuất hóa đơn, cập nhật trạng thái xe “đã bán”.

### 1.3.3 Quản lý nhân viên

- Cơ cấu mẫu: 1 quản lý bán hàng, 8 tư vấn bán hàng, 4 nhân sự kho – giao xe, 2 kế toán, 1 quản trị hệ thống, các vị trí khác (marketing…)
- Chấm công theo ca/ngày, lương cơ bản + thưởng doanh số/đánh giá hiệu suất.
- Chính sách khen thưởng/kỷ luật, nghỉ phép… được quản lý trên hệ thống.

### 1.3.4 Báo cáo thống kê

- Doanh số theo tháng/quý/năm, theo tư vấn bán hàng, theo model/phiên bản.
- Tồn kho theo màu/VIN, vòng quay tồn kho, tỉ lệ hủy cọc.
- Lợi nhuận gộp theo hợp đồng/sản phẩm.

Doanh thu = ∑ Tiền bán – ∑ Chi phí/giá nhập liên quan.

## 1.4 Xác định yêu cầu của hệ thống

### 1.4.1 Yêu cầu chức năng

- Đăng nhập/Phân quyền theo vai trò (Quản lý, Tư vấn bán hàng, Kế toán, Kho)
- Quản lý nhân viên
- Quản lý nhà cung cấp/đối tác
- Quản lý xe (sản phẩm) và tồn kho theo VIN
- Quản lý báo giá – hợp đồng – hóa đơn – thanh toán
- Báo cáo thống kê

### 1.4.2 Yêu cầu phi chức năng

#### 1.4.2.1 Hiệu năng

- Tra cứu xe theo VIN/model trong < 2 giây với dữ liệu cỡ vừa.

#### 1.4.2.2 Khả năng tương tác

- Giao diện thân thiện, dễ dùng trên desktop; quy trình thao tác nhất quán.

#### 1.4.2.3 Tính dễ sử dụng

- Hỗ trợ tìm kiếm, lọc, xuất báo cáo; kiểm tra hợp lệ dữ liệu đầu vào.

#### 1.4.2.4 Ràng buộc thiết kế

- Kiến trúc đơn giản, dễ bảo trì; dữ liệu chuẩn hóa, theo dõi trạng thái theo VIN.

---

# CHƯƠNG 2: QUẢN LÝ DỰ ÁN

## 2.1 Ước lượng dự án

### 2.1.1 Ước lượng chi phí

Giai đoạn | Công việc | Mô tả | Chi phí (VND)
---|---|---|---
Quản lý dự án | Khảo sát yêu cầu dự án | Thu thập các yêu cầu tổng quan của dự án | 500.000 – 1.000.000
Quản lý dự án | Khởi tạo dự án | Thông báo triển khai dự án, lập project charter | 2.000.000 – 2.500.000
Quản lý dự án | Lập kế hoạch phạm vi dự án | Lập bản kế hoạch phạm vi dự án | 2.000.000 – 2.500.000
Quản lý dự án | Viết báo cáo tổng kết | Tổng kết lại toàn bộ công việc thành báo cáo cuối cùng | 0
Quản lý dự án | Rút kinh nghiệm | Rút kinh nghiệm cho đợt dự án sau | 0
Phân tích & thiết kế | Đặc tả chi tiết các yêu cầu | Mô tả cụ thể yêu cầu phần mềm | 2.000.000 – 2.500.000
Phân tích & thiết kế | Mô tả kiến trúc bằng các sơ đồ UML | Use case, trình tự, hoạt động | 2.000.000 – 2.500.000
Phân tích & thiết kế | Thiết kế cơ sở dữ liệu | Cấu trúc CSDL (bảng xe, khách hàng, hợp đồng, hóa đơn…) | 5.000.000 – 6.500.000
Phân tích & thiết kế | Thiết kế giao diện | Các form cốt lõi (xe, khách hàng, hợp đồng, báo cáo) | 5.000.000 – 6.500.000
Phân tích & thiết kế | Viết bản phân tích hệ thống chi tiết | Tổng hợp báo cáo phân tích thiết kế | 500.000 – 1.000.000
Module bán hàng | Phân tích yêu cầu module | Kế hoạch chức năng báo giá–hợp đồng–hóa đơn | 500.000 – 1.000.000
Module bán hàng | Thiết kế module | Form đăng nhập; form quản lý hợp đồng/hóa đơn | 5.000.000 – 6.500.000
Module bán hàng | Viết code module | Xử lý luồng báo giá–hợp đồng–thanh toán | 10.000.000 – 13.000.000
Module bán hàng | Cài đặt module | Chạy thử module | 0
Module bán hàng | Kiểm thử module | Giao diện, luồng nghiệp vụ, dữ liệu | 2.000.000 – 2.500.000
Module bán hàng | Viết báo cáo module | Mô tả chi tiết module | 0
Tích hợp | Tích hợp các module | Lắp ráp hoàn chỉnh để chạy thử | 2.000.000 – 2.500.000
Tích hợp | Kiểm thử tích hợp | Test tổng quan toàn hệ thống | 2.000.000 – 2.500.000
Tích hợp | Fix lỗi tồn tại | Sửa lỗi phát sinh khi test | 4.000.000 – 5.500.000
Chuyển giao | Tài liệu hướng dẫn | Hướng dẫn sử dụng phần mềm | 0
Chuyển giao | Lên kế hoạch bảo trì | Chuyển giao sản phẩm & kế hoạch bảo trì | 0
Kết thúc | Tổng kết dự án | Tổng kết & bàn giao | 0

> Bảng 2.1.1 Ước lượng chi phí

### 2.1.2 Ước lượng thời gian

Giai đoạn | Công việc | Mô tả | Thời gian
---|---|---|---
Quản lý dự án | Khảo sát yêu cầu | Thu thập yêu cầu tổng quan | 1 ngày
Quản lý dự án | Khởi tạo dự án | Lập project charter | 1 ngày
Quản lý dự án | Lập kế hoạch phạm vi | Kế hoạch phạm vi | 5 ngày
Quản lý dự án | Báo cáo tổng kết | Giai đoạn cuối dự án | Cuối dự án
Quản lý dự án | Rút kinh nghiệm | Bài học kinh nghiệm | Cuối dự án
Phân tích & thiết kế | Đặc tả chi tiết yêu cầu | Mô tả yêu cầu | 2 ngày
Phân tích & thiết kế | Sơ đồ UML | Use case, trình tự, hoạt động | 5 ngày
Phân tích & thiết kế | Thiết kế CSDL | Cấu trúc dữ liệu | 3 ngày
Phân tích & thiết kế | Thiết kế giao diện | Form cốt lõi | 4 ngày
Phân tích & thiết kế | Báo cáo phân tích | Hoàn chỉnh tài liệu | 2 ngày
Module bán hàng | Phân tích yêu cầu | Lập kế hoạch chi tiết | 2 ngày
Module bán hàng | Thiết kế module | Đăng nhập; hợp đồng/hóa đơn | 3 ngày
Module bán hàng | Viết code | Luồng báo giá–hợp đồng–thanh toán | 5 ngày
Module bán hàng | Cài đặt | Chạy thử | 1 ngày
Module bán hàng | Kiểm thử | Giao diện & dữ liệu | 3 ngày
Module bán hàng | Báo cáo module | Mô tả chi tiết | 1 ngày
Tích hợp | Tích hợp hệ thống | Lắp ráp module | 1 ngày
Tích hợp | Kiểm thử tích hợp | Test tổng quan | 1 ngày
Tích hợp | Fix lỗi | Sửa lỗi phát sinh | 2 ngày
Chuyển giao | Hướng dẫn sử dụng | Soạn tài liệu | 1 ngày
Chuyển giao | Kế hoạch bảo trì | Bàn giao | 1 ngày
Kết thúc | Tổng kết dự án | Tổng kết | 1 ngày

> Bảng 2.1.2 Ước lượng thời gian

### 2.1.3 Ước lượng người tham gia

- Số lượng: 3 người

Gồm: 1 PM/BA, 1 Dev fullstack, 1 Tester (kiêm hỗ trợ triển khai). Phân công theo các giai đoạn: khảo sát – phân tích thiết kế – phát triển – kiểm thử – tích hợp – chuyển giao – bảo trì.

> Bảng 2.1.3 Ước lượng người tham gia

## 2.2 Lập lịch và theo dõi

WBS rút gọn:

1. Khảo sát mô hình: khảo sát thực tế, phân tích yêu cầu (01/08/2022)
2. Báo cáo triển khai dự án, phạm vi dự án (01/08/2022)
3. Lập kế hoạch dự án (01/08/2022)
4. Phân tích & thiết kế hệ thống: quy trình nghiệp vụ, use case, trình tự, thống nhất thiết kế (02/08/2022)
5. Lập cơ sở dữ liệu: phân tích đối tượng, thuộc tính, thiết lập CSDL & nhập dữ liệu mẫu (03/08/2022)
6. Xây dựng chức năng đăng nhập/đăng ký và kiểm thử (04/08/2022)
7. Xây dựng chức năng hệ thống (form, xử lý, chạy thử) (05/08/2022)
8. Kiểm thử phần mềm (giao diện, dữ liệu, sửa lỗi) (06–08/08/2022)
9. Cài đặt, viết báo cáo module, kiểm tra dữ liệu (08/08/2022)
10. Tích hợp & bảo trì: kế hoạch bảo trì, kết thúc dự án (08/08/2022)

> Bảng 2.2: Lập lịch và theo dõi

---

# CHƯƠNG 3: PHÂN TÍCH THIẾT KẾ HỆ THỐNG

## 3.1 Các tác nhân chính tham gia hệ thống

### 3.1.1 Khách hàng

- Người mua xe; nhận báo giá, ký hợp đồng, thanh toán, nhận hóa đơn và bàn giao xe; được hỗ trợ đăng ký biển số, bảo hiểm, phụ kiện.

### 3.1.2 Tư vấn bán hàng (Nhân viên bán hàng)

- Tư vấn model/phiên bản/màu, lập báo giá, tạo hợp đồng/đặt cọc, cập nhật tiến độ, phối hợp các bộ phận để giao xe đúng hẹn.

### 3.1.3 Quản lý

- Theo dõi doanh số, tồn kho theo VIN, phê duyệt đặt hàng/nhập xe, quản lý nhân sự, nhà cung cấp/đối tác, xem báo cáo.

## 3.2 Các use case chính tham gia hệ thống

Có 5 use case chính:

- Nhân viên bán hàng: Quản lý hợp đồng/hóa đơn
- Quản lý: Quản lý nhân viên; Quản lý xe; Quản lý nhà cung cấp/đối tác; Báo cáo thống kê

## 3.3 Sơ đồ tổng quan và đặc tả (mô tả văn bản)

### 3.3.1 Use case tổng quát

- Phạm vi: quản lý danh mục, bán hàng, giao xe, báo cáo.

### 3.3.2 Đăng nhập

#### Đặc tả use case đăng nhập

- Tác nhân: Quản lý, Nhân viên bán hàng, Kế toán, Kho
- Mô tả: Người dùng đăng nhập để truy cập các chức năng theo vai trò; đăng xuất khi kết thúc.
- Dòng sự kiện chính:
  1) Mở giao diện đăng nhập
  2) Nhập tên đăng nhập/mật khẩu
  3) Hệ thống kiểm tra và phân quyền
  4) Thành công: vào màn hình chính; thất bại: thông báo và cho nhập lại

### 3.3.3 Quản lý nhân viên

#### Đặc tả use case quản lý nhân viên

- Tác nhân: Quản lý
- Mô tả: Thêm/sửa/xóa/tìm kiếm nhân viên; thông tin gồm mã NV, họ tên, ngày sinh, giới tính, liên hệ, chức vụ, trạng thái.
- Dòng sự kiện chính: nhập thông tin -> Thêm; chọn bản ghi -> Sửa/Xóa; Làm mới để nhập mới.

### 3.3.4 Quản lý nhà cung cấp/đối tác

#### Đặc tả use case quản lý nhà cung cấp/đối tác

- Tác nhân: Quản lý
- Mô tả: Quản lý hãng xe, ngân hàng, bảo hiểm, đăng kiểm; thông tin gồm mã, tên, địa chỉ, điện thoại, loại đối tác.
- Dòng sự kiện chính: Thêm/Sửa/Xóa tương tự quản lý nhân viên.

### 3.3.5 Quản lý hợp đồng/hóa đơn bán xe

#### Đặc tả use case quản lý hợp đồng/hóa đơn

- Tác nhân: Nhân viên bán hàng, Kế toán
- Mô tả: Lập báo giá -> hợp đồng/đặt cọc -> hóa đơn -> thanh toán -> bàn giao.
- Dòng sự kiện chính: yêu cầu tạo -> nhập thông tin khách hàng/xe/VIN/giá -> xác nhận lưu -> cập nhật CSDL -> hiển thị danh sách.

### 3.3.6 Quản lý xe (sản phẩm)

#### Đặc tả use case quản lý xe

- Tác nhân: Quản lý, Kho
- Mô tả: Quản lý model/phiên bản/màu/VIN/trạng thái; Thêm/Sửa/Xóa, tìm kiếm theo VIN.

### 3.3.7 Báo cáo thống kê

#### Đặc tả use case báo cáo

- Tác nhân: Quản lý
- Mô tả: Xem doanh số theo thời gian/nhân viên/sản phẩm; tồn kho theo VIN; xuất báo cáo.

---

# KẾT LUẬN

Sau thời gian nghiên cứu và triển khai, đề tài “Quản lý mua bán xe ô tô” đã bước đầu hoàn thiện các nội dung: khảo sát hiện trạng, xác định bài toán, phân tích – đặc tả nghiệp vụ, quản lý dự án, thiết kế tổng quan và mô tả use case cốt lõi. Hệ thống hướng tới giải quyết các vấn đề then chốt tại đại lý ô tô: quản lý tồn kho theo VIN, luồng báo giá–hợp đồng–hóa đơn–thanh toán–bàn giao, phối hợp đa bộ phận và báo cáo điều hành.

Do hạn chế về thời gian và dữ liệu khảo sát, báo cáo còn có thể thiếu các chi tiết chuyên sâu (tích hợp tài chính – bảo hiểm, đăng ký trực tuyến…). Rất mong nhận được góp ý để hoàn thiện hơn.

## Hướng phát triển

- Tích hợp CRM và lịch hẹn lái thử; quản lý pipeline bán hàng.
- Tích hợp ngân hàng/bảo hiểm (tính khoản vay, duyệt hồ sơ, phát hành hợp đồng điện tử).
- Quản lý quy trình đăng ký biển số trực tuyến; theo dõi trạng thái hồ sơ.
- Ứng dụng di động cho tư vấn bán hàng (tra cứu tồn kho VIN, tạo báo giá nhanh).
- Dashboard BI realtime (doanh số, tồn kho, hiệu suất nhân viên).
- Khả năng mở rộng sang quản lý dịch vụ sau bán hàng (bảo dưỡng, phụ tùng).

## Tài liệu tham khảo

1. Giáo trình Công nghệ phần mềm
2. Giáo trình Phân tích thiết kế hướng đối tượng (UML)
3. Tài liệu Java/SQL và các mẫu thiết kế kiến trúc ứng dụng quản lý
