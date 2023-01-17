# Cơ sở dữ liệu 

### Chương 1: Khái niệm cơ bản về Cơ sở dữ liệu 

**Khái niệm về CSDL** 

- Khái niệm dữ liệu trong CSDL có thể bao gồm một phạm vi rất rộng các đối tượng: chữ số, văn bản, đồ họa, video.

- Định nghĩa cụ thể hơn của một CSDL bao gồm một tập các đặc tính không tường minh được xem xét cùng nhau để định nghĩa một CSDl.

- CSDL thể hiện các khía cạnh của thế giới thực.

- CSDL được coi là một tập dữ liệu gắn kết logic với nhau. Các dữ liệu ngẫu nhiên không được coi là một CSDL.


**Hệ quản trị CSDL** 

- Hệ quản trị cơ sở dữ liệu (**D**ata**B**ase **M**anagement **S**ystem - **DBMS**) là một hệ thống phần mềm cho phép tạo lập CSDL và điều khiển mọi truy cập đến CSDL đó.


- Đặc điểm: 

    1, Cho phép người dùng tạo CSDL - ngôn ngữ định nghĩa dữ liệu 

    2, Cho phép người dùng truy vấn CSDL - ngôn ngữ thao tác dữ liệ 

    3, Hỗ trợ lưu trữ số lượng lớn dữ liệu 

    4, Kiểm soát truy cập dữ liệu từ nhiều người dùng cùng lúc

**Hệ CSDL** 

Một CSDL được quản lý bởi một hệ quản trị CSDL thường được gọi là một hệ CSDL.

**Tổng quan các thành phần của một hệ CSDl** 

![m](https://github.com/Toeeeee/CSDL_PTIT/blob/main/Images/Screenshot%202022-12-23%20111549.png?raw=true)


**Kiến trúc hệ quản trị CSDL** 

![m](http://www.hocvienmang.com/newsimage/original/2017/08/image_695_02_KienTrucHeQuanTriCSDL.PNG)


**Mô hình trừu tượng 3 lớp** 

![m](https://github.com/Toeeeee/CSDL_PTIT/blob/main/Images/Screenshot%20from%202022-12-23%2017-56-54.png?raw=true)

**Mức ngoài**

- Là khung nhìn của người sử dụng CSDL, mô tả phần CSDL tương ứng với người dùng đó.

- Mỗi người dùng có một khung nhìn khác nhau về thế giới thực

- Mức ngoài chỉ bao gồm các thực thể, thuộc tính, quan hệ trong thế giới thực mà người dùng quan tâm

**Mức khái niệm** 


- Mức khái niệm là khung nhìn của người thiết kế CSDL, mô tả dữ liệu nào được lưu trong CSDL và mối quan hệ giữa chúng 

- Người quản trị CSDL nhìn thấy toàn bộ cấu trúc logic của CSDL. 

**Mức trong** 

- Mức trong biểu diễn về mặt vật lý của CSDL trong máy tính, mô tả các thức lưu trữ dữ liệu trong CSDL


![m](https://github.com/Toeeeee/CSDL_PTIT/blob/main/Images/Screenshot%20from%202022-12-23%2018-05-54.png?raw=true)

**Các ngôn ngữ CSDL** 

- Ngôn ngữ định nghĩa dữ liệu 
- Ngôn ngữ thao tác dữ liệu 

**Ngôn ngữ định nghĩa dữ liệu** 
- Là ngôn ngữ cho phép người quản lý CSDL hoặc người dùng mô tả và đặt tên các thực thể, thuộc tính và các quan hệ cần thiết cho ứng dụng, cùng với những ràng buộc về bảo mật và toàn vẹn liên quan.

**Ngôn ngữ thao tác dữ liệu** 

- Là ngôn ngữ cung cấp một tập các thao tác hỗ trợ cho các phép toán thao tác dữ liệu cơ bản trên dữ liệu được lưu trong CSDL

- Bao gồm: 

    1, Chèn dữ liệu vào CSDL mới 

    2, Sử dổi dữ liệu đã được lưu trữ trong CSDL

    3, Lấy dữ liệu từ CSDL 

    4, Xóa dữ liệu trong CSDL

- Phần thao tác lấy dữ liệu gọi là ngôn ngữ truy vấn 

**Phân loại các hệ CSDL** 

Có 2 loại kiến trúc 

- Hệ CSDL tập trung 
    - Hệ CSDL cá nhân 
    - Hệ CSDL trung tâm
    - Hệ CSDL client/ server

- Hệ CSDL phân tán 
    - Hệ CSDl phân tán thuần nhất 
    - Hệ CSDL phân tán không thuần nhất 



**Hệ CSDL tập trung** 

- Là các hệ CSDL mà trong đó phần CSDL được lưu trữ tại một ví trí nhất định 

**Hệ CSDL phân tán** 


- CSDL phân tán là một CSDl logic đơn lẻ được trải ra về amwjt vật lý trên nhiều máy tính ở nhiều vị trí địa lý khác nhau

VD: CSDL của một ngân hàng sẽ được phân bổ theo các chi nhánh tại từng địa phương

### Chương 2: Các mô hình dữ liệu 

**Mô hình dữ liệu** 

- Là một tập hợp các khái niệm dùng cho việc mô tả và thao tác dữ liệu, các mối quan hệ và các ràng buộc trên dữ liệu tổ chức 

- 3 loại chính: 
    - Hướng đối tượng 
    - Hướng bản ghi 
    - Vật lý 

- Có 3 mô hình hướng bản ghi cơ bản:
    - Mô hình dữ liệu quan hệ 
    - Mô hình dữ liệu mạng 
    - Mô hình dữ liệu phân cấp 
    
- 6 bước thiết kế cơ sở dữ liệu: 
    - Phân tích yêu cầu 
    - Thiết kế CSDL mức khái niệm
    - Thiết kế CSDL mứn logic 
    - Cái tiến lược đồ 
    - Thiết kế CSDL mức vật lý 
    - Thiết kế an toàn bảo mật 
    
 
### Chương 3: Ngôn ngữ truy vấn đại số quan hệ 

- Năm phép toán cơ bản trong đại số quan hệ: phép chọn, phép chiếu, phép hợp, phép trừ, phép tích Đề-các

- Một số phép toán mở rộng: phép giao, phép kết nối tự nhiên, phép chia, phép bán kết nối, phép kết nối ngoài.


