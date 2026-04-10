# FIT4012 - Report 1 Page
## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab
- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm
- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính
**Assets:**
- Cơ sở dữ liệu điểm số và thông tin cá nhân của sinh viên.
- Tài khoản định danh và quyền truy cập của giảng viên/quản trị viên.

**CIA mapping:**
- Sự cố A -> (Thay đổi điểm trái phép): Vi phạm tính Integrity (Tính toàn vẹn).
- Sự cố B -> (Hệ thống bị sập, không thể truy cập): Vi phạm tính Availability (Tính khả dụng).
- Sự cố C -> (Rò rỉ bảng điểm ra bên ngoài): Vi phạm tính Confidentiality (Tính bảo mật).

**Phân tích sự cố B:**
- Threat: Tấn công từ chối dịch vụ (DDoS) hoặc quá tải truy cập trong kỳ thi
- Vulnerability: Hệ thống thiếu cơ chế cân bằng tải (Load Balancing) và tài nguyên máy chủ hạn chế.
- Mitigation: Triển khai hệ thống dự phòng, sử dụng Cloud để tự động mở rộng tài nguyên (Auto-scaling) và thiết lập tường lửa ngăn chặn traffic ảo.

### 4. Kết luận ngắn
(4-6 dòng: em học được gì từ bài lab này, phần nào khó nhất, điều gì cần chú ý khi phân tích một sự cố an toàn thông tin.)
Qua bài lab này, em đã hiểu rõ cách vận dụng bộ ba CIA để phân loại và đánh giá rủi ro cho một hệ thống thực tế. Phần khó nhất là việc phân biệt rạch ròi giữa Threat (mối đe dọa bên ngoài) và Vulnerability (điểm yếu nội tại). Bài học quan trọng nhất là khi phân tích sự cố, cần phải nhìn nhận khách quan từ nhiều phía để đưa ra biện pháp giảm thiểu (Mitigation) phù hợp, thay vì chỉ tập trung vào việc vá lỗi kỹ thuật đơn thuần.