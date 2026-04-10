# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Phạm Ngọc Hùng 

**MSSV:** 1871020265 

**Lớp/Nhóm:** Lớp CNTT 18-01 

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1:Cơ sở dữ liệu khách hàng (Chứa thông tin cá nhân, lịch sử mua hàng)
- Asset 2:Cổng thanh toán trực tuyến (Hệ thống xử lý giao dịch và thông tin thẻ)
- Asset 3 (nếu có):Máy chủ (Server) lưu trữ website

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A -> Hacker đánh cắp thông tin thẻ tín dụng của khách -> Confidentiality (Tính bảo mật): Dữ liệu nhạy cảm bị lộ lọt cho người không có thẩm quyền.
- Sự cố B ->Kẻ tấn công xâm nhập và thay đổi giá niêm yết của sản phẩm -> Integrity (Tính toàn vẹn): Dữ liệu bị chỉnh sửa trái phép, làm mất đi sự chính xác và đáng tin cậy.
- Sự cố C ->Website bị tấn công DDoS khiến người dùng không thể truy cập để mua hàng -> Availability (Tính sẵn sàng): Hệ thống bị gián đoạn, người dùng hợp pháp không thể tiếp cận được dịch vụ khi cần.

---

## 3. Phân tích sự cố B
- Threat: Hacker hoặc đối thủ cạnh tranh có mục đích trục lợi tài chính, gây thất thoát doanh thu và làm giảm uy tín của doanh nghiệp.
- Vulnerability:Cơ chế phân quyền (Access Control) lỏng lẻo, lỗ hổng xác thực đầu vào (ví dụ: Insecure Direct Object References - IDOR), hoặc tài khoản của quản trị viên hệ thống (Admin) sử dụng mật khẩu yếu, không có bảo vệ lớp thứ hai.
- Mitigation:Áp dụng nguyên tắc đặc quyền tối thiểu (Principle of Least Privilege); bắt buộc sử dụng xác thực đa yếu tố (MFA) cho mọi tài khoản có quyền chỉnh sửa dữ liệu; triển khai hệ thống giám sát (Logging & Monitoring) để phát hiện và cảnh báo ngay lập tức khi có sự thay đổi giá cả bất thường.

---

## 4. Reflection
Viết 5-7 dòng.
Qua bài tập này, em nhận thấy việc bảo vệ một hệ thống thông tin luôn phải bắt đầu từ việc xác định chính xác các tài sản (assets) cốt lõi. Việc mapping các sự cố vào tam giác bảo mật CIA giúp em phân loại và đánh giá đúng bản chất của rủi ro: nó đang nhắm vào tính bảo mật, toàn vẹn hay tính sẵn sàng. Khi phân tích sâu một sự cố cụ thể, em hiểu rằng một mối đe dọa (Threat) chỉ có thể khai thác thành công nếu tồn tại lỗ hổng (Vulnerability). Từ đó, việc đề xuất các biện pháp giảm thiểu (Mitigation) trở nên có cơ sở, logic và mang tính ứng dụng thực tế cao hơn trong việc thiết kế hệ thống an toàn.
---

## 5. Bonus Flag
`FIT4012{A-?-B-?-C-?}`

Flag của em:FIT4012{A-C-B-I-C-A}

