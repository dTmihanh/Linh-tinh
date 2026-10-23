# 02 – Báo cáo kết quả hoạt động kinh doanh (Mẫu B02-DN)

> Căn cứ: Điều 113 Thông tư 200/2014/TT-BTC.  
> Báo cáo phản ánh kết quả từ **hoạt động KD chính + tài chính + khác** trong kỳ.  
> Khi lập BCTC tổng hợp với đơn vị phụ thuộc: **loại trừ** toàn bộ DT/CP nội bộ.

---

## Sơ đồ logic các chỉ tiêu cốt lõi

```text
01 Doanh thu bán hàng và cung cấp DV
- 02 Các khoản giảm trừ doanh thu
= 10 Doanh thu thuần
- 11 Giá vốn hàng bán
= 20 Lợi nhuận gộp
+ 21 Doanh thu hoạt động tài chính
- 22 Chi phí tài chính (trong đó 23: lãi vay)
- 24 Chi phí bán hàng
- 25 Chi phí quản lý DN
= 30 Lợi nhuận thuần từ HĐKD
+ 31 Thu nhập khác
- 32 Chi phí khác
= 40 Lợi nhuận khác
= 50 Tổng LN kế toán trước thuế
- 51 Chi phí thuế TNDN hiện hành
- 52 Chi phí thuế TNDN hoãn lại
= 60 Lợi nhuận sau thuế TNDN
```

*(Một số DN trình bày thêm lãi cơ bản/suy giảm trên mỗi cổ phiếu theo quy định riêng.)*

---

# 1. Doanh thu bán hàng và cung cấp dịch vụ (Mã 01) — RỦI RO GIAN LẬN CAO NHẤT

## 1.1. Ý nghĩa
Tổng doanh thu từ bán sản phẩm, hàng hóa, BĐS đầu tư (khi là hàng hóa), cung cấp dịch vụ… **chưa trừ** giảm trừ; **không gồm** thuế GTGT, thuế xuất khẩu, thuế TTĐB phải nộp (theo TT200).

## 1.2. Điều kiện ghi nhận (VAS 14 & nguyên tắc thực chất)
Cần đảm bảo (tùy loại giao dịch):
1. Đã chuyển giao rủi ro và lợi ích gắn với quyền sở hữu (hàng hóa) / đã hoàn thành dịch vụ hoặc phần dịch vụ có thể đo lường.
2. DN không còn nắm quyền quản lý / kiểm soát như chủ sở hữu.
3. Doanh thu đo lường được đáng tin cậy.
4. Có khả năng thu được lợi ích kinh tế.
5. Chi phí liên quan đo lường được đáng tin cậy.

## 1.3. Assertions phải đảm bảo

| Assertion | Rủi ro gian lận điển hình |
|-----------|---------------------------|
| **Occurrence** | Doanh thu giả, vòng tròn |
| **Accuracy** | Sai giá, sai số lượng, sai tỷ giá |
| **Cut-off** | Kéo DT về kỳ này / đẩy sang kỳ sau |
| **Completeness** | Che giấu DT (mục tiêu thuế) |
| **Classification** | Nhầm DT tài chính / thu nhập khác vào DT bán hàng |
| **Presentation** | Không tách giảm trừ; gộp thuế vào DT |

## 1.4. Thủ tục kiểm tra chi tiết

### A. Thủ tục phân tích (thực hiện trước)
- So sánh DT theo tháng/quý: đột biến tháng 12?
- Biên LN gộp theo dòng sản phẩm / theo khách hàng.
- DT vs số lượng tiêu thụ vs giá bình quân ngành.
- DT vs phải thu vs tiền thu từ khách.
- Hệ số: `DT tăng X% nhưng CFO giảm` → cảnh báo chất lượng DT.

### B. Kiểm tra chi tiết – mẫu chuẩn
1. **Tách doanh thu theo luồng:** bán nội địa, xuất khẩu, dịch vụ, nội bộ, bên liên quan.
2. **Key items:** hợp đồng lớn, giao dịch gần ngày khóa sổ, bên liên quan, doanh thu bất thường, ghi nhận một lần (lump-sum).
3. **Vouching mẫu HĐ → chứng từ:**
   - Hợp đồng / đơn hàng
   - Hóa đơn GTGT / HĐ xuất khẩu
   - Phiếu xuất kho, vận đơn, tờ khai HQ, biên bản nghiệm thu
   - Chứng từ thanh toán (nếu có)
4. **Cut-off test (bắt buộc):**
   - Chọn phiếu xuất kho / biên bản nghiệm thu **trước và sau** ngày khóa sổ (ví dụ ±7–15 ngày).
   - Đảm bảo DT ghi đúng kỳ so với thời điểm chuyển giao rủi ro.
