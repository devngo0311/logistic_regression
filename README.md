Logistic Regression - Bài toán cơ bản trong Machine Learning
1. Giới thiệu
  Trong Machine Learning (ML) thì bài toán phân lớp dữ liệu (Logistic Regression) được xem là một trong những bài toán cơ bản nhất. 
  Đây là kiến thức tôi đã học được và hoàn toàn tự mình xây dựng mô hình nên không tránh khỏi còn những vấn đề chưa hợp lý.
  Logistic Regression là 1 thuật toán phân loại được dùng để gán các đối tượng cho 1 tập hợp giá trị rời rạc (như 0, 1, 2, ...). Một ví dụ điển hình là phân loại Email, gồm có email công việc, email gia đình, email spam, ...
2. Đặt vấn đề
  Bài viết này tôi sẽ xây dựng một mô hình máy học logistic regression để huấn luyện mô hình tôi sử dụng 1 tập dữ liệu về số giờ học và giờ nghỉ của sinh viên, dựa vào đó để đánh giá kết quả học tập của sinh viên là pass hay false.
  Chúng ta cùng quan sát dữ liệu được biểu diễn bằng biểu đồ sau
  
![image](https://user-images.githubusercontent.com/87468563/129730800-6a9558b2-a1c4-4132-be0c-a5d3ff675705.png)

  Về logic thì chúng ta có thể vẽ 1 đường thẳng để phân chia 2 vùng dữ liệu như thế này
  
  ![image](https://user-images.githubusercontent.com/87468563/130008460-ee3a5f14-4b7e-4394-8158-31762ceae858.png)
  
  Nó có thể đúng nhưng còn có những ngoại lệ thì sao, chúng ta cần một mô hình chính xác hơn để dự đoán thay vì 1 đường thẳng như thế
3. Hàm sigmoid
  Bây giờ chúng ta sẽ tìm xác suất của 1 điểm dữ liệu mà nó có thể được chấp nhận, tất nhiên xác suất sẽ nằm trong khoảng từ [0;1]
  Và có 1 hàm số thỏa mãng là hàm sigmoid
  
  ![image](https://user-images.githubusercontent.com/87468563/130008913-75500c96-2b8a-4366-93fb-114542130f57.png)

  
