# Large-Scale NLP Pipeline for Legal Document Analysis

## 📋 Mô Tả Dự Án

Dự án xây dựng hệ thống xử lý ngôn ngữ tự nhiên (NLP) quy mô lớn cho phân tích văn bản pháp luật Việt Nam. Dự án sử dụng dataset chứa **498,938 tài liệu pháp luật** để thực hiện các nhiệm vụ phân tích và phân loại toàn diện.

## 🎯 Mục Tiêu Chính

1. **Khám Phá Dữ Liệu (EDA)** - Phân tích chi tiết dataset lớn
2. **Tiền Xử Lý Dữ Liệu** - Pipeline xử lý hiệu quả với batch processing
3. **Phân Loại Văn Bản** - So sánh 2 phương pháp:
   - Machine Learning truyền thống (TF-IDF + Logistic Regression)
   - Deep Learning (CNN + LSTM + Embeddings)
4. **Phân Tích Chiều Sâu Văn Bản Pháp Luật**:
   - Trích xuất cấu trúc pháp lý (điều, khoản, mục)
   - Phân tích chủ đề (Topic Modeling với LDA)
   - Tìm kiếm văn bản tương tự (Document Similarity)
   - Trích xuất từ khóa pháp lý
5. **Đánh Giá Hiệu Năng** - Đo lường throughput, memory, scalability

## 📊 Cấu Trúc Notebook

### 📖 Phần 1: Khám Phá Dữ Liệu (EDA)
- Tải và kiểm tra dataset
- Phân tích phân bố các loại tài liệu
- Phân tích độ dài văn bản
- Phân tích từ vựng và đặc trưng ngôn ngữ
- Trực quan hóa dữ liệu

### 🔧 Phần 2: Tiền Xử Lý Dữ Liệu
- Làm sạch văn bản
- Tách từ tiếng Việt (word tokenization)
- Xử lý dữ liệu mất mát
- Chuẩn hóa dữ liệu

### 🤖 Phần 3: Phân Loại Machine Learning
- **TF-IDF Vectorization**: Chuyển đổi văn bản thành vector số
- **Logistic Regression**: Mô hình phân loại
- Đánh giá: accuracy, precision, recall, F1-score
- Confusion Matrix

### 🧠 Phần 4: Phân Loại Deep Learning
- **Word Embeddings**: Chuyển đổi từ thành vector
- **CNN/LSTM**: Extracting cấu trúc văn bản
- **Bidirectional LSTM**: Xử lý văn bản hai chiều
- Early Stopping & Learning Rate Reduction
- Đánh giá mô hình

### 📈 Phần 5: Phân Tích Chủ Đề (Topic Modeling)
- Latent Dirichlet Allocation (LDA)
- Khám phá các chủ đề chính trong văn bản pháp luật

### 🔍 Phần 6: Phân Tích Tương Tự & Trích Xuất Từ Khóa
- Dùng Cosine Similarity tìm văn bản tương tự
- Trích xuất từ khóa quan trọng
- Phân tích tần số từ

### 📊 Phần 7: Đánh Giá Hiệu Năng
- So sánh TF-IDF vs Deep Learning
- Phân tích throughput, memory usage
- Khảo sát độ chính xác vs tốc độ

## 🛠 Các Thư Viện Sử Dụng

### Xử Lý Dữ Liệu
- `pandas` - Xử lý dữ liệu bảng
- `numpy` - Tính toán số học

### Xử Lý Tiếng Việt
- `underthesea` - Tách từ tiếng Việt

### Machine Learning & Deep Learning
- `scikit-learn` - ML truyền thống
- `tensorflow` & `keras` - Deep Learning

### Trực Quan Hóa
- `matplotlib` & `seaborn` - Biểu đồ
- `wordcloud` - Word cloud

## 📋 Yêu Cầu Hệ Thống

```bash
# Cài đặt các thư viện
pip install pandas numpy matplotlib seaborn scikit-learn
pip install tensorflow
pip install underthesea
pip install wordcloud
pip install tqdm
```

## 🚀 Cách Chạy

1. **Chuẩn bị dữ liệu**: Đặt file CSV chứa dữ liệu pháp luật
2. **Mở notebook**:
   ```bash
   jupyter notebook Nhom37_Cuoiky_Bigdata25.ipynb
   ```
3. **Chạy từng cell** theo thứ tự từ trên xuống dưới

## 💡 Điểm Nổi Bật

✅ **Xử lý dữ liệu quy mô lớn** - 498,938 tài liệu  
✅ **So sánh 2 phương pháp** - ML vs Deep Learning  
✅ **Phân tích toàn diện** - Topic modeling, similarity, keyword extraction  
✅ **Tối ưu bộ nhớ** - Garbage collection, batch processing  
✅ **Code dễ hiểu** - Có comment tiếng Việt chi tiết  

## 📊 Kết Quả Dự Kiến

- **Phân loại chính xác**: > 85% accuracy
- **Xử lý hiệu quả**: Hàng chục nghìn tài liệu/phút
- **Memory optimization**: RAM tối ưu cho dữ liệu lớn

## 👥 Người Tạo

**Nhóm 37** - Bài tập cuối kỳ môn Big Data 2025

## 📝 Lưu Ý

- Notebook này được tạo cho Kaggle environment
- Yêu cầu dataset: `top5_documents.csv`
- Mỗi cell có thể chạy độc lập (ngoại trừ các cell phụ thuộc)

## 🎓 Kiến Thức Áp Dụng

- Xử lý ngôn ngữ tự nhiên (NLP)
- Machine Learning & Deep Learning
- Big Data processing
- Data visualization
- Vietnamese language processing

---

**Thời gian cập nhật cuối**: April 2026
