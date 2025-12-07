# TRƯỜNG ĐẠI HỌC ĐIỆN LỰC

## KHOA CÔNG NGHỆ THÔNG TIN



# BÁO CÁO CHUYÊN ĐỀ HỌC PHẦN

## MÔN CÔNG NGHỆ PHẦN MỀM

### ĐỀ TÀI: QUẢN LÝ KÝ TÚC XÁ TRƯỜNG ĐẠI HỌC ĐIỆN LỰC



- Sinh viên thực hiện: BÙI XUÂN SƠN
- Giảng viên hướng dẫn: (cập nhật GVHD)
- Ngành: CÔNG NGHỆ THÔNG TIN
- Chuyên ngành: CÔNG NGHỆ PHẦN MỀM
- Lớp: (ví dụ) D15CNPM5
- Khóa: D15



Hà Nội, tháng …

---

## Mô tả tóm tắt đề tài

Xây dựng “Hệ thống phần mềm quản lý ký túc xá” cho Trường Đại học Điện Lực, bám theo cấu trúc và cách trình bày của tài liệu mẫu (BaoCao_QuanLyMuaBanOto_full), nhưng nội dung chuyển sang miền KTX.

Chức năng trọng tâm:

- Đăng nhập, phân quyền
- Tiếp nhận & xét duyệt hồ sơ nội trú, ký hợp đồng
- Quản lý khu/nhà/phòng/giường; phân phòng, đổi/trả phòng
- Ghi chỉ số điện/nước, tính phí, lập hóa đơn, thanh toán, công nợ
- Quản lý tài sản phòng, phiếu bảo trì, vi phạm nội quy, khách/ra-vào
- Báo cáo thống kê vận hành KTX

Tham chiếu biểu đồ (Mermaid, HTML): KTX_Diagrams.html

### 1. Nội dung thực hiện

- Chương 1: Giới thiệu dự án phần mềm.
- Chương 2: Quản lý dự án.
- Chương 3: Phân tích hệ thống.
- Chương 4: Thiết kế.
- Chương 5: Lập trình.
- Chương 6: Kiểm thử phần mềm.
- Chương 7: Đóng gói và bảo trì phần mềm.

### 2. Kết quả đạt được

- Hoàn thiện bộ tài liệu phân tích–thiết kế cho hệ thống QL KTX.
- Bộ sơ đồ đầy đủ (Phân rã chức năng, DFD mức 0/1/2, ERD) – xem file HTML.
- Mô hình quan hệ dữ liệu và mô tả chi tiết bảng phục vụ triển khai.



Hà Nội, ngày … tháng … năm 2025

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

Ký túc xá là môi trường sống học tập của sinh viên với quy mô lưu trú lớn, nhiều nghiệp vụ: tiếp nhận hồ sơ – xét duyệt – phân phòng/giường – hợp đồng – tính phí (phòng, điện/nước, dịch vụ) – thu/đối soát – bảo trì – khách/ra vào – vi phạm – báo cáo. Quản lý thủ công gây chậm trễ, sai sót và khó tổng hợp dữ liệu.

Từ kiến thức môn Phân tích & Thiết kế hệ thống và Công nghệ phần mềm, báo cáo đề xuất hệ thống “Quản lý ký túc xá” số hóa nghiệp vụ cốt lõi, đảm bảo dữ liệu nhất quán, quy trình minh bạch, và khả năng mở rộng.

Do thời gian có hạn, tài liệu không tránh khỏi thiếu sót. Kính mong thầy/cô góp ý để hoàn thiện hơn.

---

# CHƯƠNG 1: GIỚI THIỆU DỰ ÁN PHẦN MỀM

## 1.1 Khảo sát hiện trạng

- Nhiều khâu còn thủ công: xét hồ sơ, phân phòng, chốt chỉ số, tính tiền, theo dõi công nợ.
- Dữ liệu phân tán: file rời, khó kiểm soát thay đổi và báo cáo tức thời.
- Rủi ro: trùng cấp giường, tính hóa đơn sai, chậm bảo trì, thiếu minh bạch.

