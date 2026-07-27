# 03 — Individual Reflection Report

---

## 1. Đóng góp của Dương trong nhóm

| Hoạt động                   | Đã làm gì?                                                                                                     | Kết quả                                                                                                                       |
| --------------------------- | -------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **Scan cá nhân**            | Đưa ra danh sách 7 problems quan sát được từ lăng kính học tập, sinh hoạt hàng ngày và môi trường thực chiến.  | Nhóm có nguồn candidate đa dạng bao phủ nhiều môi trường (sinh viên, cư dân chung cư, nghiên cứu).                            |
| **Pitch**                   | Pitch bài toán "Tra cứu nội quy chung cư bằng ngôn ngữ tự nhiên" với đầy đủ bối cảnh, actor và dấu hiệu thật.  | Bài được chọn vào shortlist Top 1 vì có pain point rõ ràng từ cả 2 phía (cư dân & BQL).                                       |
| **Challenge**               | Đặt câu hỏi phản biện về việc liệu bài toán tìm quán ăn có dễ thu thập dữ liệu sạch để làm Lab/Demo hay không. | Nhóm loại bớt các đề tài có scope data quá lớn hoặc khó kiểm soát chất lượng đầu vào.                                         |
| **Workflow**                | Làm rõ bottleneck của bài toán                                                                                 | Nhóm sử dụng để làm rõ workflow của bài toán.                                                                                 |
| **Research**                | Tìm hiểu các giải pháp tương tự và kiến trúc RAG (Retrieval-Augmented Generation), Chatbot AI trên App         | Nhóm thấy rõ tính khả thi, không cần train model từ đầu mà chỉ cần làm tốt khâu chuẩn bị Knowledge Base.                      |
| **Rule / Workflow / Agent** | Lập luận chọn mô hình AI Agent kết hợp Workflow .                                                              | Nhóm thống nhất decision: dùng AI Agent cho khâu tra cứu ngữ cảnh, dùng Rule/Workflow cho khâu xuất form và xử lý tranh chấp. |

---

## 2. Bảng dùng AI trong reflection

| Phase                 | Tôi dùng AI để làm gì?                                                                                                | AI hữu ích ở đâu?                                                                                                                | AI sai/hời hợt ở đâu?                                                                                                 | Tôi sửa gì                                                                                                                                                      |
| --------------------- | --------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Scan**              | Gợi ý mở rộng các góc nhìn về nỗi đau (pain point) của sinh viên trong sinh hoạt và học tập.                          | Giúp nhớ thêm các bối cảnh thực tế như tìm trọ lừa đảo, đọc paper tiếng Anh hay xem lại video record.                            | Gợi ý một số ý tưởng quá thiên về kỹ thuật (như "tối ưu hóa database") thiếu hình bóng của Actor và Workflow rõ ràng. | Bỏ các ý không phản ánh nỗi đau người dùng thật, tập trung viết lại theo công thức: Actor + Bối cảnh + Bottleneck.                                              |
| **Workflow**          | Nhờ AI cấu trúc lại các bước từ lúc cư dân phát sinh thắc mắc đến khi được giải đáp thành quy trình từng bước.        | Rất nhanh trong việc phân chia giai đoạn (Current State vs Future State) và ước lượng thời gian trung bình.                      | AI có xu hướng gộp chung bước "đọc dò nội quy" và "đợi BQL trả lời" thành một bước duy nhất.                          | Tách đôi thành 2 bottleneck riêng biệt vì một cái là nỗi đau tự tra cứu (15'), một cái là nỗi đau chờ đợi ngoài giờ (2–12 tiếng).                               |
| **Research**          | Tìm hiểu cách công nghệ RAG hoạt động trong việc tra cứu văn bản pháp lý / nội quy và tìm các tool xây dựng AI Agent. | Gợi ý chính xác cấu trúc giải pháp (Knowledge Base -> Retrieval -> Generation) và giải thích lý do vượt trội hơn Keyword Search. | Có đưa ra một số claim về việc "AI giải quyết 100% khiếu nại của cư dân" thiếu thực tế và không nguồn kiểm chứng.     | Điều chỉnh lại metric (chỉ cam kết giảm > 70% các câu hỏi lặp lại), giữ lại ranh giới chuyển giao cho nhân viên con người xử lý ngoại lệ.                       |
| **Problem Statement** | Nhờ AI phản biện và rà soát lại các field trong Problem Card #1 xem đã đủ độ sắc bén để pitch chưa.                   | Chỉ ra được metric về "trải nghiệm hài lòng" là cảm tính, cần thay bằng metric thời gian và số lượng ticket BQL phải nhận.       | AI đề xuất áp dụng mô hình Agent tự động hóa cả việc ra quyết định xử phạt cư dân mà không cần BQL thông qua.         | Nhóm phản bác và giới hạn scope của Agent: AI chỉ đóng vai trò tra cứu, giải đáp và cung cấp link biểu mẫu; con người (BQL) vẫn giữ quyền quyết định cuối cùng. |

---

## 3. Bài học của Dương

- **Problem tốt là problem có nỗi đau thật và đo lường được:** Một bài toán hay không phải là bài toán nghe có vẻ "đao to búa lớn" hay dùng công nghệ phức tạp nhất, mà là bài toán chỉ ra được chính xác ai đang đau (Actor), đau ở bước nào (Bottleneck) và thời gian tiết kiệm được là bao nhiêu (Success Metric).
- **Vẽ Workflow giúp định hình rõ ranh giới giữa AI và con người (Human Boundary):** Việc phân tích chi tiết quy trình hiện tại và tương lai giúp nhóm nhận ra AI Agent RAG làm rất tốt khâu tra cứu ngữ cảnh và tổng hợp câu trả lời.
- **AI Agent là công cụ mở rộng năng lực, không phải sự thay thế toàn diện:** Trong case study nội quy chung cư, giải pháp tối ưu là sự kết hợp: **Agent** (để hiểu ngôn ngữ tự nhiên của cư dân 24/7) + **Workflow/Rule** (để hướng dẫn điền biểu mẫu đúng quy trình và chuyển tiếp ticket khi vượt ngoài cơ sở tri thức).
- **Research là để hiểu Pattern thành công:** Tham khảo các giải pháp AI CSKH không phải để copy-paste tính năng, mà để nhìn ra mô hình chung của các sản phẩm tốt: _AI xử lý công việc lặp lại tần suất cao -> Con người tập trung giải quyết các ca phức tạp và ra quyết định._

### Nếu làm lại:

```text
Tôi sẽ tiến hành phỏng vấn sâu hoặc khảo sát nhanh thêm 3–5 nhân viên Lễ tân/CSKH tại các chung cư lớn để thu thập số liệu thực tế về tỷ lệ phân bổ các câu hỏi (bao nhiêu % là hỏi nội quy lặp lại, bao nhiêu % là sự cố phát sinh). Điều này sẽ giúp baseline của metric "giảm > 70% lượng tin nhắn thắc mắc" trở nên vững chắc và thuyết phục tuyệt đối trước hội đồng review, thay vì chỉ dựa vào ước lượng từ quan sát trải nghiệm của cư dân.
```
