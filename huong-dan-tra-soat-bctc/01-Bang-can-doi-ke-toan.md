# 01 – Bảng cân đối kế toán (Mẫu B01-DN) – Tra soát từng khoản mục

> Căn cứ: Điều 112 Thông tư 200/2014/TT-BTC.  
> Phương trình kiểm soát: **Mã 270 (Tổng TS) = Mã 440 (Tổng nguồn vốn)**.

---

# PHẦN A – TÀI SẢN NGẮN HẠN (Mã 100)

`100 = 110 + 120 + 130 + 140 + 150`

---

## A1. Tiền và các khoản tương đương tiền (Mã 110 = 111 + 112)

### Ý nghĩa
Phản ánh khả năng thanh khoản tức thời: tiền mặt, tiền gửi không kỳ hạn, tiền đang chuyển, và các khoản tương đương tiền (đầu tư ngắn hạn ≤ 3 tháng, dễ chuyển đổi thành tiền, rủi ro thay đổi giá trị không đáng kể).

### Assertions trọng tâm
| Assertion | Mức rủi ro điển hình |
|-----------|----------------------|
| Hiện hữu | Cao (gian lận chiếm dụng tiền) |
| Quyền | Trung bình–Cao (tài khoản phong tỏa, cầm cố) |
| Đầy đủ | Trung bình |
| Đánh giá | Trung bình (ngoại tệ, vàng tiền tệ) |
| Trình bày | Cao (nhầm “tương đương tiền” với đầu tư ngắn hạn) |

### Thủ tục kiểm tra chi tiết
1. **Đối chiếu 3 chiều:** BCTC ↔ sổ cái TK 111/112/113 ↔ bảng tổng hợp chi tiết từng quỹ/từng ngân hàng.
2. **Gửi thư xác nhận ngân hàng** (VSA 505) tới **toàn bộ** ngân hàng đã giao dịch trong kỳ (kể cả số dư = 0 cuối kỳ).
3. **Kiểm quỹ tiền mặt:** bất ngờ (surprise count); đối chiếu biên bản kiểm quỹ cuối kỳ.
4. **Đánh giá lại ngoại tệ** cuối kỳ theo tỷ giá giao dịch thực tế.
5. **Kiểm tra cut-off** séc/ủy nhiệm chi gần ngày khóa sổ.
6. **Rà soát hạn chế sử dụng:** phong tỏa, ký quỹ → phải tách khỏi “Tiền” nếu không thỏa định nghĩa tương đương tiền / thuyết minh hạn chế.
7. **Kiểm tra phân loại tương đương tiền (112):** chứng từ gửi có kỳ hạn ≤ 3 tháng kể từ ngày mua.

### Mẫu kiểm toán & bằng chứng
| Mẫu | Bằng chứng |
|-----|-----------|
| 100% tài khoản ngân hàng | Thư xác nhận ngân hàng (bank confirmation) |
| Toàn bộ quỹ tiền mặt trọng yếu | Biên bản kiểm quỹ có chữ ký Thủ quỹ + Kế toán trưởng + KTV |
| Các bút toán lớn gần cuối kỳ | Ủy nhiệm chi, sao kê, chứng từ thu/chi |
| Khoản ngoại tệ | Bảng tỷ giá NHNN/NH thương mại ngày khóa sổ + tính lại |

### Sai sót
| Mức | Ví dụ |
|-----|-------|
| Cơ bản | Sai số dư do chưa ghi nhận lãi tiền gửi; nhầm quỹ |
| Thường gặp | Đưa tiền gửi 6–12 tháng vào “tương đương tiền”; không đánh giá lại ngoại tệ |
| Gian lận | Kiting (phao tiền giữa 2 ngân hàng); lapping (che chiếm dụng bằng thu của khách sau); tạo sao kê giả; bỏ sót tài khoản phong tỏa |