### 1.1.1 Tổng quan

- Đơn vị: Ban quản lý KTX – Trường Đại học Điện Lực
- Quy mô: nhiều khu/nhà, tầng; phòng nhiều loại (4–8 giường…)
- Ca trực: 24/7 (bảo vệ), giờ hành chính (tiếp nhận, kế toán, kỹ thuật)
- Đối tượng phục vụ: sinh viên nội trú, khách thăm

## 1.2 Bài toán cần giải quyết

- Chuẩn hóa quy trình tiếp nhận – phân phòng – hợp đồng – thu phí – bảo trì – an ninh.
- Theo dõi phòng/giường trống – đang dùng; hợp đồng; công nợ; chỉ số điện/nước.
- Minh bạch báo cáo: lấp đầy, doanh thu, nợ quá hạn, bảo trì, vi phạm.

## 1.3 Phân tích hoạt động nghiệp vụ (tóm tắt)

- Tiếp nhận & xét duyệt: nhận hồ sơ SV, tiêu chí ưu tiên, danh sách chờ.
- Phân phòng/giường: xếp chỗ, đổi phòng, trả phòng; cập nhật trạng thái.
- Tính phí & hóa đơn: định phí theo loại phòng; điện/nước theo chỉ số; dịch vụ.
- Thanh toán & công nợ: ghi nhận phiếu thu, đối soát cổng thanh toán (tùy chọn).
- Bảo trì: tiếp nhận phiếu, xử lý, nghiệm thu, chi phí.
- An ninh & ra/vào: sổ ra/vào, khách; biên bản vi phạm; xử lý.
- Báo cáo: theo thời gian, khu/nhà, loại phòng, doanh thu, lấp đầy, vi phạm.

## 1.4 Yêu cầu của hệ thống

### 1.4.1 Yêu cầu chức năng (cốt lõi)

- Đăng nhập, phân quyền người dùng.
- Quản lý danh mục: Khu/nhà, loại phòng, phòng, giường, dịch vụ.
- Quản lý nội trú & hợp đồng; phân phòng/giường, đổi/trả phòng.
- Ghi chỉ số điện/nước; tính phí; lập hóa đơn; thanh toán.
- Quản lý tài sản – bảo trì; vi phạm; khách/ra-vào.
- Báo cáo/Thống kê.

### 1.4.2 Yêu cầu phi chức năng

- Hiệu năng: tra cứu nhanh theo phòng/giường, hợp đồng, kỳ hóa đơn.
- Dễ dùng: giao diện phù hợp nghiệp vụ KTX.
- Tin cậy: ràng buộc dữ liệu, kiểm soát trạng thái.
- Mở rộng: kết nối cổng thanh toán, SIS (tuỳ chọn).

---

# CHƯƠNG 2: QUẢN LÝ DỰ ÁN

## 2.1 Ước lượng (mẫu tham chiếu)

Tương tự cấu trúc ở tài liệu mẫu, điều chỉnh cho miền KTX: khảo sát, phân tích–thiết kế, xây dựng, tích hợp, kiểm thử, chuyển giao. Nhân sự tham chiếu: 1 PM/BA, 1 Dev fullstack, 1 Tester.

## 2.2 Lập lịch & theo dõi

WBS rút gọn: Khảo sát → Phân tích/Thiết kế → CSDL/Diagrams → Giao diện → Nghiệp vụ tính phí → Kiểm thử → Tài liệu người dùng.

---

# CHƯƠNG 3: PHÂN TÍCH THIẾT KẾ HỆ THỐNG

## 3.1 Tác nhân

- Sinh viên nội trú
- Cán bộ KTX (tiếp nhận, vận hành)
- Kế toán/Tài chính
- Kỹ thuật/Bảo trì
- Bảo vệ (ra/vào)
- Quản trị hệ thống

## 3.2 Ca sử dụng chính (tóm tắt)