5. **Thủ tục gian lận bổ sung (VSA 240):**
   - Đọc side agreement / email điều khoản trả hàng, hỗ trợ giá.
   - Kiểm tra hàng gửi / bill-and-hold: có yêu cầu bằng văn bản của khách? hàng tách biệt? sẵn sàng giao?
   - Xác nhận điều khoản với khách hàng (không chỉ số dư).
6. **Đối chiếu thuế:** doanh thu kê khai thuế GTGT / TNDN vs sổ 511 (giải thích chênh lệch hợp lý).

### C. Ví dụ cỡ mẫu
| Tổng thể | Cách chọn |
|----------|-----------|
| DT = 500 tỷ; PM = 3 tỷ | 100% HĐ > 3 tỷ; top 20 khách; 60 bút toán tháng 12; 40 bút toán các tháng khác (MUS/ngẫu nhiên) |
| Dịch vụ theo tiến độ | 100% HĐ > PM; mẫu các HĐ còn lại theo % hoàn thành |

## 1.5. Sai sót theo mức độ

| Mức | Ví dụ cụ thể |
|-----|----------------|
| **Cơ bản** | Sai mã hàng, nhầm tỷ giá, cộng sai bảng kê |
| **Thường gặp** | Ghi DT khi mới xuất kho nội bộ; chưa nghiệm thu đã ghi; quên tách thuế; không trừ đúng bản chất giảm trừ vào 521 trước khi lên B02 |
| **Gian lận nâng cao** | **Channel stuffing** (nhồi hàng cho NPP kèm quyền trả lại ngầm); **Round-tripping** (bán qua công ty liên kết rồi mua lại); **Fake invoices**; ghi DT từ hợp đồng chưa có hiệu lực; **Pull-in** doanh thu quý sau; ghi DT từ gia công / nhận ủy thác như hàng tự doanh |

## 1.6. Khắc phục & trọng yếu
- Điều chỉnh giảm DT (+ giảm phải thu / tăng hàng tồn nếu hàng chưa chuyển giao).
- Điều chỉnh đồng thời giá vốn nếu liên quan.
- Thường **vượt ngưỡng trọng yếu** rất nhanh vì DT là chỉ tiêu người dùng quan tâm nhất; ngay cả sai sót < OM nhưng có yếu tố gian lận → xem xét ý kiến ngoại trừ / từ chối và nghĩa vụ thông báo.

---

# 2. Các khoản giảm trừ doanh thu (Mã 02)

## Ý nghĩa
Chiết khấu thương mại, giảm giá hàng bán, hàng bán bị trả lại (TK 521) — dùng để xác định **Doanh thu thuần (10 = 01 − 02)**.

## Thủ tục
- Đối chiếu chính sách CKTM/giảm giá với HĐ và phê duyệt.
- Kiểm tra hàng trả lại sau ngày khóa sổ liên quan DT kỳ trước → sự kiện điều chỉnh (VAS 23 / TT200).
- Đảm bảo không “chôn” giảm trừ vào chi phí bán hàng để làm đẹp DT gộp sai bản chất.

## Gian lận
- Cố ý không ghi nhận giảm trừ / hàng trả lại để giữ DT và LN gộp.
- Đẩy hàng trả lại sang kỳ sau.

---

# 3. Doanh thu thuần (Mã 10) & Giá vốn hàng bán (Mã 11)

## 3.1. Doanh thu thuần (10)
Chỉ tiêu phân tích cốt lõi; mọi sai sót ở 01/02 đều chảy vào đây.

## 3.2. Giá vốn hàng bán (11) — liên kết tồn kho

### Ý nghĩa
Giá trị vốn của hàng đã bán / dịch vụ đã cung cấp trong kỳ; quyết định **LN gộp (20 = 10 − 11)**.

### Assertions: Occurrence (có DT tương ứng), Completeness, Accuracy, Cut-off, Classification.

### Thủ tục
1. Công thức kiểm soát (hàng hóa/thành phẩm):
   ```text
   Giá vốn ≈ Tồn đầu + Nhập trong kỳ − Tồn cuối (± điều chỉnh)
   ```
2. Tính lại giá xuất kho theo đúng phương pháp đã chọn (nhất quán).
3. Đối chiếu với biến động tồn kho đã kiểm toán.
4. Kiểm tra các khoản ghi thẳng vào 632: hao hụt vượt định mức, hàng mất phẩm chất — có phê duyệt không?
5. Phân tích biên LN gộp theo sản phẩm: biến động bất thường → khoan sâu.