### Khắc phục & trọng yếu
- Điều chỉnh phân loại 112 ↔ 123; ghi nhận chênh lệch tỷ giá vào DT/CP tài chính.
- Thiếu tiền do chiếm dụng → ghi nhận phải thu/chi phí; đánh giá gian lận (VSA 240) và thông báo Ban quản trị.
- Sai sót tiền thường **nhạy cảm định tính** dù số tiền nhỏ hơn OM (liên quan kiểm soát và trung thực).

---

## A2. Đầu tư tài chính ngắn hạn (Mã 120 = 121 + 122 + 123)

### Ý nghĩa
- **121 Chứng khoán kinh doanh:** nắm giữ để bán lãi ngắn hạn.
- **122 Dự phòng giảm giá CKKD:** điều chỉnh giá trị về giá thị trường thấp hơn.
- **123 Đầu tư nắm giữ đến ngày đáo hạn (ngắn hạn):** TGCK, trái phiếu… kỳ hạn còn lại ≤ 12 tháng (không gồm tương đương tiền).

### Assertions: Hiện hữu, Quyền, Đánh giá, Trình bày (rủi ro cao ở định giá & phân loại).

### Thủ tục
1. Xác nhận với tổ chức lưu ký / ngân hàng / công ty chứng khoán về số lượng sở hữu.
2. Đối chiếu hợp đồng, giấy chứng nhận sở hữu, sao kê custodial.
3. Định giá lại theo giá thị trường đáng tin cậy tại ngày báo cáo; kiểm tra tính dự phòng 122.
4. Kiểm tra ý định & khả năng nắm giữ đến đáo hạn với 123 (không được “taint” danh mục bằng bán sớm hàng loạt).
5. Rà soát lãi/lỗ đã ghi nhận vào 515/635.

### Sai sót / gian lận
- Không trích dự phòng khi giá giảm; dùng giá nội bộ không độc lập.
- Phân loại sai dài hạn ↔ ngắn hạn để làm đẹp thanh khoản.
- Ghi nhận chứng khoán không thuộc sở hữu (repo chưa chuyển rủi ro).

### Khắc phục: điều chỉnh dự phòng; thuyết minh phương pháp định giá; đánh giá ảnh hưởng đến LN trước thuế.

---

## A3. Các khoản phải thu ngắn hạn (Mã 130)

`130 = 131 + 132 + 133 + 134 + 135 + 136 + 137 + 139`  
*(Lưu ý TT200: công thức gốc gồm các mã chi tiết; dự phòng 137 ghi âm)*

### A3.1. Phải thu ngắn hạn của khách hàng (Mã 131) — **KHOẢN MỤC RỦI RO CAO**

#### Ý nghĩa
Quyền thu tiền từ bán hàng/cung cấp dịch vụ đã ghi nhận doanh thu. Liên kết trực tiếp với chất lượng doanh thu.

#### Assertions
| Assertion | Thủ tục chính |
|-----------|---------------|
| Hiện hữu | Thư xác nhận công nợ; vouching hóa đơn + biên bản giao hàng/ nghiệm thu |
| Đầy đủ | Tracing từ biên bản giao hàng chưa lập HĐ |
| Đánh giá | Tuổi nợ + chính sách dự phòng + thu hồi sau ngày khóa sổ |
| Quyền | Factoring / cầm cố phải thu |
| Cut-off (qua DT) | Doanh thu cuối kỳ ↔ hàng xuất kho |

#### Thủ tục kiểm tra chi tiết (checklist)
1. Đối chiếu tổng sổ cái 131 với bảng kê tuổi nợ (aging).
2. **Gửi thư xác nhận** theo mẫu dương tính (positive) với:
   - Các khoản lớn (key items, ví dụ top 20 hoặc mọi khoản > PM)
   - Khoản quá hạn, tranh chấp, bên liên quan
   - Mẫu ngẫu nhiên phần còn lại
