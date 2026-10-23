# 03 – Báo cáo lưu chuyển tiền tệ (Mẫu B03-DN)

> Căn cứ: Điều 114 Thông tư 200/2014/TT-BTC; Chuẩn mực kế toán “Báo cáo lưu chuyển tiền tệ”.  
> Mục tiêu thẩm định: đánh giá **chất lượng lợi nhuận**, khả năng tạo tiền, và phát hiện phân loại sai / che giấu thanh khoản.

---

## 1. Ý nghĩa tổng thể của BCLCTT

BCLCTT giải thích vì sao số dư **Tiền và tương đương tiền** thay đổi trong kỳ, chia 3 hoạt động:

| Luồng | Bản chất | Câu hỏi thẩm định |
|-------|----------|-------------------|
| **HĐKD (Operating – CFO)** | Tiền từ kinh doanh cốt lõi | DN có tự tạo tiền từ việc bán hàng không? |
| **HĐĐầu tư (Investing – CFI)** | Mua/bán TS dài hạn, đầu tư | Có “đốt tiền” đầu tư / thanh lý TS che dòng tiền? |
| **HĐTài chính (Financing – CFF)** | Vay/trả nợ, tăng vốn, trả cổ tức | Sống nhờ vay mới hay trả được nợ? |

**Phương trình kiểm soát cuối kỳ:**
```text
Tiền cuối kỳ = Tiền đầu kỳ + CFO + CFI + CFF ± ảnh hưởng tỷ giá
```
Số này phải khớp Mã **110** trên Bảng CĐKT.

---

## 2. Hai phương pháp lập – điểm kiểm toán khác nhau

### 2.1. Phương pháp trực tiếp (ưu tiên khuyến khích)

Trình bày trực tiếp các khoản thu/chi tiền HĐKD.

| Mã (điển hình) | Chỉ tiêu | Nguồn kiểm tra |
|----------------|----------|----------------|
| 01 | Thu từ bán hàng, cung cấp DV | Sổ tiền + đối chiếu DT & Δ phải thu |
| 02 | Thu khác từ HĐKD | Phạt, hoàn thuế, ký quỹ… |
| 03 | Chi trả cho người cung cấp | Chi tiền + Δ phải trả / tồn kho |
| 04 | Chi trả người lao động | Bảng lương, BHXH |
| 05 | Chi lãi vay | Lãi đã trả (không gồm vốn hóa nếu đúng chuẩn trình bày) |
| 06 | Chi thuế TNDN | Giấy nộp thuế |
| 07 | Chi khác cho HĐKD | |
| **20** | Lưu chuyển tiền thuần HĐKD | Tổng 01…07 |

### 2.2. Phương pháp gián tiếp (phổ biến)

Bắt đầu từ **LN trước thuế (Mã 01 = Mã 50 trên B02)** rồi điều chỉnh:

1. Các khoản **phi tiền** (khấu hao, dự phòng…)
2. Lãi/lỗ **hoạt động đầu tư** đã nằm trong LN
3. Biến động **vốn lưu động** (phải thu, tồn kho, phải trả…)
4. Tiền lãi vay / thuế TNDN đã trả

**Assertions chung BCLCTT:** Đầy đủ, Chính xác, Phân loại đúng 3 luồng, Trình bày & đối chiếu được.

---

## 3. Thủ tục kiểm tra chi tiết BCLCTT

### Bước 1 – Đối chiếu khung
1. Tiền đầu kỳ / cuối kỳ ↔ Mã 110 B01 (và thuyết minh tương đương tiền).
2. LN trước thuế (PP gián tiếp) ↔ Mã 50 B02.
3. Tổng CFO+CFI+CFF ± FX ↔ biến động tiền.

### Bước 2 – Tái lập (reperformance) các điều chỉnh trọng yếu
Với PP gián tiếp, KTV nên **tự lập lại** BCLCTT từ:
- Bảng CĐKT kỳ này / kỳ trước
- B02
- Sổ chi tiết khấu hao, dự phòng, thanh lý TS, vay…

