# 🎮**LEAGUE OF LEGENDS WINNING RATE PREDICTION BEFORE 15 MINUTES**

## ⚒ Cài đặt

```bash
  pip install -r requirements.txt
```

## 🚀 Trình tự chạy chương trình

Crawl dữ liệu từ 3 trang web

```bash
  1. getlink.ipynb
  2. getdata.ipynb
```

Folder lưu trữ các file dữ liệu thô sau khi craw

```bash
  data/raw_data/
```

Làm sạch dữ liệu

```bash
  data_cleaning.ipynb
```

Folder lưu trữ dữ liệu được làm sạch

```bash
  data/clean_data/
```

Thêm đặc trưng mới, xóa bỏ đặc trưng thừa, chia dữ liệu thành tập train và test, xử lý ngoại lệ, xử lý đặc trưng

```bash
  feature_engineering.ipynb
```

Folder lưu trữ các file dữ liệu đã được xử lý chia ra thành 10 phần 1k

```bash
  data/data etracted/
```
Folder lưu trữ các file dữ liệu kết quả dự đoán (trên tập kiểm thử) của 2 bộ dữ liệu

```bash
  data/result/
```
Xây dựng mô hình dự đoán giá tỷ lệ thắng trận đấu

```bash
  data_processing.ipynb
```

## 👨🏽‍💻 Thành viên

- [Đặng Thị Trúc Ni](https://github.com/trucni2005)
- [Nguyễn Hữu Thiện](https://github.com/huu-thien)
- [Huỳnh Văn Việt](https://github.com/Tyrion1927)

## ✍🏽 Dữ liệu
 Bộ dữ liệu bao gồm các thông tin các trận đấu từ rank bạch kim, thông tin các tướng được thu thập từ:
 - [League of lengends Champions](https://www.leagueoflegends.com/en-sg/champions/)
 - [OP.GG LoL Stats](https://www.op.gg/champions)
 - [League of graphs replays](https://www.leagueofgraphs.com/replays/all)

## 🔨 Feature engineering
 - Thêm các cột chênh lệch rồng, sứ giả, kda lane, vai trò đi đường, tính điểm đội hình
 - Xóa các cột dư thừa sau khi tính chênh lệch
 - Chia dữ liệu, xử lý ngoại lệ
 - Trực quan hóa đặc trưng

## 💡 Mô hình dự đoán
 - **LinearDiscriminantAnalysis** 
 - **LogisticRegression** 

## 🧠 Các metrics đánh giá
 - **Acurracy**
 - **AUC (Area Under the Curve)**

## ☃️ Kết quả dự đoán

| Mô hình          | Acurracy    | AUC      | 
| :--------------- | :----- | :-------- |
| LinearDiscriminantAnalysis | 0.755 | 0.860799 |
| LogisticRegression   | 0.773 | 0.855418 | 