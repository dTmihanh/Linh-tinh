# 00 – Khung chung: Assertions, trọng yếu, mẫu kiểm toán, sai sót & gian lận

## 1. Mục tiêu Giai đoạn 2

Thu thập **bằng chứng kiểm toán đầy đủ, thích hợp** (VSA 500) để kết luận liệu từng khoản mục BCTC có sai sót trọng yếu do **nhầm lẫn** hoặc **gian lận** hay không.

Hai nhóm thủ tục:

| Nhóm | Mục đích | Khi nào tăng cường |
|------|----------|--------------------|
| **Thử nghiệm kiểm soát (TOC)** | Đánh giá hiệu quả KSNB | KSNB được thiết kế và vận hành tốt |
| **Thủ tục cơ bản (Substantive)** | Phát hiện sai sót số tiền | Luôn bắt buộc với khoản mục trọng yếu; tăng khi RMM cao |

Thủ tục cơ bản gồm: **phân tích cơ bản** + **kiểm tra chi tiết (tests of details)**.

---

## 2. Cơ sở dẫn liệu (Assertions) – “yếu tố phải đảm bảo”

### 2.1. Số dư tài khoản (Balance sheet)

| Assertion | Câu hỏi kiểm toán | Ví dụ sai |
|-----------|-------------------|-----------|
| **Hiện hữu (Existence)** | Tài sản/nợ có thực sự tồn tại? | Ghi nhận phải thu ảo |
| **Quyền và nghĩa vụ (Rights & Obligations)** | DN có quyền với TS / nghĩa vụ với nợ? | TSCĐ thế chấp nhưng không thuyết minh |
| **Đầy đủ (Completeness)** | Mọi khoản phải ghi đã được ghi? | Che giấu nợ phải trả |
| **Đánh giá và phân bổ (Valuation & Allocation)** | Số tiền ghi đúng giá trị? | Không trích dự phòng nợ xấu |
| **Trình bày và thuyết minh (Presentation)** | Phân loại NH/DH, thuyết minh đúng? | Vay dài hạn đến hạn vẫn để dài hạn |

### 2.2. Nghiệp vụ / kết quả kinh doanh (Income statement)

| Assertion | Câu hỏi kiểm toán | Ví dụ sai |
|-----------|-------------------|-----------|
| **Xảy ra (Occurrence)** | Nghiệp vụ có thực sự xảy ra? | Doanh thu giả |
| **Đầy đủ (Completeness)** | Mọi nghiệp vụ đã ghi? | Che giấu chi phí |
| **Chính xác (Accuracy)** | Số tiền tính đúng? | Sai tỷ giá, sai số lượng |
| **Cắt kỳ (Cut-off)** | Ghi đúng kỳ kế toán? | Đẩy doanh thu sang kỳ sau / kéo về kỳ này |
| **Phân loại (Classification)** | Đúng khoản mục? | Vốn hóa chi phí sửa chữa thành TSCĐ |
| **Trình bày (Presentation)** | Đúng mẫu B02 / thuyết minh? | Gộp doanh thu tài chính vào doanh thu bán hàng |

### 2.3. Lưu chuyển tiền tệ & thuyết minh

Ngoài các assertion trên, cần đảm bảo:
- **Phân loại đúng 3 luồng**: KD / Đầu tư / Tài chính
- **Đối chiếu được** với biến động Bảng CĐKT và KQHĐKD
- **Đầy đủ thuyết minh** bắt buộc theo B09-DN và các chuẩn mực VAS

---

## 3. Mức trọng yếu (VSA 320) – khung đánh giá

### 3.1. Ba tầng trọng yếu

| Tầng | Ký hiệu | Ý nghĩa thực hành |
|------|---------|-------------------|
| **Trọng yếu tổng thể BCTC** | Overall Materiality (OM) | Sai sót ≥ OM → ảnh hưởng quyết định người dùng |
| **Trọng yếu thực hiện** | Performance Materiality (PM) | Thường 50–75% OM; dùng để thiết kế thủ tục, giảm rủi ro tích lũy |
| **Ngưỡng rõ ràng tầm thường** | Clearly Trivial (CT) | Thường 1–5% OM; dưới ngưỡng này không tích lũy vào bảng sai sót |

