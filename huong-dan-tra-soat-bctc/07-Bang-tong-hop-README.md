# 07 – Bảng tổng hợp thẩm định theo khoản mục BCTC

Tài liệu dạng **bảng** phục vụ tra soát nhanh từng khoản mục theo đúng các cột:

| STT | Khoản mục BCTC | Báo cáo | Giải thích, ý nghĩa, ví dụ | Phương thức kiểm tra / điều kiện đảm bảo | Mẫu kiểm toán | Bằng chứng | Loại sai sót (cơ bản / thường gặp / nâng cao) | Cách khắc phục | Mức độ trọng yếu |
|-----|----------------|---------|----------------------------|------------------------------------------|---------------|------------|-----------------------------------------------|----------------|------------------|

## File bảng chi tiết

| File | Phạm vi |
|------|---------|
| [07a-Bang-B01-Tai-san.md](./07a-Bang-B01-Tai-san.md) | Bảng CĐKT – Tài sản (Mã 100–270) |
| [07b-Bang-B01-No-va-Von.md](./07b-Bang-B01-No-va-Von.md) | Bảng CĐKT – Nợ phải trả & Vốn CSH (Mã 300–440) |
| [07c-Bang-B02-KQHDKD.md](./07c-Bang-B02-KQHDKD.md) | Báo cáo KQHĐKD (Mã 01–60) |
| [07d-Bang-B03-B09.md](./07d-Bang-B03-B09.md) | Báo cáo LCTT & Thuyết minh B09 |
| [07-Bang-tong-hop.csv](./07-Bang-tong-hop.csv) | **File CSV đầy đủ** – mở bằng Excel/Google Sheets |

## Chú giải cột “Mức độ trọng yếu”

Vì trọng yếu phụ thuộc OM/PM của từng cuộc kiểm toán, cột này ghi **mức độ nhạy cảm điển hình**:

| Ký hiệu | Ý nghĩa |
|---------|---------|
| **TW-Cao** | Thường trọng yếu hoặc rất nhạy cảm định tính (tiền, DT, gian lận) |
| **TW-TB** | Thường trọng yếu theo quy mô; cần đối chiếu PM |
| **TW-Thấp** | Thường dưới ngưỡng nếu số dư nhỏ; vẫn có thể TW định tính |
| **Định tính** | Dù số nhỏ vẫn có thể trọng yếu (gian lận, covenant, thuyết minh) |

## Cách dùng nhanh

1. Mở CSV bằng Excel → lọc theo cột “Báo cáo” hoặc “Mức độ”.
2. Hoặc đọc từng file 07a–07d theo báo cáo đang thẩm định.
3. Kết hợp với `05-Bang-danh-gia-trong-yeu.md` khi tổng hợp sai sót.