### Bước 3 – Kiểm tra phân loại 3 luồng (rủi ro cao)
| Giao dịch | Phân loại đúng | Sai thường gặp |
|-----------|----------------|----------------|
| Trả gốc vay | CFF | Để nhầm CFO |
| Trả lãi vay | CFO (theo VAS phổ biến) | Nhầm CFF |
| Mua TSCĐ còn nợ | Không phải luồng tiền toàn bộ; phần đã trả = CFI | Ghi full giá trị như đã trả tiền |
| Chuyển nợ thành vốn | Không trình bày trên BCLCTT (phi tiền) | Ép vào CFF |
| Tiền gửi có kỳ hạn > 3 tháng | CFI (gửi/rút) | Nhầm “tiền” / CFO |

### Bước 4 – Phân tích chất lượng dòng tiền
Các tỷ số / quan hệ:
- `CFO / LNST` — bền vững nếu ổn định dương và gần 1 trong dài hạn
- `CFO / Nợ ngắn hạn` — khả năng thanh toán thực
- `Free cash flow ≈ CFO − Capex (CFI mua TS)`
- Chuỗi nhiều năm: LN tăng + CFO âm kéo dài → **cảnh báo gian lận dồn tích**

---

## 4. Từng nhóm chỉ tiêu – ý nghĩa, kiểm tra, sai sót

## 4.1. Lưu chuyển tiền từ HĐKD (CFO)

### Ý nghĩa thẩm định
CFO dương ổn định = khả năng tự tài trợ. CFO âm tạm thời có thể do tăng trưởng (tăng tồn kho/phải thu) — cần chứng minh bằng dữ liệu vận hành.

### Điều chỉnh vốn lưu động – kiểm tra chéo

| Biến động | Ảnh hưởng CFO (PP gián tiếp) | Thủ tục |
|-----------|------------------------------|---------|
| Tăng phải thu | Giảm CFO | Khớp Δ 131 đã kiểm toán |
| Tăng tồn kho | Giảm CFO | Khớp Δ 140 |
| Tăng phải trả người bán | Tăng CFO | Khớp Δ 311; cảnh báo nếu tăng do không trả được nợ |
| Tăng dự phòng / khấu hao | Tăng CFO (phi tiền) | Khớp sổ 214, 229, 352 |

### Sai sót / gian lận
| Mức | Ví dụ |
|-----|-------|
| Cơ bản | Sai dấu điều chỉnh Δ vốn lưu động |
| Thường gặp | Nhầm lãi vay / cổ tức vào sai luồng; quên loại giao dịch phi tiền |
| Gian lận nâng cao | **Phân loại lại** chi mua TS thành chi HĐKD (hoặc ngược lại) để làm đẹp CFO; bán phải thu (factoring) ghi nhận như CFO bền vững mà không thuyết minh; trì hoãn thanh toán NCC cuối năm để tăng CFO |

### Khắc phục
Điều chỉnh phân loại giữa CFO/CFI/CFF; thuyết minh thành phần bất thường; đánh giá lại kết luận về thanh khoản trong báo cáo kiểm toán / thư quản lý.

---

## 4.2. Lưu chuyển tiền từ HĐ đầu tư (CFI)

### Các chỉ tiêu điển hình
- Chi mua TSCĐ, BĐSĐT, XDCB
- Thu từ thanh lý TS
- Chi/thu từ cho vay, mua/bán công cụ nợ, góp vốn

### Thủ tục
1. Đối chiếu sổ 211/213/217/241 với số tiền thực chi (không lấy nguyên giá nếu còn nợ).
2. Vouching hợp đồng mua TS lớn + UNC.
3. Thu thanh lý: đối chiếu biên bản thanh lý & tiền về TK.
4. Phân tách rõ phần **tiền** vs phần **còn phải trả**.

### Gian lận
- Che Capex bằng cách ghi vào chi phí HĐKD (làm giảm LN nhưng… hoặc ngược lại vốn hóa để tăng CFO gián tiếp qua LN).
- “Bán” TS cho bên liên quan rồi thuê lại để tạo dòng tiền thu CFI giả tạo.

---

## 4.3. Lưu chuyển tiền từ HĐ tài chính (CFF)

