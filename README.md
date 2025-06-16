🧪 Ứng dụng Dự đoán Nguy cơ Viêm Gan C từ Dữ liệu Sức Khỏe
🔍 Giới thiệu
Ứng dụng này giúp dự đoán nguy cơ viêm gan C dựa trên các chỉ số xét nghiệm sinh hóa của người dùng, sử dụng các thuật toán học máy như:

K-Nearest Neighbors (KNN)

Random Forest

K-Means (phân cụm không giám sát)

Apriori (khai phá luật kết hợp)

Ứng dụng được xây dựng bằng Python và giao diện bằng Streamlit, trực quan, dễ sử dụng cho cả người dùng không chuyên ngành.

🏥 Chức năng chính
📄 Hiển thị dữ liệu gốc và bảng giải thích chỉ số sinh hóa (ALT, AST, GGT,...)

📊 Phân cụm bệnh nhân thành nhóm nguy cơ bằng KMeans + trực quan hóa bằng PCA

🔍 Khai phá luật kết hợp từ dữ liệu bằng Apriori với giải thích y khoa

🧠 Dự đoán nguy cơ bằng mô hình KNN hoặc Random Forest

📈 So sánh hiệu suất mô hình theo Accuracy, Precision, Recall, F1

📋 So sánh chỉ số của người dùng với ngưỡng y học

🌱 Gợi ý chăm sóc sức khỏe gan và tài liệu tham khảo

🗃️ Dữ liệu
Bộ dữ liệu được sử dụng là Hepatitis C Dataset từ Kaggle:
📎 https://www.kaggle.com/datasets/fedesoriano/hepatitis-c-dataset

Bao gồm các chỉ số như:

ALT, AST, BIL, GGT, ALB, ALP, CHE, CHOL, CREA, PROT

Tuổi, giới tính và nhãn bệnh

🧠 Mô hình và thuật toán
Tiền xử lý dữ liệu: loại bỏ giá trị thiếu, mã hóa giới tính, chuẩn hóa chỉ số

Tạo cờ nguy cơ cao: Flag_High_Risk dựa trên ngưỡng y khoa

Phân cụm không giám sát: KMeans (n=2)

Dự đoán bệnh: sử dụng KNN và Random Forest

Khai phá luật kết hợp: áp dụng thuật toán Apriori để tìm mối quan hệ giữa các chỉ số bất thường

