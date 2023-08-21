## Thư mục Versions: chưa các file .ipynb code thuật toán XGboost và song song hóa thuật toán XGBoost
- Tệp `sequence.ipynb`: chứa toàn bộ code về thuật toán XGBoost được hỗ trợ chính bởi thư viện `numpy`
- Tệp `parralle_v1.ipynb`: chứa toàn bộ code song song hóa về thuật toán XGBoost được hỗ trợ chính bởi thư viện `numba` và `cuda`. Sau khi do thời gian tiến hành xác định những phần có thể song song hóa như 2 hàm find_best_split và similarity của class XGB tree đồng thời 2 hàm residuals và converter của class XGB classifier.
- Tệp `parralle_v2.ipynb`: chứa toàn bộ code song song hóa về thuật toán XGBoost được hỗ trợ chính bởi thư viện `numba` và `cuda`. Tiền hành song song hóa toàn bộ các hàm có trong 2 class XGB tree và XGB classifier
