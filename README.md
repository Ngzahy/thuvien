# 📚 Hệ Thống Quản Lý Thư Viện - Thiết Kế Sơ Đồ  

## 📌 Mô tả  
Dự án này bao gồm các sơ đồ thiết kế hệ thống cho **Hệ thống quản lý thư viện**, giúp quản lý sách, độc giả, và quá trình mượn/trả sách một cách hiệu quả.  

## 🛠 Các sơ đồ được thiết kế:  
### 1️⃣ **Sơ đồ Use Case**  
- Thể hiện mối quan hệ giữa người dùng (Thủ thư, Độc giả, Quản trị viên) và các chức năng chính của hệ thống.  
- Các Use Case chính:  
  ✅ Quản lý sách (Thêm, sửa, xóa, tìm kiếm)  
  ✅ Quản lý độc giả (Thêm, sửa, xóa tài khoản)  
  ✅ Quản lý mượn/trả sách  
  ✅ Xử lý vi phạm (Quá hạn, mất sách)  
  ✅ Tìm kiếm sách  
  ✅ Xem thông tin tài khoản  

### 2️⃣ **Sơ đồ Activity (Luồng mượn sách)**  
- Biểu diễn luồng hoạt động khi một độc giả muốn mượn sách.  
- Các bước chính:  
  1. Độc giả đăng nhập hệ thống.  
  2. Tìm kiếm sách theo tiêu đề, tác giả, thể loại.  
  3. Nếu sách có sẵn → Đăng ký mượn.  
  4. Thủ thư xác nhận yêu cầu mượn.  
  5. Độc giả nhận sách và theo dõi thời hạn trả.  
  6. Khi đến hạn, độc giả trả sách hoặc bị xử lý vi phạm nếu quá hạn.  

### 3️⃣ **Sơ đồ ERD (Entity Relationship Diagram)**  
- Biểu diễn mô hình dữ liệu quan hệ giữa các bảng trong cơ sở dữ liệu.  
- Các thực thể chính:  
  - **Độc giả** (Mã độc giả, Tên, Email, SĐT, Trạng thái)  
  - **Sách** (Mã sách, Tiêu đề, Tác giả, Thể loại, Trạng thái)  
  - **Phiếu mượn** (Mã phiếu, Mã độc giả, Mã sách, Ngày mượn, Ngày trả, Trạng thái)  
  - **Nhân viên thư viện** (Mã nhân viên, Tên, Quyền hạn)  
  - **Lịch sử vi phạm** (Mã vi phạm, Mã độc giả, Nội dung, Mức phạt)
