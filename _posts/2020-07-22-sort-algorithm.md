---
layout: post
title: Thuật toán sắp xếp
tags: [thuật toán, sắp xết, sort]
---
Trong thực tế, bạn sẽ gặp rất nhiều bài toán thống kê với một danh sách khủng. Cụ thể như bạn muốn sắp xếp số lượng thành viên trong 1 gia đình của cả một thành phố. Hay đơn giản hơn, bạn muốn tìm ra người cao điểm nhât lớp/trường hay là bạn muốn xếp thứ tự kết quả hoc tập trừ trên xuống dưới, từ cao xuống thấp, bạn muốn danh sách lớp theo thứ tự alpha cho thuận tiện trong việc kiểm soát.

![mình hoạ lời giải Thuật toán sắp xếp](https://i.ibb.co/LQ1zCk1/1-Tf-ZROec-pj-08h-BXKho-UZA.png"thuật toán sắp xếp")

Vậy để thực hiện tốt những quá trình trên thì trước tiên bạn cần làm gì. Đó chính là ***sắp xếp*** danh sách đó theo ý muốn riêng của chính bản thân. Thế thuật toán sắp xếp nó được ứng dụng như thế nào? độ phức tạp của mỗi thuật toán sắp xếp là bao nhiêu? nó có ich trong việc học thuật toán của bạn như thế nào?. Bài viết hôm nay sẽ giải đáp những vấn đề đó.

### Bài toán minh hoạ

Cho bạn một danh danh sách lớp học chứa điểm tổng kết của các thành viên trong lớp. Yêu cầm bạn hãy tìm học sinh mà có điểm tổng kết cao nhất lớp.

### Ý tưởng
Bài này có rất nhiều cách để tiếp cận và tìm được nhiều cách giải khác nhau, tuy nhiên mỗi cách đều có ưu điểm và nhược điểm riêng biệt của nó.

* Cách đầu tiên, cách đơn giản nhất mà chúng ta nghĩ ngay đầu tiên trong đầu là lấy một học sinh bất kì trong lớp  rồi so sánh với các học sinh còn lại. Nếu có bạn có điểm lớn hơn thì ta lại lấy bạn có điểm lớn hơn đó và tiếp tục đi so sánh cho đến kết thúc danh sách lớp và ta sẽ tìm được học sinh có số điểm tổng kết cao nhất lớp.

* Cách thứ hai, chúng ta có thể chia học sinh theo từng nhóm (tổ), rồi lấy học sinh cao nhất của các nhóm tiếp tục so sánh với nhau thì chúng ta cũng sẽ tìm được người có điểm tổng kết cao nhất lớp.

Vậy khi làm bài ta nên sử dụng thuật toán nào? Thuật toán nào khi chạy sẽ tốt hơn, tối ưu hơn?

### Muốn biết được thuật toán nào tốt hơn và tối ưu hơn thì ta nên quan tâm các yêu tố sau:

* Thời gian chạy: Đối với một số bài có dữ liệu cực kì lớn, thì sẽ có một số thuật toán chạy cực kì chậm và không đáp ứng được yêu cầu của đề ra nên không được áp dụng vào thực tế.
* Bộ nhớ: Khi chạy các chương trình thì nó sẽ tự động tạo ra các bộ nhớ để lưu trữ diệu, vậy thuật toán tối ưu là thuật toán sử dụng ít bộ nhớ nhất.
### Phân loại thuật toán sắp xếp

#### Sắp xếp ổn định
Một thuật toán sắp xếp được gọi là sắp xếp ổn định nếu sau khi tiến hành sắp xếp vị trí tương đối giữa các phần tử bằng nhau không bị thay đổi.

#### Sắp xếp so sánh
Một thuật toán sắp xếp được gọi là sắp xếp so sánh nếu trong quá trình thực hiện thuật toán ta tiến hành so sánh các khoá và đổi chỗ các phần tử cho nhau. Đa số các thuật toán sắp xếp dưới đây là sắp xếp so sánh, riêng sắp xếp đếm phân phối không phải là sắp xếp so sánh.

### Ứng dụng

* Tìm người có điểm cao nhất lớp/trường ....
* Sắp xếp một danh sách tên các học viên theo bảng chữ cái alpha 
* Sắp xếp một mảng theo thứ tự giảm dần, tăng dần.
* Sắp xếp và xử lí các số liệu khủng trong thực tế.


Tuỳ vào mỗi bài, dữ liệu đầu vào và thời gian chạy ta chọn thuật toán phù hợp.