### 3.2. Công thức tham chiếu thường dùng (điều chỉnh theo ngành)

| Cơ sở | Tỷ lệ tham chiếu | Phù hợp khi |
|-------|------------------|-------------|
| Lợi nhuận trước thuế | 3–10% (thường 5%) | DN ổn định, có lãi |
| Doanh thu thuần | 0,5–2% | DN break-even / biến động LN mạnh |
| Tổng tài sản | 0,5–2% | DN tài chính, bất động sản, chưa có lãi |
| Vốn chủ sở hữu | 1–5% | DN vốn lớn, LN thấp |

### 3.3. Trọng yếu theo khoản mục (Specific materiality)

Đặt thấp hơn OM khi khoản mục nhạy cảm với người dùng:
- Thù lao ban lãnh đạo, giao dịch bên liên quan
- Vi phạm cam kết vay (covenant)
- Thuế phải nộp / tranh chấp pháp lý
- Các khoản mục liên quan mục tiêu thưởng / IPO

### 3.4. Ma trận phân loại sai sót (VSA 450)

| Loại | Định nghĩa | Xử lý |
|------|------------|-------|
| **Factual** | Sai sót đã chứng minh chắc chắn | Yêu cầu điều chỉnh |
| **Judgmental** | Khác biệt về ước tính / chính sách | Thảo luận với BGĐ; có thể điều chỉnh |
| **Projected** | Sai sót mẫu ngoại suy ra tổng thể | Đánh giá thêm; có thể mở rộng mẫu |

**Quyết định trọng yếu:**
- Một sai sót ≥ OM → trọng yếu đơn lẻ
- Tổng sai sót chưa điều chỉnh ≥ OM → trọng yếu tích lũy
- Sai sót < OM nhưng mang tính định tính (gian lận, che giấu, ảnh hưởng xu hướng) → vẫn có thể trọng yếu

---

## 4. Phương pháp chọn mẫu kiểm toán (VSA 530)

### 4.1. Ba cách chọn phần tử (VSA 500)

1. **Kiểm tra 100%** – ít phần tử giá trị lớn; rủi ro cao; dữ liệu tự động
2. **Chọn phần tử cụ thể** – key items: giá trị cao, bất thường, liên quan bên liên quan, gần cuối kỳ
3. **Lấy mẫu thống kê / phi thống kê** – suy luận về phần còn lại của tổng thể

### 4.2. Công thức cỡ mẫu tham chiếu (MUS / kiểm tra chi tiết)

Với rủi ro trung bình, công thức thực hành phổ biến:

```
n ≈ (Giá trị sổ sách của tổng thể × Hệ số tin cậy) / (PM − Sai sót kỳ vọng)
```

| Mức đảm bảo mong muốn | Hệ số tin cậy (xấp xỉ) |
|----------------------|------------------------|
| 95% | 3,0 |
| 90% | 2,3 |
| 80% | 1,6 |
| 70% | 1,2 |

**Ví dụ:** Phải thu = 100 tỷ; PM = 2 tỷ; kỳ vọng sai sót = 0; đảm bảo 90%  
→ n ≈ (100 × 2,3) / 2 = **115 phần tử** (có thể kết hợp key items + mẫu ngẫu nhiên).

### 4.3. Nguyên tắc mở rộng mẫu

- Phát hiện sai sót trong mẫu → ngoại suy → nếu projected error + factual gần PM → **mở rộng mẫu** hoặc yêu cầu DN tự kiểm tra 100% phần còn lại
- Không “thay thế” phần tử sai bằng phần tử đúng để giữ nguyên kết luận

---

## 5. Phân loại sai sót: Cơ bản – Thường gặp – Gian lận nâng cao