### Sai sót / gian lận
| Hướng | Mục đích | Cách làm |
|-------|----------|----------|
| Giảm giá vốn | Tăng LN gộp | Thổi tồn cuối; vốn hóa chi phí vào tồn; không ghi xuất kho |
| Tăng giá vốn | Giảm thuế / “big bath” | Xuất kho khống; dự phòng tồn quá tay; đưa chi phí khác vào 632 |

### Khắc phục
Điều chỉnh 632 ↔ 155/156/155… (tồn kho) hoặc chi phí liên quan; đánh giá ảnh hưởng đến thuế TNDN.

---

# 4. Lợi nhuận gộp (Mã 20)

## Ý nghĩa thẩm định
Chỉ báo sức khỏe kinh doanh cốt lõi. Biên LN gộp thay đổi mạnh mà không giải thích được bằng giá/nguyên liệu/cơ cấu mặt hàng → **dấu hiệu đỏ**.

### Phân tích bắt buộc
- Biên gộp kỳ này vs kỳ trước vs ngành.
- Biên gộp theo tháng: có “đẹp” đột biến quý cuối?
- So với dòng tiền từ HĐKD.

---

# 5. Doanh thu hoạt động tài chính (Mã 21)

## Ý nghĩa
Lãi tiền gửi, lãi cho vay, lãi bán ngoại tệ, cổ tức được chia, lãi bán chứng khoán… (TK 515).

## Thủ tục
- Vouching hợp đồng tiền gửi/cho vay; sao kê lãi.
- Cổ tức: nghị quyết chia tức của bên được đầu tư + tiền về / phải thu.
- Chênh lệch tỷ giá: tính lại mẫu đánh giá cuối kỳ.
- Đảm bảo không đưa nhầm DT bán hàng vào đây (hoặc ngược lại).

## Gian lận
- Ghi nhận cổ tức / lãi chưa được quyền hưởng.
- Tạo lãi ảo từ giao dịch chứng khoán nội bộ / định giá không độc lập.

---

# 6. Chi phí tài chính (Mã 22) & Trong đó lãi vay (Mã 23)

## Ý nghĩa
Lãi vay, lỗ chênh lệch tỷ giá, lỗ bán CK, chiết khấu thanh toán…  
**Mã 23** là thuyết minh/chỉ tiêu trong yếu tố lãi vay — dùng đối chiếu với dư nợ vay.

## Thủ tục
1. Tính lại lãi vay: `Dư nợ bình quân × lãi suất × thời gian`.
2. Đối chiếu thư xác nhận ngân hàng về lãi đã trả / phải trả.
3. Kiểm tra **vốn hóa lãi vay** vào XDCB (242): có đủ điều kiện? ngừng vốn hóa khi tạm dừng kéo dài?
4. Phân bổ chiết khấu/phụ trội trái phiếu.

## Gian lận
- Không ghi nhận đủ lãi vay cuối kỳ (tăng LN).
- Vốn hóa lãi vay vào tài sản không đủ điều kiện (chuyển chi phí thành tài sản).

---

# 7. Chi phí bán hàng (Mã 24) & Chi phí quản lý doanh nghiệp (Mã 25)

## Ý nghĩa
- **24:** tiếp thị, vận chuyển bán hàng, hoa hồng, bảo hành bán hàng…
- **25:** lương khối QP, đồ dùng văn phòng, dự phòng phải thu khó đòi, dịch vụ mua ngoài QL, thuế môn bài…

## Assertions: Completeness (thiếu chi phí), Occurrence (chi phí giả), Cut-off, Classification (đẩy sang trả trước / TSCĐ), Accuracy.

## Thủ tục
1. Phân tích tỷ lệ `24/DT`, `25/DT` theo thời gian.
2. Key items: chi phí lớn, giao dịch bên liên quan, chi phí gần cuối kỳ, chi phí không hóa đơn.
3. Vouching chứng từ: HĐ, nghiệm thu, chứng từ thanh toán, phê duyệt.
4. Kiểm tra phân bổ CCDC, trả trước → đúng kỳ.
5. Đối chiếu quỹ lương, BHXH với 334/338.
6. Rà soát chi phí bị “đẩy” sang 151/261/241/242/211.

## Sai sót / gian lận
| Mức | Ví dụ |
|-----|-------|
| Cơ bản | Sai tài khoản chi phí |
| Thường gặp | Thiếu cut-off chi phí tháng 12; không trích trước |
| Gian lận | Hóa đơn khống tăng chi phí (giảm thuế); hoặc ngược lại giấu chi phí để tăng LN phục vụ vay/IPO; chi hộ cá nhân ghi vào DN |

---

# 8. Lợi nhuận thuần từ HĐKD (Mã 30)

```text
30 = 20 + 21 − 22 − 24 − 25
```
Đánh giá hiệu quả HĐKD cốt lõi trước hoạt động khác. Nếu 30 thấp nhưng 50 cao nhờ thu nhập khác → chất lượng LN yếu.

