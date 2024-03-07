# Movie-Recommender-System

## Giai đoạn 1: Giới thiệu
- Đề tài: Xây dựng hệ thống gợi ý phim.
- Ý nghĩa thực tiễn:
  - Cải thiện trải nghiệm giải trí bằng cách cá nhân hóa việc tìm kiếm và khám phá nội dung phim.
  - Tăng sự tương tác và doanh thu cho các nền tảng phân phối phim.
  - Cung cấp thông tin quan trọng về thị trường và sở thích tiêu dùng thông qua phân tích dữ liệu.
  - Hỗ trợ chiến lược tiếp thị và quảng cáo hiệu quả hơn trong ngành công nghiệp giải trí.
- Giới thiệu bộ dữ liệu:
  - TMDB là cơ sở dữ liệu phim toàn diện cung cấp thông tin về phim, bao gồm các chi tiết như tiêu đề, xếp hạng, ngày phát hành, doanh thu, thể loại,...
  - Kích thước tập dữ liệu có 1002798 dòng dữ liệu và 23 cột thuộc tính.
- Link bộ dữ liệu được lấy trên Kaggle: [Xem tại đây](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies)

## Giai đoạn 2: Khai thác thông tin cơ bản của dữ liệu
- Kích thước của dữ liệu
- Ý nghĩa mỗi dòng dữ liệu và cột thuộc tính
- Kiểu dữ liệu hiện tại của mỗi cột là gì? Có cột nào có kiểu dữ liệu không phù hợp không?
- Tình trạng lặp dữ liệu
- Tình trạng khuyết dữ liệu
- Với mỗi cột số, các giá trị được phân bố như thế nào?
- Với mỗi cột phân loại, các giá trị được phân bổ như thế nào?

## Giai đoạn 3: Phân tích khám phá dữ liệu
- Phân tích dữ liệu đơn biến.
- Phân tích dữ liệu hai biến.
- Phân tích dữ liệu đa biến.

## Giai đoạn 4: Xây dựng hệ thống gợi ý phim
- Gợi ý phim dựa trên đánh giá trung bình: Ta sẽ sử dụng weighted rating (điểm đánh giá có trọng số) được tính như sau:
    $$\text{Weighted Rating: }wr = \left(\dfrac{v}{v+m}\times R\right) + \left(\dfrac{m}{v+m}\times C\right)$$
- Gợi ý phim dựa trên mức độ tương đồng với tìm kiếm: Sử dụng trích xuất đặc trưng sử dụng `TF - IDF`.
![](https://drive.google.com/uc?export=view&id=1GJff8U0BBlL9MKYKfnVM8llpdzLViTPm)
