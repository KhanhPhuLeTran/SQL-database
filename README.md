#  Xây dựng mô hình cơ sở dữ liệu quản lý mua bán xe của cửa hàng HonDa
### Mô tả hệ thống quản lý cửa hàng bán xe máy HonDa

Cửa hàng bán xe máy HonDa cung cấp các loại xe thuộc thương hiệu HonDa và có nhiều chi nhánh trên toàn quốc. Để đảm bảo công tác quản lý chặt chẽ và chính xác, hệ thống quản lý hoạt động bán xe của cửa hàng cần được xây dựng với các chức năng chính sau:

1. **Quản lý khách hàng:**
   - Thêm, sửa, xóa thông tin khách hàng.
   - Lưu trữ thông tin khách hàng mua hàng lần đầu để hưởng ưu đãi cho lần mua tiếp theo.
   
2. **Quản lý nhà sản xuất (NSX):**
   - Thêm, sửa, xóa thông tin NSX.
   - Đảm bảo nguồn gốc xe rõ ràng và hợp tác với NSX uy tín.

3. **Quản lý bảo hành:**
   - Quản lý thông tin bảo hành để tránh sai sót trong chăm sóc khách hàng sau mua bán.

4. **Quản lý loại xe và xe:**
   - Lưu trữ và phân loại các loại xe kinh doanh.
   - Thêm mới, sửa, xóa thông tin loại xe và xe.

5. **Quản lý nhân viên:**
   - Thêm, sửa, xóa thông tin nhân viên.
   - Quản lý quá trình làm việc và hiệu quả kinh doanh của nhân viên.

6. **Quản lý nhập hàng:**
   - Kiểm định chất lượng sản phẩm trước khi nhập hàng.
   - Lập phiếu nhập hàng và thanh toán cho NSX.

7. **Quản lý xuất hàng:**
   - Lập phiếu xuất hàng, phiếu bảo hành và giao hàng cho khách hàng.
   - Giải quyết thanh toán qua nhiều hình thức như tiền mặt, thẻ, chuyển khoản hoặc trả góp.

### Xác định thuộc tính cho các thực thể trong hệ thống:

1. **Khách hàng:** MAKH, TENKH, NS, PHAI, DIACHI, SDT, EMAIL.
2. **NSX:** MANSX, TENNSX, ĐIACHI, SDT, EMAIL.
3. **Bảo hành:** MABH, GOIBH.
4. **Loại xe:** MALOAI, TENLOAI.
5. **Xe:** MAXE, TENXE, MALOAI, MABH, BAN, MAU, SL.
6. **Nhân viên:** MANV, TENNV, NS, PHAI, DIACHI, SDT, CHUCVU, LUONG, MANQL.
7. **Trả góp:** MAGOI, TRATRUOC, LAISUAT, THOIGIAN.
8. **Phiếu nhập:** MANHAP, NGNHAP, MANV, MANSX, MAXE, SLNHAP, DGNHAP, THUENHAP.
9. **Phiếu xuất:** MAXUAT, NGXUAT, MANV, MAKH, MAXE, SLXUAT, DGNHAP, THUEXUAT, PTTT, TRAGOP.

### Ưu nhược điểm của hệ thống cũ:

**Ưu điểm:**
- Quản lý dễ dàng, chi phí thấp.
- Phù hợp với hệ thống nhỏ.
- Các phần mềm quản lý có sẵn như Sapo, Pos365, KiotViet hỗ trợ nhanh chóng và tiện lợi.

**Nhược điểm:**
- Không đáp ứng được yêu cầu quản lý khi quy mô cửa hàng tăng lên.
- Khó khăn trong việc lưu trữ và tìm kiếm thông tin khách hàng lớn.
- Phần mềm quản lý có sẵn ít khi phù hợp tuyệt đối với nhu cầu của nhà quản lý.

### Hệ thống mới:
- Giảm bớt công việc của nhân viên.
- Dễ dàng quản lý cửa hàng hơn cho nhà quản lý.
