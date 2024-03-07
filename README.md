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
- Gợi ý phim dựa trên đánh giá trung bình: Ta sẽ sử dụng weighted rating (điểm đánh giá có trọng số):
  - Gợi ý phim hay nhất mọi thời đại:
  
  ![](https://drive.google.com/uc?export=view&id=1M-oKO6Xd0YKK6sJ2_-fOyrhRfBBguRPq)
  
  - Gợi ý phim hay nhất trong năm 2019:
  
  ![](https://drive.google.com/uc?export=view&id=1NHye7NJvY5wqecz4T8ChZm_Tqh_Py096)
  
  - Gợi ý phim hay nhất mọi thời đại của đất nước Thái Lan:
  
  ![](https://drive.google.com/uc?export=view&id=1kxot0me71_oOSa2WM4QsCt8rcl8RBwO4)
  
- Gợi ý phim dựa trên mức độ tương đồng với tìm kiếm: Sử dụng trích xuất đặc trưng sử dụng `TF - IDF`:
  - Phim tìm kiếm:
    
  ![](https://drive.google.com/uc?export=view&id=1lN53KU5EsYrc7E1qAKO3VQTQOCcNLr5_)
  
  - Những phim gợi ý:
    
  ![](https://drive.google.com/uc?export=view&id=1EEmRguhqZ08_10Y9Ho6WW1jywXWZoGMx)
  
