# (Bài Tập Tổng Hợp) Tech Lead của Cyber Arena
## Phần 1 – Lĩnh vực CNTT và đơn vị lưu trữ
1.  Ngân sách chỉ đủ tuyển 1 người. Bạn chọn ứng viên nào? Nêu lựa chọn và giải thích trong 2–3 câu, dựa trên nhu cầu thực tế của ***Cyber Arena***.
  -->Em chọn ứng viên B: giỏi lắp ráp, sửa máy tính và cài đặt mạng (lĩnh vực ***Mạng máy tính / Quản trị hệ thống***).
 Lí do: + Cyber Arena cần máy tính hoạt động ổn định, mạng livestream tốt.
              +Nếu giỏi lắp ráp, sửa máy tính thì dĩ nhiên về phần lập trình cũng sẽ giỏi, đáp ứng được yêu cầu phụ trách kĩ thuật và cũng như thiết kế hệ thống quay và xem. Nâng cấp máy tính cho giai đoạn sau này tốt hơn. 
2.  Sắp xếp các đơn vị sau theo thứ tự **tăng dần**: `GB`, `Byte`, `TB`, `KB`, `MB`
Trả lời: ``Byte < KB < MB < GB < TB``
    

## Phần 2 – Mô hình IPO và lĩnh vực CNTT
1.  **Hệ thống quay lại** và **xem lại trận đấu** hoạt động theo **_mô hình IPO_**, kèm một nơi lưu trữ. Điền vào bảng, mỗi ô 1 ý ngắn:
    
|Thành phần  |Trong hệ thống quay/xem lại trận đấu
|:--- | :---| 
|Input | Hình ảnh và âm thanh trận đấu |
|Process | Máy tính xử lý và mã hóa video, 
|Output| Video trận đấu để xem lại, chất lượng video tốt, rõ nét 
|Storage|SSD lưu trữ video

2.  Hoạt động của **Cyber Arena** (livestream, quay video, xem lại phân tích) gắn với lĩnh vực CNTT nào đã được học ? (Chọn 1-2 lĩnh vực và mỗi lĩnh vực giải thích 1 câu)  
 -   Mạng máy tính / Quản trị hệ thống: Đảm bảo kết nối mạng ổn định để livestream trận đấu lên YouTube.
-   Kỹ thuật phần mềm: Có thể phát triển phần mềm quản lý video và hỗ trợ huấn luyện viên xem lại trận đấu.
## Phần 3 –Tính toán dung lượng và tốc độ mạng

1.  **Tính dung lượng lưu trữ:**
    -   20 trận × 500 MB = 10.000MB
    -   Đổi kết quả sang GB: Lấy 10.000GB : 1024= 9.765625GB
    -   SSD 512 GB có chứa đủ video của 1 tháng 
    - Sau 1 tháng đầu tiên vận hành còn trống ``502.234GB``GB (Bỏ qua dung lượng hệ điều hành và game.)
2.  **Tính tốc độ mạng:**
    
    -   Mạng 100 Mbps tương đương tối đa 12.5 MB/s (Lấy 100Bps : 8)
    -   Với tốc độ đó, tải lên (upload) 1 đoạn video 200 MB mất tối thiểu 16 giây (Lấy 200 MB: 12.5MB/s)
    -   Thực tế thường lâu hơn con số tính được vì tốc độ upload thực tế có thể thấp hơn 100 Mbps do đường truyền không ổn định hoặc lưu lượng mạng tăng cao.
        
## Phần 4 –Phần cứng và mô hình DIKW
1.  Máy bị giật khi vừa **chơi game** vừa **quay video livestream**. Bạn sẽ nâng cấp **RAM** hay **CPU** để giải quyết vấn đề này ? Chọn 1 và giải thích 2–3 câu dựa trên vai trò của từng thành phần.
   `Trả lời`:  Chọn CPU vì vừa chơi game vừa livestream khiến CPU phải xử lý nhiều tác vụ cùng lúc. CPU mạnh hơn có thể giúp xử lý game và mã hóa video tốt hơn, giảm tình trạng giật nếu CPU đang là điểm nghẽn của hệ thống.
2.  Áp mô hình **DIKW** vào 1 tình huống: "Huấn luyện viên xem video thấy tuyển thủ hay chết ở phút 15-20, phát hiện do thiếu tầm nhìn bản đồ, nên yêu cầu mua thêm mắt (Ward) cho trận sau." Đâu là Data, Information, Knowledge, Wisdom trong câu trên?

| Tầng | Nội dung trong tình huống | Vì sao thuộc tầng này? |
|---|---|---|
| Data | Tuyển thủ thường chết ở phút 15–20. | Đây là dữ liệu quan sát được từ các trận đấu. |
| Information | Video cho thấy tuyển thủ thiếu tầm nhìn bản đồ. | Dữ liệu được phân tích để xác định vấn đề. |
| Knowledge | Thiếu tầm nhìn bản đồ làm tuyển thủ dễ bị đối phương tấn công. | Đây là sự hiểu biết về nguyên nhân của vấn đề. |
| Wisdom | Huấn luyện viên yêu cầu mua thêm mắt (Ward) cho trận sau. | Đây là quyết định hành động dựa trên kiến thức đã có. |