3. Với thư không hồi đáp: thủ tục thay thế (subsequent receipts, vận đơn, nghiệm thu, đối chiếu đơn hàng).
4. Kiểm tra thu tiền sau ngày khóa sổ (subsequent collection) → củng cố hiện hữu & đánh giá.
5. Đánh giá dự phòng phải thu khó đòi theo TT 48/2019/TT-BTC (hoặc chính sách DN nếu chặt hơn) và bằng chứng khách hàng mất khả năng thanh toán.
6. Rà soát công nợ âm (khách trả thừa) → có thể trình bày ở phải trả / người mua trả trước.
7. Phân tích tỷ số: `Ngày thu tiền bình quân (DSO)`, biến động phải thu vs doanh thu.

#### Mẫu & bằng chứng
| Mục | Ví dụ |
|-----|-------|
| Key items | 15 khoản lớn nhất = 60% số dư |
| Mẫu | 40 khoản ngẫu nhiên / MUS |
| Bằng chứng | Thư xác nhận; UNC thu tiền sau kỳ; HĐĐT + biên bản giao hàng; email đối chiếu |

#### Sai sót
| Mức | Ví dụ |
|-----|-------|
| Cơ bản | Sai đối tượng, sai số tiền hóa đơn |
| Thường gặp | Không lập dự phòng đủ; không phân loại NH/DH; công nợ đã cấn trừ vẫn treo |
| Gian lận | Phải thu từ doanh thu giả; “bill and hold” không đủ điều kiện; kênh phân phối nhồi hàng (channel stuffing) kèm quyền trả lại ngầm; vòng tròn (round-tripping) với bên liên quan |

#### Khắc phục & trọng yếu
- Điều chỉnh giảm phải thu / doanh thu nếu không thỏa điều kiện ghi nhận.
- Bổ sung dự phòng → tăng chi phí quản lý DN / giảm LN.
- Sai sót dự phòng thường là **judgmental** — ghi rõ khoảng ước tính hợp lý của KTV.

---

### A3.2. Trả trước cho người bán ngắn hạn (Mã 132)

**Ý nghĩa:** Đã trả tiền nhưng chưa nhận hàng/dịch vụ.  
**Rủi ro:** Ứng trước “treo” dài ngày → thực chất đã nhận hàng hoặc mất vốn / thông đồng NCC.

**Thủ tục:** đối chiếu hợp đồng, tiến độ giao hàng, biên bản nhận hàng sau kỳ; xác nhận với NCC; đánh giá khả năng thu hồi / chuyển thành chi phí hoặc phải thu khác nếu dự án hủy.

**Gian lận:** ứng trước cho công ty “ma”, bên liên quan để rút tiền.

---

### A3.3. Phải thu nội bộ ngắn hạn (Mã 133) & dài hạn liên quan

**Ý nghĩa:** Thanh toán nội bộ giữa cấp trên – đơn vị phụ thuộc (ngoài giao vốn).  
**Thủ tục:** đối chiếu 2 chiều; khi lập BCTC tổng hợp phải **bù trừ** với phải trả nội bộ.  
**Sai sót:** không loại trừ giao dịch nội bộ → thổi phồng TS và nợ.

---

### A3.4. Phải thu theo tiến độ HĐ xây dựng (Mã 134)

**Ý nghĩa:** Doanh thu theo tiến độ > số đã lập hóa đơn.  
**Assertions:** Đánh giá % hoàn thành; xảy ra; cắt kỳ.  
**Thủ tục:** nghiệm thu khối lượng; hồ sơ kỹ thuật; đối chiếu điều khoản HĐ; tính lại doanh thu theo VAS 15.  
**Gian lận:** đẩy % hoàn thành để ghi DT sớm.

---

### A3.5. Phải thu về cho vay ngắn hạn (Mã 135)

**Thủ tục:** khế ước vay, lịch trả nợ, xác nhận bên vay, đánh giá tài sản đảm bảo, lãi dự thu, dự phòng.  
**Gian lận:** cho vay bên liên quan không thuyết minh / lãi suất phi thị trường.

---

### A3.6. Phải thu ngắn hạn khác (Mã 136)

