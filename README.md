# VNTC-Abs

**VNTC-Abs** is a modified version of [**VNTC**](github.com/duyvuleo/VNTC) to be compatible with _Abstractive Summarization_ task.

| type|Train set | Validate set | Test set |
|----|---|---|---|
|Num of docs | 34,503 | 7,422 | 7,364 |
|Avg. Input length | 309 |
|Avg. Target length | 43 |

We use [UETsegmenter](github.com/phongnt570/UETsegmenter) for tokenization.

**Train sample:**
```
INPUT:
theo số_liệu của ngân_hàng nhà_nước , cho vay bằng ngoại_tệ trong năm 2003 tăng đến 34 % so với năm 2002 , trong khi đó lượng tiền gửi chỉ tăng 3,4 % . một quan_chức cao_cấp của ngân_hàng nhà_nước cho_biết nguyên_nhân chính của tình_trạng trên là do lãi_suất ngoại_tệ , chủ_yếu là usd rất cạnh_tranh . hầu_hết các ngân_hàng cho vay usd ngắn_hạn với mức 3 % / năm , trong khi lãi_suất trung_bình cùng kỳ_hạn bằng đồng nội_tệ khoảng 8,5 % / năm . các chuyên_gia cảnh_báo , tăng_trưởng tín_dụng bằng ngoại_tệ quá nhanh có_thể mang lại nhiều rủi_ro cho các ngân_hàng , nhất_là trong bối_cảnh mỹ có_thể tăng lãi_suất cho vay qua đêm bất_cứ lúc_nào . ngân_hàng nhà_nước đề_nghị , nhằm giảm_thiểu rủi_ro , các ngân_hàng phải thực_hiện mua tín_dụng ngoại_tệ có kỳ_hạn

TARGET:
ngân_hàng nhà_nước vừa yêu_cầu các tổ_chức tín_dụng thận_trọng khi cho vay vì thanh khoản ngoại_tệ của nhiều đơn_vị hiện rất mỏng . năm_ngoái , tốc_độ cho vay các loại tiền nước_ngoài đã gấp 10 lần tốc_độ huy_động .
```

**Validate sample:**
```
INPUT:
theo ông trần vĩnh_khâm , chánh_văn_phòng cụm cảng_hàng_không miền nam , khi dự_án hoàn_thành , toàn_bộ khu_vực nhà_ga hiện_tại sẽ chỉ dành cho khách nội_địa . nhà_ga quốc_tế sẽ nằm bên trái ga nội_địa . tổng diện_tích sân_bay lúc đó là 92.000 m2 . ga sân_bay tân_sơn nhất vừa được mở_rộng thêm thành 4.000 m2 . tuy_nhiên , nhiều chuyên_gia hàng_không đánh_giá , trong vài năm tới , ga sẽ quá_tải khi công_suất hoạt_động của các khu_vực như đường cất - hạ_cánh , sân đậu máy_bay ... được nâng lên . việc xây mới nhà_ga quốc_tế nằm trong dự_án vay vốn từ quỹ_tín_dụng đặc_biệt trị_giá 219 triệu usd của nhật bản ký_kết với chính_phủ cuối năm 2002 . ông khâm cũng cho_biết , hiện hai đường cất - hạ_cánh được kéo_dài thêm từ 3.000 lên 3.800 m , đảm_bảo cho máy_bay boeing 747-400 , loại máy_bay dân_dụng lớn nhất thế_giới cất - hạ_cánh . bên cạnh đó , 12 vị_trí đậu máy_bay được làm mới . trang_thiết_bị điều_hành chỉ_huy và phục_vụ gồm ống lồng dẫn khách , quầy cân và băng_chuyền hành_lý vừa được thay_thế bằng máy_móc hiện_đại . riêng hệ_thống rađa có khả_năng bao_quát vùng bán_kính 500 km . sau nhiều lần cơi_nới mở_rộng từ 1990 , diện_tích sân_bay tân_sơn nhất là 32.000 m2

TARGET:
dự_kiến dự_án sẽ được khởi_công vào quý iii năm nay với số vốn đầu_tư 219 triệu usd . nhà_ga mới sẽ nâng tổng công_suất phục_vụ từ 7 triệu lên 15 triệu hành_khách mỗi năm khi đưa vào khai_thác vào cuối năm 2006 .
```
**Test sample:**
```
INPUT:
hiện_trường để lại đêm 18/10 là bàn_ghế , cốc chén ngổn_ngang . 3 thanh_niên bị_thương nặng là : nguyễn đình phước ( 21 tuổi ) , lữ đức lợi ( 19 tuổi ) và đặng_mậu_quốc_tuấn ( 22 tuổi ) , trú ở phường an_khê , quận thanh_khê , đà_nẵng . qua xác_minh điều_tra , vụ_việc đã được làm rõ . chiều 17/10 , bà phạm thị vỹ bị phạm_ngọc thôi , nguyễn_thu , nguyễn trung_trực và nguyễn tấn lộc dùng dao khống_chế cướp 1 sợi dây_chuyền vàng , 2 nhẫn vàng , 1 kiềng đá_quý và 200 nghìn đồng . thôi sau đó yêu_cầu bà vỹ đem 3 triệu đồng chuộc lại số tài_sản này . bà vỹ về kể lại sự_việc cho chồng và con_trai là nguyễn văn mẫn . chiều 18/10 , mẫn rủ hơn chục thanh_niên mang theo tuýp sắt , dao đi tìm thôi và đồng_bọn trả_thù . tìm không được , chúng kéo nhau về nhậu rồi giải_tán , chỉ còn khoảng 7 tên đến quán cà_phê cao_nguyên uống cà_phê . phạm ngọc thôi biết tin mẫn đang truy_lùng hắn cùng đồng_bọn , liền tổ_chức " đánh phủ_đầu " . thôi rủ đám bạn đến tấn_công nhóm của mẫn ở quán cà_phê . phòng cảnh_sát điều_tra tội_phạm về trật_tự xã_hội công_an đà_nẵng đã 6 đối_tượng liên_quan gồm : nguyễn_thu , nguyễn tấn lộc , trần_quang chính , nguyễn trung_trực , nguyễn văn_minh , huỳnh thanh_long . riêng nguyễn minh hải thấy đồng_bọn sa lưới liền ra đầu_thú .

TARGET:
hai taxi đỗ xịch trước quán cà_phê cao_nguyên ( huyện hoà_vang , đà_nẵng ) đang rất đông khách . hơn chục thanh_niên mặt_mày dữ_dằn , lăm_lăm trong tay hung_khí ùa vào quán tấn_công một nhóm khách khoảng 7 người ...
```

```
@misc{vntc-abs,
  author = {Trang-Phuong, N. Nguyen},
  title = {VNTC-Abs},
  year = {2020},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{github.com/trangnnp/VNTC-Abs}},
 }
```