- Đăng nhập/Phân quyền
- Quản lý danh mục (khu/nhà/phòng/giường/dịch vụ)
- Quản lý nội trú & hợp đồng
- Phân phòng/Đổi/Trả
- Ghi chỉ số/Tính phí/Hóa đơn/Thanh toán
- Bảo trì/Tài sản/Vi phạm/Khách – ra vào
- Báo cáo/Thống kê

## 3.3 Sơ đồ & mô hình

- Phân rã chức năng: xem KTX_Diagrams.html
- DFD Mức 0/1/2: xem KTX_Diagrams.html
- ERD: xem KTX_Diagrams.html

---

# CHƯƠNG 4: THIẾT KẾ

## 4.1 Thiết kế giao diện (tóm tắt)

- Đăng nhập → Trang chính: menu Danh mục, Nội trú/Hợp đồng, Phòng/giường, Chỉ số & hóa đơn, Thanh toán, Bảo trì, Vi phạm, Báo cáo.
- Form phân phòng: lọc phòng trống theo khu/loại, gợi ý giường, xác nhận.
- Form hóa đơn: chốt kỳ, tính phí phòng + điện/nước + dịch vụ, in/xuất.

## 4.2 Thiết kế lưu trữ (mô hình quan hệ dữ liệu)

- BUILDING(BuildingId PK, Code UQ, Name, Address)
- ROOM_TYPE(RoomTypeId PK, Code UQ, Name, Capacity, BasePrice)
- ROOM(RoomId PK, BuildingId FK→BUILDING, RoomTypeId FK→ROOM_TYPE, Number, Floor, Status)
- BED(BedId PK, RoomId FK→ROOM, BedNo, Status, UQ(RoomId,BedNo))
- RESIDENT(ResidentId PK, StudentCode UQ, FullName, Gender, DoB, Phone, Email, Department, Class)
- CONTRACT(ContractId PK, ResidentId FK→RESIDENT, BedId FK→BED, StartDate, EndDate, Status, DepositAmount)
- SERVICE(ServiceId PK, Code UQ, Name, Unit, Price)
- UTILITY_METER(MeterId PK, RoomId FK→ROOM, Type, Serial UQ, Active)
- METER_READING(ReadingId PK, MeterId FK→UTILITY_METER, Period YYYYMM, PrevIndex, CurrIndex, UQ(MeterId,Period))
- INVOICE(InvoiceId PK, ContractId FK→CONTRACT, Period YYYYMM, IssueDate, DueDate, Status, TotalAmount)
- INVOICE_ITEM(ItemId PK, InvoiceId FK→INVOICE, ItemType, RefId NULL, Description, Qty, UnitPrice, Amount)
- PAYMENT(PaymentId PK, InvoiceId FK→INVOICE, PaidDate, Method, RefNo UQ NULL, Amount, Status)
- ASSET(AssetId PK, Code UQ, Name, Unit, Price)
- ROOM_ASSET(RoomId FK→ROOM, AssetId FK→ASSET, Qty, PRIMARY KEY(RoomId, AssetId))
- MAINTENANCE_TICKET(TicketId PK, RoomId FK→ROOM, ReportedBy, ReportedAt, Category, Content, Status, Cost NULL)
- VIOLATION(ViolationId PK, ResidentId FK→RESIDENT, Date, Category, Detail, Penalty, Status)
- VISITOR_LOG(VisitId PK, ResidentId FK→RESIDENT NULL, RoomId FK→ROOM NULL, VisitorName, IdNo, InAt, OutAt, Note)
- USER(UserId PK, Username UQ, FullName, Email UQ NULL, PasswordHash, Status)
- ROLE(RoleId PK, Code UQ, Name)
- USER_ROLE(UserId FK→USER, RoleId FK→ROLE, PRIMARY KEY(UserId, RoleId))

### 4.2.1 Mô tả chi tiết các bảng (tóm lược)

Chi tiết tên cột, kiểu và ràng buộc xem mục 7 ở cuối tài liệu (bảng dữ liệu).

---

# CHƯƠNG 5: LẬP TRÌNH

## 5.1 Ngôn ngữ & công cụ

