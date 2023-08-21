# 2023_LTSS_UD_CLC - Project - Parallelize XGBoost
## Group: 666

## Giới thiệu đồ án 
<b>Mô tả về bài toán</b>: Giải quyết được nhiệm vụ phải xác định và phân loại các loại bệnh khác nhau có trong lá cây, đặc biệt có thể gồm các loại bệnh trên những loại cây khác nhau. Nhiệm vụ chính là tạo ra mô hình phân loại bằng thuật toán XGBoost nhằm phân loại chính xác đối với 38 phân lớp có trong tập dữ liệu, dựa trên hình ảnh lá cây là đầu vào và kết quả trả về là loại bệnh nằm trong 38 phân lớp có sẵn. Thuật toán XGBoost tuần tự được code được hỗ trợ bởi thư viện numpy và phần phát triển song song của nhóm được hỗ trợ bởi thư viện cuda và numba.

## Dataset 
Dữ liệu cho bài toán bao gồm một tập các hình ảnh của các lá cây bị nhiễm bệnh. Mỗi hình ảnh đã được gán nhãn với một trong 38 loại bệnh khác nhau. Mỗi loại bệnh đại diện cho một lớp. Dữ liệu này là cơ sở để huấn luyện và kiểm tra thuật toán nhận dạng bệnh.
- Số lượng phân lớp: 38 (bao gồm các bệnh khác nhau và phân lớp khỏe mạnh).
- Số lượng thực vật: 14 loài và 26 loại bệnh
- Tổng số ảnh: 43456 (tập train) + 10849 (tập test)
- Độ phân giải ảnh: 256 x 256 (dài x rộng)
- Định dạng ảnh: RGB
- Kích thước dataset: 166M (tập test) + 660M (tập train)
- Nguồn: [Kaggle](https://www.kaggle.com/datasets/saroz014/plant-disease), [Kaggle2](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset), [Github](https://github.com/spMohanty/PlantVillage-Dataset/tree/master/raw/color)

## Giới thiệu thành viên
| Student ID  | Student Name    | Github Profile |
| ----------- | -----------     | ----------- |
| 19127132    | Tran Quang Duy  |[tranquangduy0410](https://github.com/tranquangduy0410)|
| 19127328    | Do Quoc Anh     | [Kata-R](https://github.com/Kata-R) |
| 19127332    | Nguyen Nam Anh  |[Manh231](https://github.com/NguyenNamAnh-201)|

## Phân công nhiệm vụ
Nhiệm vụ phân công cho từng thành viên [link](https://docs.google.com/spreadsheets/d/15s2afOR2gVjnIMj73hI5pvIKmiFk8SmJ/edit?usp=sharing&ouid=104020213200031684849&rtpof=true&sd=true).

## Mô tả Github
Phần mô tả về các thư mục cũng như các file mà nhóm đã sử dụng và lưu trữ:
- Thư mục `comparing_models`: chưa các file `.pkl` chưa các thông tin về các mô hình được huấn luyện.
- Thư mục `data_preprocessing`: tiền xử lí dữ liệu, rút trích đặc trưng và xử lí cân bằng dữ liệu.
- Thư mục `models`: chưa các file `.pkl` mô hình đã được nhóm thực hiện huấn luyện.
- Tệp `Final_report.ipynb`:  Bản báo cáo của nhóm về đồ án Song song hóa thuật toán XGBoost cùng với đó là phần so sánh thời gian huấn luyện và độ chính xác của các mô hình khác nhau các parameters.
- Tệp `Proposal.docx`: trình bày về phần tìm hiểu của nhóm trước và sau khi chọn đề tài.
