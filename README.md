# Machine Learning Project: Diabetes Prediction 🩺

Dự án machine learning để dự đoán khả năng mắc bệnh tiểu đường dựa trên các thông số y tế của bệnh nhân.

## 📋 Mô tả dự án

Dự án này sử dụng các thuật toán machine learning để phân tích và dự đoán khả năng mắc bệnh tiểu đường dựa trên bộ dữ liệu Pima Indian Diabetes. Mục tiêu là xây dựng một mô hình có độ chính xác cao để hỗ trợ chẩn đoán sớm bệnh tiểu đường.

## 🗂️ Cấu trúc dự án

```
Machine_learning_Project_diabetes_data/
├── classifier.py          # File chính chứa code phân tích và training model
├── diabetes.csv          # Bộ dữ liệu diabetes
└── README.md            # File hướng dẫn này
```

## 📊 Dataset

Bộ dữ liệu sử dụng là **Pima Indian Diabetes Dataset** bao gồm các thuộc tính:

- **Pregnancies**: Số lần mang thai
- **Glucose**: Nồng độ glucose trong máu
- **BloodPressure**: Huyết áp tâm trương
- **SkinThickness**: Độ dày nếp gấp da
- **Insulin**: Nồng độ insulin
- **BMI**: Chỉ số khối cơ thể
- **DiabetesPedigreeFunction**: Hàm di truyền tiểu đường
- **Age**: Tuổi
- **Outcome**: Kết quả (0: không mắc, 1: mắc tiểu đường)

## 🔧 Công nghệ sử dụng

- **Python**: Ngôn ngữ lập trình chính
- **Pandas**: Xử lý và phân tích dữ liệu
- **Scikit-learn**: Thư viện machine learning
- **YData Profiling**: Tạo báo cáo phân tích dữ liệu
- **LazyPredict**: So sánh hiệu suất của nhiều mô hình ML

### Các thuật toán được sử dụng:
- Support Vector Machine (SVM)
- Logistic Regression
- Random Forest Classifier
- Và nhiều mô hình khác qua LazyClassifier

## 🚀 Cài đặt và chạy

### Yêu cầu hệ thống
```bash
pip install pandas
pip install scikit-learn
pip install ydata-profiling
pip install lazypredict
```

### Chạy dự án
```bash
python classifier.py
```

## 📈 Quy trình phân tích

1. **Tải và khám phá dữ liệu**: Sử dụng pandas để đọc file CSV
2. **EDA (Exploratory Data Analysis)**: Tạo báo cáo chi tiết với YData Profiling
3. **Tiền xử lý dữ liệu**: 
   - Chia dữ liệu train/test (80/20)
   - Chuẩn hóa dữ liệu (StandardScaler)
4. **Training mô hình**: 
   - Random Forest Classifier
   - Grid Search để tối ưu hyperparameters
   - So sánh nhiều mô hình với LazyClassifier
5. **Đánh giá mô hình**: Sử dụng classification report

## 📊 Kết quả

Dự án sử dụng LazyClassifier để so sánh hiệu suất của nhiều thuật toán machine learning khác nhau và chọn ra mô hình tốt nhất dựa trên các metrics như accuracy, precision, recall và f1-score.

## 🔍 Tính năng chính

- ✅ Phân tích dữ liệu tự động với YData Profiling
- ✅ So sánh nhiều mô hình ML cùng lúc
- ✅ Tối ưu hyperparameters với Grid Search
- ✅ Báo cáo hiệu suất chi tiết
- ✅ Code được tổ chức rõ ràng và dễ hiểu

## 📝 Hướng dẫn sử dụng

1. Đảm bảo file `diabetes.csv` nằm cùng thư mục với `classifier.py`
2. Chạy script để xem kết quả so sánh các mô hình
3. Bỏ comment các dòng code để chạy từng phần cụ thể:
   - EDA report
   - Random Forest với Grid Search
   - Standardization

## 🎯 Mục tiêu tương lai

- [ ] Thêm feature engineering
- [ ] Triển khai web app với Flask/Streamlit
- [ ] Tối ưu hóa mô hình với cross-validation
- [ ] Thêm visualization cho kết quả

## 👨‍💻 Tác giả

**QuyDatSadBoy** - [GitHub Profile](https://github.com/QuyDatSadBoy)

---

⭐ Nếu bạn thấy dự án hữu ích, hãy cho một star nhé!
