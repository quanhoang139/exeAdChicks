# Adventure Chicks (Gà con mạo hiểm)
_Hoàng Mạnh Quân - 21020786_
--------------------------
Xin chào các bạn, mình tên là Hoàng Mạnh Quân. Trong project này, mình làm về tựa game [Gà con mạo hiểm](https://gunnypc.zing.vn/huong-dan/tieu-hoc/ga-con-mao-hiem.html) ở trong game [Gunny](https://gunnypc.zing.vn/bianrungxanh). Ngôn ngữ được sử dụng là [C++](https://vi.wikipedia.org/wiki/C%2B%2B) và sử dụng thư viện đồ họa [SDL2.0](https://www.libsdl.org/).

Mục tiêu của game là đạt được số điểm cao nhất có thể. 3 người đạt được số điểm cao nhất ở mỗi độ khó sẽ được lưu lại.

### Hướng dẫn cài đặt:

- Bước 1: Cài đặt SDL2 vào Code Block theo như [Hướng dẫn](https://www.youtube.com/watch?v=kxi0TMXEG3g)
- Bước 2: Tải project game về và mở file Adventure_Chicks.cpb bằng Code Block
- Bước 3: Do trong project đã có sẵn file .dll nên chỉ cần run và chơi game thôi
  
### Mô tả chung:
  Game có cách chơi đơn giản. Nhấn chuột để chọn các tính năng. 
  Chọn các ô để gà con di chuyển đến. Nếu đi vào ô không có bom, bạn sẽ được cộng 1 điểm. Nếu đi vào ô có bom, bạn sẽ phải trả lời câu hỏi. Trả lời đúng sẽ được an toàn, trả lời sai hoặc hết thời gian trả lười sẽ bị trừ 1 mạng.
  Trò chơi kết thúc khi bạn bị trừ hết 2 mạng. 
  
### Các chức năng:
- Video minh họa: [Adventure Chick]
- Chọn độ khó: Độ khó khác nhau thì số lượng bom trên bản đồ sẽ khác nhau.
- Đặt cờ (Set Flag): Dựa vào con số hiển thị trên đầu gà (số lượng bom xung quanh) để tính toán các ô có bom. Việc đặt cờ sẽ giúp đánh dấu lại những ô có bom để không cho gà con đi đến ô đó nữa.
- Hủy cờ (Remove Flag): Với những ô đang có cờ, nếu muốn bỏ cờ để gà con có thể đi vào ô đó thì dùng nút này.
- Dò mìn (Minesweeper): Mở 1 có chứa bom ở xung quanh vị trí hiện tại của gà con mà không phải trả lời câu hỏi hay mất mạng.
- Trả lời câu hỏi: Nhấn vào các ô chứa đáp án A, B, C, D để trọn đáp án. Trả lời sai hoặc hết thời gian đếm ngược nhưng chưa trả lười sẽ bị mất 1 mạng.
- Xem bảng thành tích: Mỗi độ khó sẽ hiển thị top 3 lần chơi có thành tích cao nhất. Thành tích sẽ được bảo toàn kể cả khi thoát game và chạy lại.
- Chức năng tắt nhạc: Khi nhấn vào sẽ dừng phát nhạc nền
- Chức năng tắt hiệu ứng âm thanh: Khi nhấn vào sẽ tắt các âm thanh nhấn nút, click, tiếng bom nổ, ...

### Các kĩ thuật sử dụng:
- Thư viện đồ họa SDL2: Sử dụng hiển thị ảnh, chữ, phát âm thanh.
- Mảng 2 chiều: dùng để lưu trữ trạng thái hiển thị của các ô bom, cỏ, cờ.
- Fps: Đặt fps cố định là 25 khung hình trên giây để cho gà con di chuyển một cách ổn định, dễ nhìn.
- Đọc, in dữ liệu ra file: dùng để lưu trữ dữ liệu thành tích, tránh bị mất mỗi lần chạy game.
- Cấu trúc, lớp: Xây dựng một số cấu trúc để lưu tọa độ (x và y), cấu trúc câu hỏi (bao gồm câu hỏi, các đáp án, đáp án đúng, lựa chọn của người chơi)
- Nạp chồng toán tử để so sánh các tọa độ.
- Chia code thành các file: window (xử lý khởi tạo, đóng SDL, chứa game loop), core (chứa việc xử lý các sự kiện cũng như logic game), Texture (xử lý việc hiển thị ảnh và text), Button (xử lý việc hiển thị các nút, thay đổi trạng thái nút), Sound (xử lý phát, dừng âm thanh game), Time (xử lý vấn đề thời gian cho game).
- Photoshop: Cắt ghép ảnh, tách nhân vật từ ảnh game gốc.

### Kết luận:
Sau khi hoàn thành dự án game cuối kì này, em học được rất nhiều kiến thức và kinh nghiệm, từ tư duy code, kĩ năng chỉnh sửa ảnh cho đến việc lên ý tưởng, quản lý thời gian làm game.

**Điều tâm đắc:**

Những ngày vừa qua, thông tin môn Lịch sử sẽ là môn tự chọn trong Chương trình giáo dục phổ thông mới đã làm dấy lên nhiều tranh cãi.

**Các hướng phát triển trong tương lai:**

- Nâng cao hơn kĩ năng photoshop để có đồ họa đẹp hơn cho game.
- Phát triển các gói câu hỏi phong phú hơn nữa, mở rộng các lĩnh vực khác.

### Đánh giá của mình
*Mục này dành cho thầy cô chấm, các bạn cũng có thể xem*    
  Em (Mình) xin tự đánh giá 9 điểm. 
  Em tự code game này, không có tham khảo ở đâu (em học dùng SDL2.0 qua lazyfoo thôi ạ). Do game này không public asset nên ảnh em chụp màn hình rồi dùng photoshop cắt ra. Âm thanh thì lấy được file giải nén của trò chơi.

### Cách chơi
  Game có cách chơi đơn giản. Dùng chuột di chuyển đến các ô hình mèo, click chuột vào hình mèo để ăn điểm.
  
  Người chơi chỉ ăn điểm khi có từ 2 chú mèo xung quanh cùng màu trở lên. Chi tiết hơn thì mình có làm [video](https://www.youtube.com/watch?v=B4l_B_p_x6M) chơi thử.
  
### Thuật toán của game
  Khi người chơi click chuột thì đầu tiên, mình xác định xem ở đó có phải ô hình mèo không. Sau đó xác định xem người chơi có ăn điểm được không.
  Mình check bằng cách kiểm tra 4 ô xung quanh xem có ô cùng màu không. Nếu tồn tại ít nhất 1 ô cùng màu, mình duyệt BFS cái bảng đó, dùng hàng đợi lưu lại vị trí những ô cùng màu mà có thể xóa được.   
  Sau đó mình cho xóa lần lượt từng ô trong hàng đợi. Sau khi các ô xóa xong, thì mình cho các dòng hạ xuống rồi sau đó cột dồn về bên trái (nếu được).
  
  Để check xem người dùng còn có thể ăn điểm nữa không thì mình duyệt từng cột từ trái sang, duyệt từ dưới lên, nếu thấy 1 ô mà có ít nhất 1 ô xung quanh nó ăn được thì level đó vẫn tiếp tục, còn không thì kiểm tra điểm với mục tiêu.
  
### Đánh giá của mình
*Mục này dành cho thầy cô chấm, các bạn cũng có thể xem*    
  Em (Mình) xin tự đánh giá 9 điểm. 
  Em tự code game này, không có tham khảo ở đâu (em học dùng SDL2.0 qua lazyfoo thôi ạ). Do game này không public asset nên ảnh em chụp màn hình rồi dùng photoshop cắt ra. Âm thanh thì lấy được file giải nén của trò chơi.
