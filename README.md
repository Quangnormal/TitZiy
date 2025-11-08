# 🧠 TitZiy — Trắc nghiệm

**TitZiy** là một website ôn tập trắc nghiệm ban đầu được tạo ra cho tập thể lớp 11A1 THPT LangBiang Ứng dụng cho phép người dùng làm bài kiểm tra theo từng môn học, chấm điểm tự động, xem kết quả chi tiết và hỗ trợ hiển thị công thức Toán học bằng **MathJax**.  



## 🚀 Tính năng nổi bật

- 📶 **Tốc độ tải câu hỏi nhanh:**
  - Dữ liệu câu hỏi qua file json rất nhẹ
  - Không có backend, mọi hoạt động đều nội bộ thiết bị
  - Việc chạy local giúp mọi trải nghiệm mượt mà

- 🎯 **Hỗ trợ 3 dạng câu hỏi:**
  - Trắc nghiệm 4 lựa chọn
  - Câu hỏi trả lời ngắn
  - Câu hỏi Đúng/Sai

- 🔀 **Xáo trộn đáp án:**  
  Khi bật, hệ thống sẽ tự động thay đổi thứ tự các đáp án A–B–C–D mà vẫn đảm bảo đáp án đúng chính xác.

- 🧮 **Hiển thị công thức Toán học:**  
  Tích hợp **MathJax** để hiển thị các biểu thức, ký hiệu và công thức toán học trong câu hỏi và đáp án.

- 🖥️ **Giao diện gồm 3 trang:**
  1. **Trang chính:** nhập tên, chọn môn, bật/tắt xáo trộn đáp án.
  2. **Trang làm bài:** hiển thị câu hỏi, trạng thái, nút điều hướng (bao gồm kiểm tra đáp án, trở về trước, và sang câu tiếp theo).
  3. **Trang kết quả:** tổng hợp điểm, thống kê đúng/sai và cho phép xem lại từng câu.

- 📊 **Chấm điểm tự động:**  
  Tự động tính điểm và quy đổi sang thang 10, hiển thị số câu đúng và điểm trung bình.

- 📖 **Xem chi tiết từng câu hỏi:**  
  Sau khi nộp bài, người dùng có thể mở **modal** để xem chi tiết câu hỏi, đáp án đã chọn và đáp án đúng.

- 📱 **Tương thích với thiết bị di động (Thiết bị màn hình nhỏ):**  
  Giao diện responsive, có thanh điều hướng riêng cho mobile, hiển thị mượt mà trên mọi thiết bị.


## 🛠️ Công nghệ sử dụng

- **Frontend:** HTML5, CSS3, JavaScript  
- **Thư viện:** MathJax
- **Lưu trữ cục bộ:** LocalStorage  
- **Triển khai:** Cloudflare Pages / Netlify / Vercel



## ⚙️ Cấu hình & Cài đặt

### 1️⃣ Cấu hình file `config.json`

```json
{
  "shuffleAnswers": false,
  "files": ["Monhoc1.json", "Monhoc2.json", "MonhocN.json"]
}
```

### 2️⃣ Cấu trúc thư mục

```
TitZiy/
├── index.html
├── style.css
├── script.js
├── config.json
├── data/
│   └── <các file câu hỏi>
├── README.md
└── LICENSE
```

### 3️⃣ Định dạng file môn học

```json
{
    "Mon": "Tên môn học",
    "QA": [
        {
            "Q": "Câu hỏi trắc nghiệm thông thường",
            "A": "Đáp án A", 
            "B": "Đáp án B",
            "C": "Đáp án C", 
            "D": "Đáp án D",
            "True": "A"
        },
        {
            "Q": "Câu hỏi trả lời ngắn",
            "type": "short_answer",
            "correctAnswer": "Đáp án chính xác cần nhập"
        },
        {
            "Q": "Câu hỏi đúng/sai với 4 câu nhỏ",
            "type": "true_false_set", 
            "questions": [
                {"text": "Nội dung câu 1", "correct": true},
                {"text": "Nội dung câu 2", "correct": false},
                {"text": "Nội dung câu 3", "correct": true},
                {"text": "Nội dung câu 4", "correct": false}
            ]
        }
    ]
}
```


### 4️⃣ Cách chạy dự án🤔

- Dùng các dịch vụ deploy tĩnh như Cloudflare, Netlify,...(Khuyên dùng *Cloudflare*)
- Sau khi deploy thì sử dụng thôi🐢

## 💬 Liên hệ & Hỗ trợ

📞 Zalo: 0977329375  
💬 Messenger: [m.me/Quangnormal](https://m.me/Quangnormal)
## 📜 Giấy phép

Dự án **TitZiy** được phát hành theo giấy phép  
**Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.  

Bạn được phép:
- Sử dụng, chia sẻ và chỉnh sửa dự án này **cho mục đích học tập hoặc cá nhân, tổ chức**.  
- Ghi rõ nguồn: *© 2025 Quang Nguyễn (QuangNormal) — Tác giả dự án TitZiy.*  

Không được phép:
- Dùng dự án này **cho mục đích thương mại hoặc kiếm lợi nhuận**.  
- Bán lại, nhúng vào sản phẩm thương mại hoặc sử dụng để thu phí.  

🔗 Xem chi tiết giấy phép: [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/)

## ⭐ Góp ý & Ủng hộ

Nếu bạn thấy **TitZiy** hữu ích, hãy để lại một ⭐ trên [GitHub](https://github.com/Quangnormal/TitZiy)!