Gồm tạm ứng (141), ký cược ký quỹ ngắn hạn, chi hộ, phải thu lãi…  
**Thủ tục:** đối chiếu từng tiểu khoản; kiểm tra tạm ứng quá hạn chưa quyết toán; xác nhận ký quỹ.  
**Sai sót thường gặp:** tạm ứng “treo” nhiều năm để che chi phí / rút tiền.

---

### A3.7. Dự phòng phải thu ngắn hạn khó đòi (Mã 137)

**Ý nghĩa:** Điều chỉnh giảm giá trị phải thu về mức có thể thu hồi.  
**Thủ tục:**  
- Kiểm tra chính sách vs TT 48 (thời gian quá hạn 6–12–24–36 tháng…).  
- Kiểm tra từng khoản lớn đã khởi kiện / phá sản.  
- So sánh dự phòng kỳ này vs kỳ trước và với lịch sử mất nợ thực tế (back-testing).  

**Gian lận:** cố ý **dưới dự phòng** để tăng LN; hoặc **lợi dụng “big bath”** tăng dự phòng năm lỗ để năm sau hoàn nhập.

---

## A4. Hàng tồn kho (Mã 140 = 141 + 149) — **RỦI RO CAO**

### Ý nghĩa
Nguyên vật liệu, công cụ, thành phẩm, hàng hóa, hàng gửi đi bán, chi phí SXKD dở dang ngắn hạn — sau dự phòng giảm giá. Là cầu nối giữa Bảng CĐKT và Giá vốn (632).

### Assertions
Hiện hữu, Đầy đủ, Quyền, Đánh giá (giá gốc & NRV), Cut-off.

### Thủ tục bắt buộc (VSA 501)
1. **Chứng kiến kiểm kê** cuối kỳ (hoặc tại ngày khác + roll-forward/back).
2. Kiểm tra quy trình đếm, thẻ kho, hàng gửi bán / nhận giữ hộ (không được ghi vào tồn kho DN).
3. Test định giá: phương pháp giá gốc (bình quân gia quyền, FIFO…) nhất quán; tính lại một mẫu phiếu xuất.
4. Test NRV: giá bán thuần – chi phí bán; so với giá gốc → dự phòng 149.
5. Cut-off phiếu nhập/xuất ± 5–7 ngày quanh khóa sổ.
6. Phân tích: vòng quay tồn kho, tỷ lệ giá vốn/doanh thu, tồn kho tăng trong khi DT giảm.

### Mẫu & bằng chứng
| Thủ tục | Bằng chứng |
|---------|------------|
| Kiểm kê | Biên bản kiểm kê, phiếu đếm KTV (test counts 2 chiều) |
| Định giá | Phiếu nhập, hóa đơn mua, bảng tính giá thành |
| NRV | Bảng giá bán hiện hành, HĐ bán sau kỳ, hàng lỗi thời |
| Quyền | Hợp đồng cầm cố kho, thư xác nhận hàng gửi |

### Sai sót
| Mức | Ví dụ |
|-----|-------|
| Cơ bản | Sai đơn vị tính, nhầm mã hàng |
| Thường gặp | Không loại hàng đi đường / hàng nhận giữ hộ; không dự phòng hàng chậm luân chuyển |
| Gian lận | Thổi số lượng kiểm kê; tăng giá thành ảo (vốn hóa chi phí kỳ); không ghi xuất kho tương ứng DT; chuyển hàng lỗi thành “tài sản” |

### Khắc phục
Điều chỉnh số lượng/giá trị; bổ sung dự phòng; điều chỉnh đồng thời **Giá vốn** và/hoặc **Doanh thu** nếu liên quan cut-off.  
Ảnh hưởng thường **trực tiếp đến LN gộp** → dễ vượt PM.

---

## A5. Tài sản ngắn hạn khác (Mã 150 = 151 + 152 + 153 + 154 + 155)

