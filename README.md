# Bài tập giữa kỳ – So sánh biểu diễn VAE, ViT, V-JEPA

## Nội dung
- `BT_GIUA_KY.ipynb`: notebook bài làm (đã chạy sẵn, có đủ hình và kết quả).
- `outputs/`: embedding và kết quả đã tính, để chạy lại nhanh.
- `requirements.txt`: các thư viện cần cài.

## Cách chạy lại
1. Cài thư viện:
   ```
   pip install torch torchvision --index-url https://download.pytorch.org/whl/cu126
   pip install -r requirements.txt
   ```
   Trên Google Colab chỉ cần bỏ dấu `#` ở ô cài đặt đầu notebook.
2. Mở `BT_GIUA_KY.ipynb` và chạy tất cả (Run All).

Ghi chú:
- Cần GPU NVIDIA (em chạy trên RTX A2000 8GB, Google Colab với GPU T4 cũng chạy được).
- Lần đầu notebook tự tải 3 mô hình (khoảng 2GB) và dữ liệu (CIFAR-10, UCF101-subset) từ HuggingFace, nên cần có mạng.
- Có sẵn thư mục `outputs/` thì chạy khoảng 5 phút. Muốn tính lại toàn bộ thì đặt `USE_CACHE = False` trong ô cấu hình, mất khoảng 30–40 phút.
