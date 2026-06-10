# LaptopStore - ASP.NET MVC E-Commerce Project

Một ứng dụng web thương mại điện tử chuyên nghiệp được xây dựng trên nền tảng ASP.NET MVC, phục vụ cho việc quản lý và kinh doanh máy tính xách tay (Laptop). Dự án được cấu trúc theo mô hình chuẩn MVC (Model - View - Controller), phân tách rõ ràng giữa giao diện người dùng và logic xử lý nghiệp vụ.

## 🚀 Tính năng chính

### Phân hệ khách hàng (Client Side)
- **Xem sản phẩm:** Duyệt danh sách laptop, lọc sản phẩm theo danh mục (Category), hãng sản xuất.
- **Xem chi tiết:** Hiển thị thông số kỹ thuật, giá cả, mô tả chi tiết và hình ảnh sản phẩm.
- **Giỏ hàng (Cart):** Thêm, xóa, cập nhật số lượng sản phẩm trong giỏ hàng.
- **Đặt hàng (Checkout):** Nhập thông tin giao hàng và gửi đơn hàng vào hệ thống.

### Phân hệ quản trị (Admin Area - `/Areas/Admin`)
- **Quản lý sản phẩm:** Thêm, sửa, xóa thông tin laptop, quản lý số lượng tồn kho.
- **Quản lý danh mục:** Quản lý các nhóm sản phẩm (Gaming, Văn phòng, Đồ họa...).
- **Quản lý đơn hàng:** Theo dõi trạng thái đơn hàng của khách hàng.

## 📂 Cấu trúc mã nguồn (Project Architecture)

Dự án áp dụng mô hình phân lớp chuẩn của ứng dụng .NET Framework / .NET Core:
- `Areas/Admin/`: Phân hệ quản trị hệ thống (Admin Panel) với các Controller và View độc lập.
- `Controllers/`: Tiếp nhận request từ client, xử lý điều hướng logic nghiệp vụ bán hàng.
- `Models/`: Định nghĩa các thực thể dữ liệu chính (Laptop, Category, Order, OrderDetail, User) và kết nối Cơ sở dữ liệu qua Entity Framework.
- `ViewModels/`: Đóng gói dữ liệu (Data Transfer Objects) để tối ưu hóa việc truyền dữ liệu từ Controller ra View hiển thị.
- `Views/`: Hệ thống giao diện hiển thị sử dụng Razor Engine (`.cshtml`) kết hợp Bootstrap.

## 🛠️ Công nghệ sử dụng

- **Ngôn ngữ:** C# (.NET)
- **Framework:** ASP.NET MVC, Entity Framework (Code First / Database First)
- **Cơ sở dữ liệu:** SQL Server
- **Giao diện:** HTML5, CSS3, JavaScript, Bootstrap UI Kit

## 🛠️ Hướng dẫn cài đặt và chạy ứng dụng

1. **Clone mã nguồn:**
   ```bash
   git clone https://github.com
   ```
2. **Cấu hình Database:** 
   Thay đổi chuỗi kết nối kết nối `ConnectionString` trong file cấu hình (`web.config` hoặc `appsettings.json`) phù hợp với Microsoft SQL Server của bạn.
3. **Chạy dự án:** 
   Mở file dự án bằng Visual Studio, nhấn `F5` hoặc `Ctrl + F5` để khởi chạy ứng dụng trên Localhost.