| Mã | Khoản mục | Điểm kiểm tra chính |
|----|-----------|---------------------|
| 151 | Chi phí trả trước ngắn hạn | Phân bổ đúng kỳ; chứng từ; không vốn hóa chi phí thuần túy |
| 152 | Thuế GTGT được khấu trừ | Đối chiếu tờ khai thuế; hóa đơn hợp lệ; rủi ro hóa đơn “rác” |
| 153 | Thuế & khoản khác phải thu NSNN | Quyết toán thuế; biên bản hoàn thuế |
| 154 | Giao dịch mua bán lại TPCP | Hợp đồng repo; đúng bản chất |
| 155 | TS ngắn hạn khác | Bản chất kinh tế; khả năng thu hồi |

**Gian lận phổ biến ở 151:** “parking” chi phí vào trả trước để tăng LN kỳ hiện tại.

---

# PHẦN B – TÀI SẢN DÀI HẠN (Mã 200)

`200 = 210 + 220 + 230 + 240 + 250 + 260`

---

## B1. Các khoản phải thu dài hạn (Mã 210)

Tương tự phải thu ngắn hạn nhưng kỳ hạn còn lại > 12 tháng: 211–216, dự phòng 219.  
**Thêm thủ tục:** kiểm tra điều khoản lịch thu; chiết khấu nếu có yếu tố trả chậm trọng yếu; tái phân loại phần đến hạn trong 12 tháng sang ngắn hạn.

---

## B2. Tài sản cố định (Mã 220 = 221 + 224 + 227)

### B2.1. TSCĐ hữu hình (221 = 222 Nguyên giá + 223 Hao mòn lũy kế)

#### Ý nghĩa
Tài sản hữu hình DN nắm giữ để sử dụng > 1 năm, đủ tiêu chuẩn ghi nhận; phản ánh **giá trị còn lại**.

#### Assertions: Hiện hữu, Quyền, Đầy đủ, Đánh giá (nguyên giá & khấu hao), Trình bày.

#### Thủ tục
1. Đối chiếu sổ TSCĐ chi tiết ↔ sổ cái 211/2141.
2. Chọn mẫu tài sản: kiểm tra hiện vật / ảnh hiện trường / biển số / serial.
3. Vouching mua mới: HĐ, hóa đơn, nghiệm thu, quyết định đưa vào sử dụng.
4. Kiểm tra tiêu chuẩn vốn hóa vs chi phí sửa chữa lớn (rủi ro vốn hóa sai để tăng LN).
5. Tính lại khấu hao theo khung thời gian TT 45/2013/TT-BTC (hoặc chính sách DN hợp lý); kiểm tra nhất quán.
6. Kiểm tra thanh lý/nhượng bán: giảm nguyên giá + hao mòn; ghi nhận thu nhập/chi phí khác.
7. Rà soát tài sản thế chấp → thuyết minh.
8. Impairment / không còn sử dụng: đánh giá giảm giá trị còn lại.

#### Sai sót / gian lận
- Vốn hóa chi phí vận hành / sửa chữa thường xuyên.
- Kéo dài thời gian khấu hao bất hợp lý để giảm chi phí.
- Không loại bỏ TSCĐ đã thanh lý / mất mát.
- Ghi nhận TSCĐ khống để tăng quy mô tài sản (phục vụ vay vốn).

---

### B2.2. TSCĐ thuê tài chính (224)

**Kiểm tra:** hợp đồng thuê có chuyển rủi ro/lợi ích? Phân biệt thuê tài chính vs thuê hoạt động; ghi nhận nợ thuê tương ứng; khấu hao đúng.

---

### B2.3. TSCĐ vô hình (227)

**Ví dụ:** quyền sử dụng đất, phần mềm, bằng sáng chế, lợi thế thương mại (trong một số trường hợp phân bổ qua 242).  
**Rủi ro cao:** vốn hóa chi phí R&D / thành lập không đủ điều kiện; không phân bổ; định giá nội bộ thổi phồng.

---

## B3. Bất động sản đầu tư (Mã 230 = 231 + 232)