---

# 9. Thu nhập khác (31) & Chi phí khác (32) → LN khác (40)

## Ý nghĩa
Thanh lý TSCĐ, phạt/bồi thường, nợ khó đòi đã xóa nay thu được… — **không phải** HĐKD thường xuyên.

## Thủ tục thẩm định
- Vouching biên bản thanh lý, HĐ nhượng bán TS.
- Đảm bảo không “nhồi” DT bất thường để đạt KPI mà thiếu thuyết minh.
- Phân tích tỷ trọng `|40|/|50|`: nếu lớn → nhấn mạnh trong đánh giá chất lượng LN.

## Gian lận
- Ghi nhận thu nhập khác ảo từ bán TS cho bên liên quan trên giá.
- Phân loại sai DT bán hàng thành thu nhập khác (hoặc ngược lại) để che xu hướng.

---

# 10. Tổng lợi nhuận kế toán trước thuế (Mã 50)

```text
50 = 30 + 40
```
Chỉ tiêu gốc cho thuế TNDN và điểm xuất phát BCLCTT phương pháp gián tiếp.

**Kiểm soát:** đối chiếu với kết chuyển TK 911 / LN trước thuế trên thuyết minh.

---

# 11. Chi phí thuế TNDN hiện hành (51) & hoãn lại (52)

## Ý nghĩa
- **51:** thuế phải nộp trên LN chịu thuế kỳ này (liên kết tờ khai quyết toán).
- **52:** ảnh hưởng thuế của chênh lệch tạm thời (DTA/DTL – mã 262/341 trên B01).

## Thủ tục
1. Lập bảng **đối chiếu LN trước thuế kế toán → LN chịu thuế**:
   - Chi phí không được trừ
   - Doanh thu miễn thuế
   - Chênh lệch tạm thời vs vĩnh viễn
2. Tính lại thuế theo thuế suất áp dụng / ưu đãi.
3. Đối chiếu 51 với số phát sinh TK 8211 và phải nộp 3334.
4. Kiểm tra cơ sở ghi nhận thuế hoãn lại (khả năng có LN chịu thuế tương lai với DTA).

## Sai sót / gian lận
- Không loại chi phí không hợp lệ → thiếu thuế hiện hành.
- Ghi nhận DTA khi DN lỗ liên tục không có bằng chứng thuyết phục.
- “Che” tranh chấp thuế bằng cách không thuyết minh nợ tiềm tàng.

---

# 12. Lợi nhuận sau thuế TNDN (Mã 60)

```text
60 = 50 − 51 − 52
```
Phải khớp với biến động **421b** trên Bảng CĐKT (sau điều chỉnh phân phối trong kỳ nếu có hạch toán thẳng).

### Kiểm tra chéo bắt buộc
| Từ | Đến | Mục đích |
|----|-----|----------|
| 60 | 421 (LNST chưa phân phối) | Tính liên tục vốn |
| 50 | BCLCTT Mã 01 (PP gián tiếp) | Nhất quán |
| 10, 11 | Biến động 131, 140 | Chất lượng DT & tồn |
| 22/23 | 320/338 & 315 | Đầy đủ lãi vay |

---

# 13. Ma trận dấu hiệu gian lận trên B02

| Dấu hiệu | Khoản mục nghi ngờ | Thủ tục đáp ứng |
|----------|--------------------|-----------------|
| DT tăng mạnh cuối kỳ | 01, 131 | Cut-off + xác nhận điều khoản |
| Biên gộp tăng đột biến | 01, 11, 140 | Kiểm kê + tính lại giá vốn |
| Chi phí QP giảm bất thường | 25, 151, 261 | Search unrecorded expenses |
| Thu nhập khác chiếm tỷ trọng lớn | 31, 40 | Vouching & bên liên quan |
| Thuế suất hiệu lực lệch chuẩn | 51, 52 | Tax bridge |
| LN tăng nhưng tiền KD giảm | toàn B02 ↔ B03 | Phân tích chất lượng LN |

---

# 14. Mẫu phiếu kết luận theo assertion (Doanh thu)

| Assertion | Kết luận (Đạt/Không) | Sai sót (VND) | Đề xuất điều chỉnh |
|-----------|----------------------|---------------|--------------------|
| Occurrence | | | |
| Completeness | | | |
| Accuracy | | | |
| Cut-off | | | |
| Classification | | | |
| Presentation | | | |
| **Tổng ảnh hưởng đến Mã 10 / 50 / 60** | | | |

File tiếp theo: lưu chuyển tiền tệ — công cụ phát hiện “LN đẹp nhưng tiền yếu”.
