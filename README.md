# Học AI từ số 0

Notebook chạy kèm series video "Học AI từ số 0" trên kênh YouTube [Ngọc Nguyễn Văn](https://www.youtube.com/@ngoc-nguyen-88). Dành cho người làm IT chưa học AI bao giờ: mỗi tập một notebook ngắn, chạy được trên Google Colab miễn phí, không cần cài gì trên máy.

## Các tập

| Tập | Nội dung | Chạy thử |
|---|---|---|
| 1 | AI không được lập trình, nó được dạy bằng ví dụ. Chạy mô hình nhận dạng ảnh đầu tiên (ResNet-18) | [![Mở trong Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ngocnguyen88/AI-from-Zero/blob/main/tap01/tap01.ipynb) |

## Cách chạy

1. Bấm nút "Mở trong Colab" ở tập bạn muốn (cần tài khoản Google).
2. Chọn Runtime > Run all, hoặc chạy từng ô bằng Shift + Enter.
3. Thử đổi ảnh của bạn ở ô 3 và xem mô hình đoán ra gì.

Chạy trên máy riêng: cần Python 3.9 trở lên và `pip install torch torchvision pillow`, rồi mở file `.ipynb` bằng Jupyter hoặc VS Code.

## Nguồn

- Mô hình ResNet-18 và trọng số IMAGENET1K_V1: thư viện torchvision (BSD-3-Clause).
- Ảnh thử: xem `tap01/anh/NGUON.md`.

## Giấy phép

Code và notebook trong repo này theo giấy phép MIT (file `LICENSE`). Ảnh thử theo giấy phép riêng ghi ở `tap01/anh/NGUON.md`.
