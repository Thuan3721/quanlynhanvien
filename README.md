# Hệ Thống Quản Lý Nhân Viên

Ứng dụng desktop quản lý nhân viên công ty, xây dựng bằng **C# WinForms** và **SQL Server**.

> Đây là **dự án nhóm** (Nhóm 1)

## Chức năng chính

- Đăng nhập, quản lý tài khoản người dùng
- Quản lý nhân viên (thêm, sửa, xóa, tìm kiếm, khôi phục nhân viên đã xóa)
- Quản lý phòng ban, chức vụ
- Quản lý hợp đồng lao động
- Chấm công và xem chi tiết chấm công
- Quản lý và tính lương
- Quản lý dự án, chi tiết dự án
- Báo cáo, thống kê: nhân viên, chấm công, lương, dự án, báo cáo tổng hợp
- Xuất báo cáo ra Excel và PDF
- Tạo mã QR cho nhân viên

## Công nghệ sử dụng

- C# .NET Framework (Windows Forms)
- SQL Server, ADO.NET
- DataSet / ReportViewer cho báo cáo
- Visual Studio 2022

## Cách chạy dự án

1. Clone repo:
   ```
   git clone https://github.com/Thuan3721/quanlynhanvien.git
   ```
2. Mở SQL Server Management Studio, chạy file script trong thư mục `SQL/` để tạo database và dữ liệu mẫu.
3. Sửa chuỗi kết nối trong `App.config` (và `connectData.cs` nếu có) cho khớp với SQL Server trên máy bạn.
4. Tạo thư mục `ExcelXuatVaoDay` cạnh file chạy (nếu chưa có) để chứa file báo cáo xuất ra.
5. Mở `QuanLyNhanVien3.sln` bằng Visual Studio, restore NuGet packages, nhấn **F5** để chạy.

## Cấu trúc thư mục

| Thư mục / File | Nội dung |
|---|---|
| `F_*.cs` | Các form giao diện và xử lý (nhân viên, lương, chấm công, báo cáo...) |
| `connectData.cs` | Lớp kết nối cơ sở dữ liệu |
| `DataSet1-3.xsd` | Typed DataSet dùng cho báo cáo |
| `SQL/` | Script tạo database |