| Mức | Bản chất | Ví dụ |
|-----|----------|-------|
| **Cơ bản (Error)** | Nhầm lẫn kỹ thuật, thiếu kiểm soát | Sai cộng, quên khấu hao 1 tháng |
| **Thường gặp (Common misstatement)** | Áp dụng chính sách sai / ước tính thiên lệch | Cut-off doanh thu; dự phòng thiếu |
| **Gian lận nâng cao (Fraudulent FS)** | Cố ý che giấu, tạo chứng từ giả, override KSNB | Round-tripping; side letter; channel stuffing |

### Tam giác gian lận (VSA 240)

1. **Áp lực** – KPI, vay nợ, IPO, thuế
2. **Cơ hội** – KSNB yếu, override BGĐ
3. **Hợp lý hóa** – “chỉ tạm thời”, “vì lợi ích DN”

**Giả định bắt buộc:** Có rủi ro gian lận trong **ghi nhận doanh thu**, trừ khi đủ cơ sở bác bỏ và ghi hồ sơ.

---

## 6. Bộ bằng chứng chuẩn (theo độ tin cậy giảm dần)

1. Bằng chứng do KTV tự tạo / quan sát trực tiếp (kiểm kê, tái tính)
2. Xác nhận từ bên thứ ba độc lập (ngân hàng, khách hàng, luật sư)
3. Chứng từ gốc bên ngoài (hóa đơn đầu vào có kiểm tra thuế)
4. Chứng từ nội bộ có kiểm soát tốt
5. Thẩm vấn miệng (yếu nhất nếu đứng một mình)

**Nguyên tắc:** Kết hợp nhiều nguồn; ưu tiên bằng chứng **mâu thuẫn** hơn bằng chứng khẳng định suông.

---

## 7. Mẫu phiếu làm việc chuẩn cho mỗi khoản mục

Mỗi khoản mục nên có working paper gồm:

```
A. Số liệu BCTC / sổ cái / bảng tổng hợp chi tiết (đối chiếu 3 chiều)
B. Phân tích biến động YoY / vs ngân sách / vs ngành
C. Đánh giá rủi ro & assertion trọng tâm
D. Mức trọng yếu áp dụng (OM/PM/specific)
E. Thủ tục đã thực hiện + cỡ mẫu
F. Bằng chứng đính kèm (thư xác nhận, biên bản kiểm kê…)
G. Sai sót phát hiện (factual / judgmental / projected)
H. Đề xuất điều chỉnh & ảnh hưởng đến LN / TS / thuế
I. Kết luận assertion đạt / không đạt
```

---

## 8. Quy trình logic kiểm tra chi tiết (áp dụng mọi khoản mục)

```text
Số liệu BCTC
    → Đối chiếu sổ cái / bảng tổng hợp
    → Phân tích biến động & tỷ số
    → Xác định assertion rủi ro cao
    → Chọn key items + lấy mẫu
    → Vouching (sổ → chứng từ) và/hoặc Tracing (chứng từ → sổ)
    → Thủ tục bên thứ ba / hiện trường (nếu cần)
    → Đánh giá ước tính (VSA 540)
    → Tổng hợp sai sót → so với PM/OM
    → Yêu cầu điều chỉnh / thuyết minh
    → Kết luận
```

**Vouching:** chọn số trên sổ → lần về chứng từ gốc → kiểm **Hiện hữu / Occurrence**.  
**Tracing:** chọn chứng từ gốc → lần lên sổ → kiểm **Đầy đủ (Completeness)**.

---

## 9. Liên kết 4 báo cáo – kiểm tra chéo bắt buộc

| Kiểm tra chéo | Mục đích phát hiện |
|---------------|-------------------|
| Δ Phải thu vs Doanh thu vs Tiền thu | Doanh thu ảo / không thu được tiền |
| Δ Tồn kho vs Giá vốn vs Mua hàng | Thao túng tồn kho / giá vốn |
| Lợi nhuận cao nhưng CFO thấp kéo dài | Chất lượng lợi nhuận kém / gian lận dồn tích |
| Thuyết minh bên liên quan vs số dư PT/PT | Giao dịch không công bố |
| Cam kết ngoại bảng vs thư luật sư | Nợ tiềm ẩn bị ẩn |

Chi tiết từng khoản mục: xem các file 01–04; ma trận quyết định ý kiến: file 05.