**Ý nghĩa:** BĐS nắm giữ để cho thuê hoặc chờ tăng giá.  
**Thủ tục:** quyền sở hữu; tách biệt với BĐS hàng hóa (tồn kho) và TSCĐ tự sử dụng; khấu hao phần cho thuê; đánh giá suy giảm với BĐS chờ tăng giá.  
**Gian lận:** phân loại sai để thay đổi khấu hao / thuyết minh giá trị.

---

## B4. Tài sản dở dang dài hạn (Mã 240 = 241 + 242)

| Mã | Nội dung | Rủi ro |
|----|----------|--------|
| 241 | CPSXKD dở dang dài hạn (vd. dự án BĐS chậm) | Không lập dự phòng; che lỗ bằng “dở dang” |
| 242 | XDCB dở dang | Treo mãi không quyết toán; vốn hóa lãi vay sai |

**Thủ tục:** hồ sơ dự án, giấy phép, tiến độ thực tế, khả năng hoàn thành, lãi vay vốn hóa theo chuẩn mực, kiểm tra nghiệm thu từng giai đoạn.

---

## B5. Đầu tư tài chính dài hạn (Mã 250 = 251 + 252 + 253 + 254 + 255)

| Mã | Khoản mục | Trọng tâm kiểm toán |
|----|-----------|---------------------|
| 251 | Đầu tư công ty con | Tỷ lệ sở hữu, quyền kiểm soát, giá gốc, BCTC công ty con |
| 252 | Liên doanh, liên kết | Ảnh hưởng đáng kể; biên bản góp vốn |
| 253 | Góp vốn đơn vị khác | Giấy chứng nhận góp vốn |
| 254 | Dự phòng tổn thất ĐT | Đơn vị nhận đầu tư lỗ / mất vốn |
| 255 | HTM dài hạn | Khả năng nắm giữ; định giá; lãi dự thu |

**Gian lận:** không trích dự phòng khi công ty con lỗ nặng; góp vốn bằng tài sản thổi giá; che giao dịch bên liên quan.

---

## B6. Tài sản dài hạn khác (Mã 260)

| Mã | Khoản mục | Điểm kiểm |
|----|-----------|-----------|
| 261 | Chi phí trả trước dài hạn | Công cụ dụng cụ phân bổ, lợi thế thương mại, chi phí thành lập (nếu còn) — rủi ro “parking” chi phí |
| 262 | Tài sản thuế TNDN hoãn lại | Chênh lệch tạm thời được khấu trừ; khả năng có LN chịu thuế tương lai |
| 263 | Thiết bị, phụ tùng thay thế DH | Tách khỏi tồn kho; dự phòng |
| 268 | TS dài hạn khác | Bản chất & khả năng thu hồi |

**Rủi ro 262:** ghi nhận DTA quá lạc quan khi DN liên tục lỗ → phải có bằng chứng thuyết phục về lợi nhuận tương lai.

---

# PHẦN C – NỢ PHẢI TRẢ (Mã 300 = 310 + 330)

## C1. Nợ ngắn hạn (Mã 310) — các khoản trọng yếu

### C1.1. Phải trả người bán ngắn hạn (311)

**Assertions ưu tiên: Đầy đủ & Cut-off** (rủi ro che giấu nợ để tăng LN).

**Thủ tục:**
1. Đối chiếu sổ 331 với bảng kê NCC.
2. Thư xác nhận NCC (đặc biệt số dư lớn / bất thường / = 0 nhưng giao dịch lớn trong kỳ).
3. **Search for unrecorded liabilities:** hóa đơn về sau ngày khóa sổ, biên bản nhận hàng chưa có HĐ, thư luật sư.
4. Đối chiếu biên bản đối chiếu công nợ cuối năm.

**Gian lận:** cố ý không ghi nhận mua hàng cuối kỳ; giữ hàng ngoài sổ.

---

### C1.2. Người mua trả tiền trước (312)

Liên kết nghĩa vụ giao hàng; kiểm tra HĐ, tiến độ; phần quá hạn dài → đánh giá khả năng ghi nhận doanh thu sai hoặc phải trả lại tiền.