- Có thể triển khai .NET WinForms + EF Core + SQLite/MySQL hoặc Java Swing + JDBC + MySQL. Tùy điều kiện, giữ cấu trúc tầng: UI – Service/DAO – DB.

## 5.2 Mã nguồn (định hướng)

- Module Danh mục; Module Nội trú & Hợp đồng; Module Tính phí & Hóa đơn; Module Bảo trì; Module An ninh; Báo cáo.

---

# CHƯƠNG 6: KIỂM THỬ PHẦN MỀM

## 6.1 Phương pháp

- Hộp đen theo ca sử dụng; kiểm thử dữ liệu biên: trùng giường, chỉ số âm, kỳ hóa đơn trùng.

## 6.2 Kịch bản tiêu biểu

- Phân phòng khi hết giường → cảnh báo.
- Đổi phòng cập nhật hợp đồng & trạng thái giường.
- Chốt kỳ đọc số, tính hóa đơn đúng định mức.
- Thanh toán đủ → hóa đơn Paid; thiếu → công nợ.

---

# CHƯƠNG 7: ĐÓNG GÓI VÀ BẢO TRÌ

## 7.1 Đóng gói

- Đóng gói bộ cài/portable; cấu hình DB file (SQLite) hoặc MySQL.

## 7.2 Bảo trì

- Sửa lỗi, nâng cấp tính năng; thêm audit log, backup DB định kỳ.

---

# KẾT LUẬN

Hệ thống “Quản lý ký túc xá” chuẩn hóa quy trình, tăng minh bạch, giảm sai sót, hỗ trợ báo cáo điều hành. Mô hình dữ liệu và sơ đồ đã sẵn sàng cho hiện thực hóa với công nghệ phù hợp.

## Hướng phát triển

- Tích hợp cổng thanh toán, SIS; cổng thông tin SV tự phục vụ.
- Lập lịch bảo trì định kỳ; dashboard BI; thông báo đa kênh.
- Kiểm soát ra/vào bằng QR/RFID (tùy hạ tầng).

## Tài liệu tham khảo

1. Giáo trình Công nghệ phần mềm; Phân tích & Thiết kế hệ thống.
2. Tài liệu thiết kế CSDL quan hệ và mô hình hóa dữ liệu.
3. Hướng dẫn Mermaid (sơ đồ): https://mermaid.js.org/
4. Thực tế vận hành KTX (quy định nội trú, biểu phí tham chiếu).

---

## 7) Phụ lục: Mô tả chi tiết các bảng dữ liệu

Gợi ý kiểu: INT, VARCHAR(n), DATE, DATETIME, DECIMAL(12,2), BOOL.

### BUILDING
- BuildingId INT PK (identity)
- Code VARCHAR(20) UQ – mã khu/nhà
- Name VARCHAR(100)
- Address VARCHAR(255)

### ROOM_TYPE
- RoomTypeId INT PK
- Code VARCHAR(20) UQ – mã loại (P4, P6…)
- Name VARCHAR(100)
- Capacity INT – số giường
- BasePrice DECIMAL(12,2) – giá phòng/tháng cơ bản

### ROOM
- RoomId INT PK
- BuildingId INT FK→BUILDING
- RoomTypeId INT FK→ROOM_TYPE
- Number VARCHAR(20) – số phòng
- Floor INT
- Status VARCHAR(20) – Active/Inactive/Maintenance
- Index: (BuildingId, Number)

### BED
- BedId INT PK
- RoomId INT FK→ROOM
- BedNo VARCHAR(10)
- Status VARCHAR(20) – Empty/Occupied/Blocked
- UQ(RoomId, BedNo)

### RESIDENT
- ResidentId INT PK
- StudentCode VARCHAR(20) UQ
- FullName VARCHAR(120)
- Gender VARCHAR(10)
- DoB DATE
- Phone VARCHAR(20)
- Email VARCHAR(120)
- Department VARCHAR(120)
- Class VARCHAR(50)