### Các chỉ tiêu điển hình
- Thu từ phát hành cổ phiếu / nhận vốn góp
- Thu từ đi vay
- Chi trả nợ gốc vay / trái phiếu
- Chi trả cổ tức, lợi nhuận cho chủ sở hữu

### Thủ tục
1. Đối chiếu biến động 411, 320/338 với dòng tiền thực.
2. Thư xác nhận ngân hàng: giải ngân / trả nợ trong kỳ.
3. Nghị quyết chia cổ tức ↔ số tiền thực trả (phần chưa trả nằm ở phải trả).
4. Kiểm tra giao dịch phi tiền: chuyển nợ → vốn không đưa vào CFF.

### Gian lận
- Ghi nhận vay mới là “DT / thu khác” để làm đẹp CFO.
- Không trình bày đầy đủ hạn mức / đảo nợ ngắn hạn liên tục (evergreen) → rủi ro thanh khoản bị che.

---

## 5. Ảnh hưởng tỷ giá và tương đương tiền

1. Đánh giá lại tiền ngoại tệ cuối kỳ: chênh lệch trình bày riêng, không gộp vào 3 luồng.
2. Kiểm tra định nghĩa **tương đương tiền**: kỳ hạn ≤ 3 tháng kể từ ngày mua, rủi ro thay đổi giá trị không đáng kể.
3. Nhầm TGCK 6–12 tháng vào tiền → làm sai cả B01 và B03.

---

## 6. Ví dụ mẫu làm việc (PP gián tiếp – rút gọn)

```text
LN trước thuế                                         XXX
+ Khấu hao TSCĐ                                       XXX
+ Dự phòng phải thu / tồn kho                         XXX
− Lãi thanh lý TSCĐ                                   (XX)
+ Lãi vay (đưa xuống phần đã trả)                     XXX
− Tăng phải thu khách hàng                            (XX)
− Tăng hàng tồn kho                                   (XX)
+ Tăng phải trả người bán                             XXX
= Tiền thu từ HĐKD trước lãi & thuế                   XXX
− Lãi vay đã trả                                      (XX)
− Thuế TNDN đã trả                                    (XX)
= CFO                                                 XXX
± CFI                                                 XXX
± CFF                                                 XXX
± Ảnh hưởng tỷ giá                                    XXX
= Tăng/(giảm) tiền thuần                              XXX
+ Tiền đầu kỳ                                         XXX
= Tiền cuối kỳ                                        XXX  ↔ khớp B01 Mã 110
```

Mỗi dòng điều chỉnh cần **working paper tham chiếu** tới số dư đã kiểm toán.

---

## 7. Ma trận “LN đẹp – tiền yếu” (dùng khi nghi gian lận BCTC)

| Hiện tượng nhiều năm | Giả thuyết | Khoan vào |
|----------------------|------------|-----------|
| LN tăng, CFO giảm | DT ảo / không thu được tiền | 01 B02, 131, cut-off |
| CFO tăng nhờ tăng phải trả | Căng thanh khoản / giấu lỗ vận hành | 311, aging NCC |
| CFI thu lớn từ bán TS | Bán tài sản cốt lõi để che CFO yếu | 211, bên liên quan |
| CFF thu lớn từ vay ngắn hạn | Đảo nợ / phụ thuộc vốn vay | 320, covenant |
| Chênh lệch lớn CFO vs PP trực tiếp vs gián tiếp | Lỗi lập báo cáo hoặc cố ý | Tái lập toàn bộ |

---

## 8. Đánh giá trọng yếu với BCLCTT

- Sai **phân loại giữa 3 luồng** có thể không đổi tiền cuối kỳ nhưng **vẫn trọng yếu định tính** vì làm sai lệch phân tích thanh khoản và quyết định tín dụng.
- Sai tiền cuối kỳ → xử lý như sai Mã 110 (thường rất nhạy cảm).
- Khi CFO bị thổi phồng trọng yếu kèm dấu hiệu gian lận → xem xét ảnh hưởng đến ý kiến kiểm toán và đoạn nhấn mạnh / nghi ngờ hoạt động liên tục (VSA 570).

Tiếp theo: Thuyết minh B09 — nơi thường **ẩn** các rủi ro không nằm trên mặt các báo cáo chính.