---

### C1.3. Thuế và các khoản phải nộp NSNN (313)

Đối chiếu tờ khai thuế GTGT, TNDN, TNCN, môn bài… với sổ 333; kiểm tra quyết toán; tranh chấp thuế → ước tính dự phòng / thuyết minh nợ tiềm tàng.

---

### C1.4. Phải trả người lao động (314)

Đối chiếu bảng lương, BHXH; kiểm tra quỹ lương tạm tính; rủi ro ghi thiếu lương tháng 12 / thưởng.

---

### C1.5. Chi phí phải trả ngắn hạn (315)

**Rủi ro hai chiều:**  
- Thiếu trích (tăng LN): lãi vay, chi phí điện nước, hoa hồng.  
- Trích thừa / “cookie jar” (giảm LN năm nay để tăng năm sau).

**Thủ tục:** tính lại lãi vay; đối chiếu HĐ; xem nhật ký chứng từ sau kỳ.

---

### C1.6. Doanh thu chưa thực hiện ngắn hạn (318)

Kiểm tra điều kiện phân bổ doanh thu (cho thuê, học phí, bảo trì…); không được ghi DT khi chưa thực hiện nghĩa vụ.

---

### C1.7. Vay và nợ thuê tài chính ngắn hạn (320)

**Thủ tục:**
1. Thư xác nhận ngân hàng / bên cho vay về dư nợ, lãi suất, tài sản đảm bảo, vi phạm covenant.
2. Tái phân loại phần vay dài hạn đến hạn trả trong 12 tháng vào 320.
3. Kiểm tra lãi vay đã ghi đủ (315/635).
4. Thuyết minh hạn mức, tài sản thế chấp.

**Gian lận:** không tái phân loại để làm đẹp hệ số thanh toán hiện hành; che giấu vay ngoài sổ (off-balance) qua hợp đồng hợp tác kinh doanh giả.

---

### C1.8. Dự phòng phải trả ngắn hạn (321)

Bảo hành, tái cơ cấu, hoàn nguyên môi trường, kiện tụng…  
**Kiểm tra:** có nghĩa vụ hiện tại? ước tính tin cậy? (VAS 18 / tương đương).  
**Gian lận:** không lập khi có nghĩa vụ (tăng LN) hoặc lập quá tay (big bath).

---

### C1.9. Các khoản khác thuộc nợ ngắn hạn

| Mã | Khoản mục | Ghi chú kiểm toán |
|----|-----------|-------------------|
| 316 | Phải trả nội bộ NH | Bù trừ khi hợp nhất/tổng hợp |
| 317 | Phải trả theo tiến độ HĐXD | Đối chiếu với doanh thu theo tiến độ |
| 319 | Phải trả NH khác | BHXH, KPCĐ, ký quỹ nhận |
| 322 | Quỹ khen thưởng, phúc lợi | Đúng nguồn trích từ LNST |
| 323 | Quỹ bình ổn giá | Theo quy định ngành |
| 324 | Repo TPCP | Đúng bản chất nợ |

---

## C2. Nợ dài hạn (Mã 330)

Các khoản tương ứng dài hạn: 331–343. Trọng tâm:

| Mã | Khoản mục | Thủ tục then chốt |
|----|-----------|-------------------|
| 338 | Vay & thuê TC dài hạn | Xác nhận; covenant; tái phân loại đến hạn |
| 339 | Trái phiếu chuyển đổi | Tách phần nợ / phần vốn (413) |
| 340 | CP ưu đãi (phân loại nợ) | Nghĩa vụ bắt buộc mua lại |
| 341 | Thuế TNDN hoãn lại phải trả | Chênh lệch tạm thời chịu thuế |
| 342 | Dự phòng phải trả DH | Bảo hành dài hạn, hoàn nguyên |
| 343 | Quỹ PT KH&CN | Đúng chế độ trích/sử dụng |

**Search for unrecorded liabilities** vẫn áp dụng cho nợ dài hạn (đặc biệt cam kết bảo lãnh, kiện tụng).

