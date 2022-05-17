# ADVENTURE CHICKS
*Dự án game cuối kì Lập trình nâng cao INT2215 1* 
--------------------------
Xin chào các bạn, mình tên là Hoàng Mạnh Quân. Trong project này, mình làm về tựa game [Gà con mạo hiểm](https://gunnypc.zing.vn/huong-dan/tieu-hoc/ga-con-mao-hiem.html/) ở trong game Gunny. Ngôn ngữ được sử dụng là [C++](https://vi.wikipedia.org/wiki/C%2B%2B) và sử dụng thư viện đồ họa [SDL2.0](https://www.libsdl.org/).

Mục tiêu của game là đạt được số điểm cao nhất có thể. 3 người đạt được số điểm cao nhất ở mỗi độ khó sẽ được lưu lại.

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
