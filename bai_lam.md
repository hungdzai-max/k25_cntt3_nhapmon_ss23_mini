# bai_lam

# BÀI LÀM – HACKATHON 02

- **Mã đề:** 01
- **Họ tên: vũ mạnh hùng**
- **Lớp:**
- **Link repository:**
- **Hệ điều hành (Windows/macOS):**

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```bash
hiển thị đường dẫn tuyệt đối của thư mục: pwd
liệt kê nội dung gồm file ẩn: ls
di chuyển file ghi_chu_ban_giao.txt vào docs: mv .\ghi_chu_ban_giao.txt docs
tạo thư mục backup trong thư mục gốc: mkdir
sao chép data/dat_san_thang_10.xlsx vào backup: cp data/dat_san_thang_10.xlsx backup
xóa file.tmp tại thư mụ gốc: rm .\temp_002.tmp
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```
(Dán kết quả vào đây – xoá dòng này)
```

## 4.3. Lọc log truy cập website

### a) Lệnh lọc các dòng status=500

```bash
get-content logs/access.log | select-string status=500
```

### 2 dòng đầu tiên trong logs/loi_500.txt

```
2026-10-28 08:03:17 GET /lich-san status=200
2026-10-28 08:05:28 GET /bang-gia status=200

```

### b) Lệnh đếm số dòng status=404 và kết quả

```bash
 (get-content logs/access.log | select-string status=404).count
```

```
4
```

## 4.4. Chạy script tong_hop (.ps1 hoặc .sh)

### 

# Script: tong_hop.ps1

# Tac gia: vũ hùng

# Ngay tao: 4/10

Write-Host "Dang tao bao cao..."
"=== BAO CAO SU CO WEBSITE ===" > logs/tong_hop.txt
Get-Content logs/access.log | Select-String "status=500" >> logs/tong_hop.txt
Get-Content  logs/access.log | Select-String "status=404" | Measure-Object >> logs/tong_hop.txt
Write-Host "Hoan thanh!"

### Nội dung file logs/tong_hop.txt

```
(Dán nội dung file vào đây – xoá dòng này)
```

## 4.5. README.md và bảo vệ thông tin bí mật

> README.md, .gitignore và .env.example được chấm trực tiếp trên file ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.
> 
- [ ]  README.md: Heading 1, mô tả có **in đậm** và *in nghiêng*, bảng, code block, task list, blockquote
- [ ]  .gitignore có dòng `.env` (tên file đúng, không có đuôi .txt)
- [ ]  .env.example có đủ tên biến, giá trị để trống (tên file đúng, không có đuôi .txt)

## 4.6. Kiểm tra trang web bằng DevTools (F12) và báo cáo lỗi

### Bảng lỗi

| STT | Tab DevTools phát hiện lỗi | Tên file hoặc thông báo lỗi | Cách khắc phục |
| --- | --- | --- | --- |
| 1 |  |  |  |
| 2 |  |  |  |

> Ảnh chụp màn hình lưu trong thư mục `evidence/` (network.png, console.png).
> 

### Báo cáo lỗi gửi trưởng nhóm

- **Context:**
- **Expected:**
- **Actual:**
- **Log:**

### Câu tìm kiếm Google

```
(Ghi câu tìm kiếm vào đây – xoá dòng này)
```

## 4.7. Excel

> Phần Excel được chấm trực tiếp trên file `data/dat_san_thang_10.xlsx`, không cần ghi vào đây.
>