---

# PHẦN D – VỐN CHỦ SỞ HỮU (Mã 400 = 410 + 430)

## D1. Vốn chủ sở hữu (Mã 410)

| Mã | Khoản mục | Ý nghĩa & kiểm toán |
|----|-----------|---------------------|
| 411 | Vốn góp CSH | Đối chiếu ĐKDN, sổ cổ đông, tiền/tài sản thực góp; 411a/411b với CTCP |
| 412 | Thặng dư vốn CP | Chênh lệch giá phát hành vs mệnh giá; chi phí phát hành |
| 413 | Quyền chọn chuyển đổi TP | Phần vốn của trái phiếu chuyển đổi |
| 414 | Vốn khác của CSH | Nguồn hợp lệ |
| 415 | Cổ phiếu quỹ | Giá trị mua vào; ghi âm |
| 416 | CL đánh giá lại TS | Chỉ khi pháp luật cho phép |
| 417 | CL tỷ giá | Trường hợp đặc thù / chuyển đổi BCTC |
| 418 | Quỹ đầu tư phát triển | Trích từ LNST đúng nghị quyết |
| 419 | Quỹ hỗ trợ SX DN | DNNN sắp xếp lại |
| 420 | Quỹ khác thuộc VCSH | Đúng thẩm quyền |
| 421 | LNST chưa phân phối | **Cầu nối với B02**; 421a + 421b |
| 422 | Nguồn vốn ĐTXDCB | Nguồn đầu tư XDCB |

### Thủ tục chung vốn CSH
1. Lập **bảng biến động vốn CSH** và đối chiếu từng dòng với nghị quyết ĐHĐCĐ/HĐQT.
2. Kiểm tra việc trích quỹ và chia cổ tức: đúng LN có thể phân phối, đúng tỷ lệ.
3. Kiểm tra góp vốn bằng tài sản: biên bản định giá độc lập, chuyển quyền sở hữu.
4. Đối chiếu 421b với LNST trên B02 (sau phân phối trong kỳ nếu có).

### Gian lận liên quan vốn
- Góp vốn “ảo” / rút vốn sau đăng ký.
- Thổi giá tài sản góp vốn.
- Chia cổ tức khi không đủ LN / ảnh hưởng khả năng thanh toán.

---

## D2. Nguồn kinh phí và quỹ khác (Mã 430 = 431 + 432)

Áp dụng DN có kinh phí sự nghiệp / dự án: kiểm tra quyết định cấp, chứng từ chi, quyết toán; TSCĐ hình thành từ nguồn kinh phí.

---

# PHẦN E – KIỂM SOÁT TỔNG HỢP BẢNG CĐKT

1. `270 = 100 + 200` và `440 = 300 + 400` và `270 = 440`.
2. Mọi chỉ tiêu = tổng các chỉ tiêu chi tiết theo công thức TT200.
3. Số đầu năm = số cuối năm trước đã kiểm toán (hoặc thuyết minh điều chỉnh hồi tố).
4. Phân loại NH/DH nhất quán với thuyết minh.
5. Các khoản ghi âm (dự phòng, hao mòn, CP quỹ) đúng hình thức `(…)`.

---

## Ma trận ưu tiên rủi ro trên Bảng CĐKT

| Mức ưu tiên | Khoản mục | Lý do |
|-------------|-----------|-------|
| Rất cao | 131, 140/141, 320/338, 315/321 | Gian lận DT–tồn kho–nợ–ước tính |
| Cao | 110, 220, 242, 251–254, 151/261 | Tiền, TSCĐ, XDCB, đầu tư, trả trước |
| Trung bình | 121–123, 230, 262/341, 411–421 | Định giá, thuế hoãn lại, vốn |
| Theo ngữ cảnh | Nội bộ, HĐXD, repo TPCP | Phụ thuộc mô hình DN |

Chi tiết liên kết sang doanh thu – giá vốn: xem file `02-Bao-cao-KQHDKD.md`.
