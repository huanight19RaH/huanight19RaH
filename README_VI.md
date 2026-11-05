<div align="center">

# Nguyễn Thái Hưng

**Kỹ sư AI & Nhà nghiên cứu Thị giác Máy tính (Computer Vision)**  
Cựu Phó Chủ nhiệm CLB Lập trình FU-DEVER • Đại học FPT Đà Nẵng  
Đà Nẵng, Việt Nam

[English](README.md) • [Tiếng Việt](README_VI.md)

---

[Curriculum Vitae (PDF)](assets/Nguyen_Thai_Hung_CV.pdf) &nbsp;|&nbsp; [LinkedIn](https://www.linkedin.com/in/thai-hung-nguyen-000b24356/) &nbsp;|&nbsp; [GitHub](https://github.com/huanight19RaH) &nbsp;|&nbsp; [LeetCode](https://leetcode.com/u/HungNguyen192/) &nbsp;|&nbsp; [Email](mailto:hungnguyen.190206@gmail.com)

</div>

---

## Tổng Quan

Mình là sinh viên năm 3 chuyên ngành **Trí tuệ nhân tạo (AI)** tại **Đại học FPT Đà Nẵng**, nguyên **Phó Chủ nhiệm Câu lạc bộ Lập trình FU-DEVER**. Định hướng phát triển của mình tập trung vào nghiên cứu thực nghiệm **Computer Vision**, **Image Restoration** và xây dựng các hệ thống **Machine Learning Systems** kết hợp hoạt động học thuật cộng đồng.

- **Nghiên cứu khoa học:** Chuyên sâu về Physics-Informed Deep Learning, Underwater Image Restoration và Low-Light Image Enhancement (LLIE). Đã có 1 bài báo xuất bản tại kỷ yếu hội nghị quốc tế **Springer MIWAI 2026** (Đồng tác giả) và 1 bài báo về phục hồi ảnh dưới nước đã accepted.
- **Kinh nghiệm thực tế:** AI Developer Intern tại **Khối Nghiên cứu & Phát triển FPT Information System (FIS R&D)** - Bộ phận IDA, phát triển pipeline streaming thị giác máy tính thời gian thực cho giải pháp Kamoi Vision AI (AICC).
- **Cộng đồng & Lãnh đạo:** Nguyên Phó Chủ nhiệm **CLB Lập trình FU-DEVER** (nhiệm kỳ 01/2026 – 10/2026), điều phối tổ chức các hội thảo chuyên môn, cuộc thi lập trình và chương trình cố vấn kỹ thuật; nguyên Trưởng ban Truyền thông dự án thiện nguyện Bật Nụ Cười Lên (Sunshine Team).
- **Chứng chỉ ngoại ngữ:** IELTS 6.0 (2024).

---

## Nghiên Cứu Khoa Học & Công Bố

### 1. HybridLLIENet: Multi-Space Luminance Prior Fusion for Low-Light Image Enhancement
- **Hội nghị / Nhà xuất bản:** International Conference on Multi-disciplinary Trends in Artificial Intelligence (MIWAI 2026), **Springer**
- **Vai trò:** Đồng tác giả (Co-Author)
- **Phương pháp tiếp cận:** Nghiên cứu tăng cường ảnh thiếu sáng bằng kỹ thuật hợp nhất prior độ sáng đa không gian màu (LAB-L, HSV-V, YCbCr-Y) kết hợp CLAHE và gamma correction trên mạng U-Net. Tham gia khảo sát tài liệu, thảo luận thực nghiệm, hoàn thiện bài báo và benchmark mô hình trên tập dữ liệu LOL.
- **Kết quả thực nghiệm:** Đạt **21.23 dB PSNR**, **0.858 SSIM**, **0.127 LPIPS** trên LOLv2-Real với mô hình tối ưu chỉ **8.04M tham số và 79.26 GFLOPs**.
- **Liên kết:** [Kỷ yếu Springer Link](https://link.springer.com/chapter/10.1007/978-981-92-6513-8_10) &nbsp;|&nbsp; [Mã nguồn GitHub](https://github.com/huanight19RaH)

### 2. Assessing Physics-Informed Priors in Underwater Image Restoration
- **Tình trạng:** Bài báo hội nghị đã được chấp thuận (Accepted)
- **Vai trò:** Tác giả (Author)
- **Phương pháp tiếp cận:** Đánh giá các prior vật lý cho bài toán phục hồi ảnh dưới nước bằng cách xây dựng transmission map *t(x)* và backscatter map *B(x)* làm các kênh bổ trợ trong kiến trúc U-Net tùy biến; so sánh đánh giá cấu hình RGB, RGB + *t(x)*, RGB + *B(x)* và RGB + *t(x)* + *B(x)*.
- **Kết quả thực nghiệm:** Đạt **21.012 dB PSNR / 0.884 SSIM** trên UIEB T90 và **26.644 dB PSNR / 0.873 SSIM** trên EUVP-Test đối với mô hình 5 kênh.
- **Liên kết:** [Mã nguồn GitHub](https://github.com/heniath/underwater-image-enhancement)

---

## Dự Án Kỹ Thuật Tiêu Biểu

### Traffic Flow Detection — Nền tảng phân tích luồng video giao thông
- **Quy mô & Phạm vi:** Hệ thống phân tích video giao thông toàn diện hỗ trợ phát hiện, theo dõi, gán làn đường và đếm phương tiện cắt vạch theo hướng di chuyển. Thiết kế luồng xử lý và trực tiếp triển khai giao diện: cấu hình vùng ROI, làn đường, giám sát luồng livestream và bảng điều khiển trực quan.
- **Công nghệ sử dụng:** Python, FastAPI, YOLO, ByteTrack, OpenCV, React
- **Chỉ số benchmark:** Đạt **Event F1: 0.942, WAPE: 5.04%** trên tập dữ liệu UA-DETRAC; thông lượng xử lý batch đạt **75.8 FPS** (gấp 3.03 lần thời gian thực) và livestream đạt **14.9 FPS** không rớt khung hình.
- **Liên kết:** [Mã nguồn GitHub](https://github.com/monsierpotato/Traffic-Flow)

### ScholarSummar — Trợ lý nghiên cứu tài liệu khoa học trên nền tảng RAG
- **Quy mô & Phạm vi:** Trợ lý thông minh hỗ trợ xử lý tài liệu PDF học thuật, tìm kiếm kết hợp ngữ nghĩa và từ khóa (hybrid search), hỏi đáp tài liệu tự động. Xây dựng các tầng trong RAG pipeline (chunking, embedding, retrieval), giao diện frontend, bộ kiểm thử backend và đóng gói triển khai Docker.
- **Công nghệ sử dụng:** Next.js, FastAPI, PostgreSQL (pgvector), Qdrant, Redis, MinIO, Docker
- **Liên kết:** [Mã nguồn GitHub](https://github.com/quangnhat1504/SchoolSummar)

---

## Kỹ Năng Kỹ Thuật

| Lĩnh vực | Công nghệ & Công cụ |
| :--- | :--- |
| **Deep Learning & Computer Vision** | PyTorch, TensorFlow, OpenCV, scikit-learn, U-Net, YOLO, ByteTrack, Physics-Informed DL |
| **Ngôn ngữ & Hệ thống Backend** | Python, C/C++, SQL, FastAPI, Next.js, NumPy, pandas |
| **Hạ tầng & Công cụ phát triển** | Docker, Linux (Ubuntu), Git, GitHub, PostgreSQL, Qdrant, Redis, Jira, Supabase |

---

## Thành Tích & Giải Thưởng

- **Giải Khuyến Khích** — Research Festival 2026 / Research Connect, Đại học FPT Đà Nẵng (Tháng 5/2026)  
  *Vinh danh công trình nghiên cứu ứng dụng thị giác máy tính và phục hồi ảnh.*
- **Giải Nhì** — Hackathon Lập trình Code Mosaic 2025, Đại học FPT Đà Nẵng (Tháng 10/2025)  
  *Cuộc thi lập trình thuật toán và cấu trúc dữ liệu thường niên.*
- **Giải Khuyến Khích môn Toán** — Kỳ thi Học sinh Giỏi cấp Thành phố Đà Nẵng (Tháng 1/2024)  
  *Khen tặng bởi Sở Giáo dục và Đào tạo Thành phố Đà Nẵng.*

---

## Kết Nối

- **Email:** [hungnguyen.190206@gmail.com](mailto:hungnguyen.190206@gmail.com)
- **LinkedIn:** [thai-hung-nguyen-000b24356](https://www.linkedin.com/in/thai-hung-nguyen-000b24356/)
- **GitHub:** [huanight19RaH](https://github.com/huanight19RaH)
- **LeetCode:** [HungNguyen192](https://leetcode.com/u/HungNguyen192/)
- **Facebook:** [thaihung.0219](https://www.facebook.com/thaihung.0219)
