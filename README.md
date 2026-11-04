# Website ôn tập Chi hội Máu 08/5

Website tĩnh, chạy trực tiếp trên Vercel. Không cần Node.js, framework hay build command.

## Cấu trúc
- `index.html`: giao diện và chức năng học.
- `cauhoi.json`: dữ liệu câu hỏi (351 câu hiện tại).
- `vercel.json`: cấu hình header để Vercel luôn kiểm tra phiên bản JSON mới.

## Deploy lên Vercel bằng GitHub
1. Tạo một repository GitHub mới.
2. Upload **cả 3 file** ở thư mục này lên thư mục gốc repository.
3. Vào https://vercel.com/new và Import repository đó.
4. Framework Preset chọn `Other`.
5. Build Command để trống; Output Directory để trống hoặc `.`.
6. Nhấn Deploy.

Sau khi deploy, website mở tại domain Vercel được cấp. Trang tự tải `cauhoi.json` cùng domain.

## Cập nhật câu hỏi
Chỉ sửa/thay `cauhoi.json`, giữ nguyên cấu trúc dữ liệu hiện tại, rồi commit/push lên GitHub. Vercel tự deploy lại. Không cần sửa `index.html` khi chỉ thay đổi nội dung câu hỏi.

## Cơ cấu đề ngẫu nhiên 30 câu
- 5 câu: Viện Huyết học - Truyền máu TW và Hội LHTN Việt Nam
- 5 câu: Chi hội trực thuộc
- 10 câu: Hiến máu tình nguyện
- 5 câu: Văn hoá tổ chức Hội Máu Việt Nam
- 5 câu: Vận động và tổ chức hiến máu

Lưu ý: Tên chủ đề trong JSON phải khớp chính xác với các tên chủ đề mà website sử dụng để tạo đề.