### CONTRACT
- ContractId INT PK
- ResidentId INT FK→RESIDENT
- BedId INT FK→BED
- StartDate DATE
- EndDate DATE
- Status VARCHAR(20) – Draft/Active/Suspended/Ended
- DepositAmount DECIMAL(12,2)
- Index: (ResidentId, Status), (BedId, Status)

### SERVICE
- ServiceId INT PK
- Code VARCHAR(20) UQ (DIEN, NUOC, VS, WIFI…)
- Name VARCHAR(120)
- Unit VARCHAR(20) – kWh, m3, tháng
- Price DECIMAL(12,2)

### UTILITY_METER
- MeterId INT PK
- RoomId INT FK→ROOM
- Type VARCHAR(10) – ELECTRIC/WATER
- Serial VARCHAR(50) UQ
- Active BOOL

### METER_READING
- ReadingId INT PK
- MeterId INT FK→UTILITY_METER
- Period CHAR(6) – YYYYMM
- PrevIndex DECIMAL(12,2)
- CurrIndex DECIMAL(12,2)
- UQ(MeterId, Period)

### INVOICE
- InvoiceId INT PK
- ContractId INT FK→CONTRACT
- Period CHAR(6) – YYYYMM
- IssueDate DATE
- DueDate DATE
- Status VARCHAR(20) – Draft/Issued/Paid/Overdue/Cancelled
- TotalAmount DECIMAL(12,2)
- UQ(ContractId, Period)

### INVOICE_ITEM
- ItemId INT PK
- InvoiceId INT FK→INVOICE
- ItemType VARCHAR(20) – ROOM_FEE/UTILITY/SERVICE/PENALTY
- RefId INT NULL – tham chiếu đọc chỉ số/vi phạm/dịch vụ
- Description VARCHAR(255)
- Qty DECIMAL(12,2)
- UnitPrice DECIMAL(12,2)
- Amount DECIMAL(12,2)
- Index: (InvoiceId, ItemType)

### PAYMENT
- PaymentId INT PK
- InvoiceId INT FK→INVOICE
- PaidDate DATETIME
- Method VARCHAR(20) – CASH/BANK/ONLINE
- RefNo VARCHAR(50) NULL UQ – mã giao dịch/biên lai
- Amount DECIMAL(12,2)
- Status VARCHAR(20) – Pending/Success/Failed/Reversed

### ASSET
- AssetId INT PK
- Code VARCHAR(30) UQ
- Name VARCHAR(120)
- Unit VARCHAR(20)
- Price DECIMAL(12,2)

### ROOM_ASSET
- RoomId INT FK→ROOM
- AssetId INT FK→ASSET
- Qty DECIMAL(12,2)
- PK(RoomId, AssetId)

### MAINTENANCE_TICKET
- TicketId INT PK
- RoomId INT FK→ROOM
- ReportedBy VARCHAR(120)
- ReportedAt DATETIME
- Category VARCHAR(50)
- Content VARCHAR(500)
- Status VARCHAR(20) – Open/Assigned/Done/Cancelled
- Cost DECIMAL(12,2) NULL

### VIOLATION
- ViolationId INT PK
- ResidentId INT FK→RESIDENT
- Date DATETIME
- Category VARCHAR(50)
- Detail VARCHAR(500)
- Penalty DECIMAL(12,2)
- Status VARCHAR(20) – Open/Closed

### VISITOR_LOG
- VisitId INT PK
- ResidentId INT NULL FK→RESIDENT
- RoomId INT NULL FK→ROOM
- VisitorName VARCHAR(120)
- IdNo VARCHAR(30)
- InAt DATETIME
- OutAt DATETIME NULL
- Note VARCHAR(255) NULL

### USER / ROLE / USER_ROLE
- USER(UserId INT PK, Username VARCHAR(50) UQ, FullName VARCHAR(120), Email VARCHAR(120) NULL UQ, PasswordHash VARCHAR(255), Status VARCHAR(20))
- ROLE(RoleId INT PK, Code VARCHAR(30) UQ, Name VARCHAR(120))
- USER_ROLE(UserId INT FK→USER, RoleId INT FK→ROLE, PK(UserId, RoleId))
