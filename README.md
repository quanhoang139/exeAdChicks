# Adventure Chicks (Gà con mạo hiểm)
_Hoàng Mạnh Quân - 21020786_
--------------------------
Xin chào các bạn, mình tên là Hoàng Mạnh Quân. Trong project này, mình làm về tựa game [Gà con mạo hiểm](https://gunnypc.zing.vn/huong-dan/tieu-hoc/ga-con-mao-hiem.html) ở trong game Gunny. Ngôn ngữ được sử dụng là [C++](https://vi.wikipedia.org/wiki/C%2B%2B) và sử dụng thư viện đồ họa [SDL2.0](https://www.libsdl.org/).

Mục tiêu của game là đạt được số điểm cao nhất có thể. 3 người đạt được số điểm cao nhất ở mỗi độ khó sẽ được lưu lại.

### Hướng dẫn cài đặt:

- Bước 1: Cài đặt SDL2 vào Code Block theo như [Hướng dẫn](https://www.youtube.com/watch?v=kxi0TMXEG3g)
- Bước 2: Tải project game về và mở file Adventure_Chicks.cpb bằng Code Block
- Bước 3: Do trong project đã có sẵn file .dll nên chỉ cần run và chơi game thôi
  
### Mô tả chung:
  Game có cách chơi đơn giản. Nhấn chuột để chọn các tính năng. 
  Chọn các ô để gà con di chuyển đến. Nếu đi vào ô không có bom, bạn sẽ được cộng 1 điểm. Nếu đi vào ô có bom, bạn sẽ phải trả lời câu hỏi. Trả lời đúng sẽ được an toàn, trả lười sai hoặc hết thời gian trả lười sẽ bị trừ 1 mạng.
  Trò chơi kết thúc khi bạn bị trừ hết 2 mạng. 
  
### Các chức năng:

### Các kì thuật sử dụng:
- Mảng 2 chiều: dùng để lưu trữ trạng thái hiển thị của các ô bom, cỏ, cờ.
- Đọc, in dữ liệu ra file: dùng để lưu trữ dữ liệu thành tích, tránh bị mất mỗi lần chạy game.
- 
### Kết luận:


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
