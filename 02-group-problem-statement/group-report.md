# Group Report — Day 02

> **Candidate được nhóm chọn:** Tái khai thác database CV nội bộ để tìm ứng viên phù hợp với JD.

## Thành viên nhóm

> Nhóm gồm 6 thành viên

| STT | Họ và tên               | Mã học viên | Vai trò trong nhóm |
| --: | ----------------------- | ----------- | ------------------ |
|   1 | Vũ Thùy Dương           | 2A202601483 | Nhóm trưởng        |
|   2 | Đào Văn Đà              | 2A202601089 | Thành viên         |
|   3 | Nguyễn Quốc Anh         | 2A202601079 | Thành viên         |
|   4 | Nguyễn Ngọc Ánh         | 2A202601643 | Thành viên         |
|   5 | Bùi Gia Huy             | 2A202601879 | Thành viên         |
|   6 | Nguyễn Hoàng Vĩnh Phong | 2A202601265 | Thành viên         |

---

| Cluster                        | Candidate examples                                                              | Pattern chung                                                                   |
| ------------------------------ | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Tra cứu / tổng hợp tri thức    | Tra cứu nội quy chung cư, tra cứu quy định trường, hỗ trợ ôn tập từ nhiều nguồn | Tìm đúng thông tin trong nhiều tài liệu hoặc nguồn rời rạc                      |
| Học tập / planning / follow-up | Learning Companion, phát hiện điểm nghẽn lớp, capture và review task            | Kế hoạch, task hoặc vấn đề của người học dễ bị rơi do thiếu context và theo dõi |
| Quy trình vận hành             | Lập và duyệt đơn nghỉ phép, bệnh nhân chờ khám                                  | Nhiều bước và nhiều bên tham gia khiến quy trình chậm hoặc thiếu minh bạch      |
| Đời sống / ra quyết định       | Chọn quán ăn, đề xuất công thức từ thực phẩm có sẵn                             | Người dùng phải so sánh nhiều lựa chọn theo nhiều tiêu chí                      |
| Tuyển dụng / khai thác dữ liệu | Tái khai thác database CV nội bộ                                                | Doanh nghiệp đã có dữ liệu nhưng khó tìm, đánh giá và tái sử dụng hiệu quả      |

## Shortlist và score

| Candidate                              | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain |   Tổng |
| -------------------------------------- | -------: | ----------: | ---------------: | -------------: | ------------: | -----------------: | ---------------: | -----: |
| Tái khai thác database CV nội bộ       |        5 |           5 |                4 |              5 |             5 |                  5 |                5 | **34** |
| Capture và review task từ nhiều nguồn  |        5 |           5 |                4 |              5 |             5 |                  5 |                4 | **33** |
| Hỗ trợ sinh viên ôn tập từ nhiều nguồn |        5 |           5 |                4 |              4 |             5 |                  5 |                4 | **32** |
| Gợi ý quán ăn cho nhóm bạn             |        5 |           5 |                4 |              4 |             5 |                  4 |                5 | **32** |
| Đề xuất công thức từ thực phẩm có sẵn  |        5 |           5 |                4 |              4 |             5 |                  5 |                4 | **32** |

Nhóm chọn: **Tái khai thác database CV nội bộ để tìm ứng viên phù hợp với JD**.

Vì sao chọn:

- Actor và workflow tuyển dụng rõ nhất.
- Pain gắn trực tiếp với thời gian sourcing, chi phí tuyển dụng và time-to-fill.
- Công ty đã có sẵn database CV nhưng chưa khai thác hiệu quả.
- Có thể lấy baseline từ thời gian tạo shortlist, số CV phải mở và tỷ lệ ứng viên được tái sử dụng.
- Có thể validate với recruiter/headhunter và pilot trên một JD cùng một tập CV nhỏ.
- Có thể research các tool/pattern như hybrid search, AI-assisted candidate search và talent rediscovery.
- Có thể vẽ before/after rõ và so sánh Rule / Workflow / Agent.

Vì sao không chọn các bài khác:

- **Capture và review task:** pain rõ nhưng có khả năng one-inbox và review rule đã giải quyết phần lớn vấn đề; giá trị tăng thêm của AI chưa chắc đủ lớn.
- **Hỗ trợ ôn tập từ nhiều nguồn:** workflow rõ nhưng quality metric như “đầy đủ”, “dễ học” và “học hiệu quả hơn” khó thống nhất trong thời gian lab.
- **Lập và duyệt đơn nghỉ phép:** phần lớn có thể giải quyết bằng rule và workflow truyền thống.
- **Chọn quán ăn:** dễ pilot nhưng khó tạo lợi thế rõ so với Google Maps, ứng dụng giao đồ ăn và form bình chọn.
- **Bệnh nhân chờ khám:** impact lớn nhưng domain phức tạp, khó tiếp cận dữ liệu và nhiều quyết định liên quan đến chuyên môn y tế.

## Quick validation

### Validation hiện có

Nhóm hiện có một domain walkthrough từ Huy dựa trên trải nghiệm/quan sát ban đầu. Nhóm chưa có đủ phỏng vấn độc lập hoặc log hệ thống để coi các con số là baseline chính thức.

| Nguồn                                |                      Số người | Tín hiệu xác nhận                                                                                                      | Tín hiệu phản bác                                                                                                    | Nhóm sửa problem thế nào                                                                           |
| ------------------------------------ | ----------------------------: | ---------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Domain walkthrough với người đề xuất |                             1 | Recruiter thử search database bằng từ khóa, phải mở nhiều CV và có xu hướng chuyển sang sourcing ngoài khi kết quả kém | Chưa có log thời gian; chưa biết đây là pain chung hay chỉ xảy ra ở một hệ thống cụ thể                              | Giữ problem ở dạng giả thuyết; không coi 190 phút và 30% là dữ kiện đã xác nhận                    |
| Quick interview recruiter/headhunter | Chưa thực hiện — mục tiêu 3–5 | Cần xác nhận tần suất bỏ database, thời gian tạo shortlist và lý do chuyển sang nguồn ngoài                            | Có thể recruiter cho rằng vấn đề chính là CV cũ, contact stale hoặc JD mơ hồ chứ không phải search                   | Nếu data quality là pain chính, chuyển trọng tâm sang làm sạch, deduplicate và cập nhật trạng thái |
| Pilot trên một JD                    |                Chưa thực hiện | Cần kiểm tra hybrid search có giúp giảm số CV phải mở và tăng tỷ lệ shortlist phù hợp không                            | Nếu recruiter loại phần lớn Top 20 hoặc ứng viên không còn liên hệ được, semantic matching chưa giải quyết pain thật | Hạ xuống rule/filter hoặc chuyển sang candidate status refresh                                     |

Insight cần kiểm chứng:

```text
Pain có thể không chỉ nằm ở việc “tìm CV theo ngữ nghĩa”.

Pain có thể gồm ba lớp:

1. Retrieval:
   Không tìm được đúng CV vì keyword search hạn chế.

2. Data quality:
   CV cũ, trùng lặp, thiếu field, thiếu lịch sử tương tác hoặc trạng thái.

3. Reachability:
   Ứng viên phù hợp nhưng contact cũ, không còn tìm việc hoặc không muốn được liên hệ.

Nếu lớp 2 và 3 là nguyên nhân chính,
Vector Search + LLM đơn thuần sẽ không đủ.
```

### Câu hỏi phỏng vấn nhanh

- Lần gần nhất anh/chị tìm ứng viên trong database nội bộ là khi nào?
- Mất bao lâu từ lúc nhận JD đến lúc có shortlist đầu tiên?
- Anh/chị phải mở thủ công khoảng bao nhiêu CV?
- Khi nào anh/chị quyết định từ bỏ database và chuyển sang LinkedIn/job board?
- Kết quả fail chủ yếu vì search kém, CV cũ hay không liên hệ được?
- Tỷ lệ shortlist hiện tại đến từ database nội bộ là bao nhiêu?
- Anh/chị cần xem bằng chứng nào để tin một matching score?
- Hệ thống có dữ liệu trạng thái và lịch sử tương tác của ứng viên không?

## Research giải pháp

Nhóm tìm các hướng đã có sẵn, không giả định phải tự build từ đầu.

| Nguồn / tool / case                   | Link                                                    | Họ giải quyết phần nào?                                                                | Điểm mạnh                                                                       | Khoảng trống / rủi ro                                                                        | Bài học cho nhóm                                                                                |
| ------------------------------------- | ------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Elasticsearch Hybrid/Semantic Search  | https://www.elastic.co/elasticsearch                    | Kết hợp full-text, semantic search, filter, ranking và reranking                       | Phù hợp để xây hybrid retrieval trên CV và structured metadata                  | Không tự làm sạch CV, cập nhật trạng thái, kiểm tra contact hoặc xử lý quyền sử dụng dữ liệu | Dùng keyword + structured filter + semantic search thay vì chỉ Vector Search                    |
| LinkedIn Recruiter AI-Assisted Search | https://www.linkedin.com/help/recruiter/answer/a1673734 | Chuyển yêu cầu tuyển dụng bằng ngôn ngữ tự nhiên thành search/filter và recommendation | Cho thấy pattern nhập JD/intake bằng ngôn ngữ tự nhiên có giá trị với recruiter | Hoạt động trên dữ liệu LinkedIn; không tự giải quyết database nội bộ của công ty             | Natural-language search nên hỗ trợ recruiter refine, không thay recruiter quyết định            |
| Greenhouse Talent Rediscovery         | https://www.greenhouse.com/ai-recruiting                | Tìm lại ứng viên tiềm năng trong database ATS và giảm hồ sơ trùng/spam                 | Use case gần trực tiếp với bài toán nhóm                                        | Phụ thuộc chất lượng dữ liệu ATS và quy trình cập nhật ứng viên                              | “Talent rediscovery” là pattern thị trường đã có, nhóm nên học cách họ giữ transparency/control |
| LeverTRM Talent Rediscovery           | https://www.lever.co/lever-trm                          | Tái khám phá ứng viên trong database ATS/CRM và quản lý quan hệ ứng viên               | Kết hợp search với candidate relationship/status                                | Không loại bỏ nhu cầu human review và cập nhật trạng thái                                    | Retrieval phải đi cùng trạng thái ứng viên và lịch sử tương tác                                 |

Research takeaway:

```text
Không nên build một Agent tự chạy toàn bộ quy trình tuyển dụng.

Hướng hợp lý hơn là Workflow:

[Chuẩn hóa dữ liệu tối thiểu]
→ [Structured filter + keyword search]
→ [Semantic matching/reranking]
→ [Tóm tắt lý do match kèm evidence]
→ [Recruiter review]
→ [Recruiter quyết định liên hệ]
→ [Cập nhật trạng thái vào ATS/CRM]

AI hỗ trợ retrieval, ranking và explanation.
Con người giữ quyền shortlist, liên hệ và quyết định tuyển dụng.
```

## Workflow before/after

Nội dung workflow:

```text
CURRENT STATE — 6 bước, khoảng 190 phút

[1 Nhận và phân tích JD: 10']
→ [2 Search từ khóa trong database cũ: 30']
     <-- nghẽn: nhiều kết quả, CV cũ, thiếu trạng thái
→ [3 Viết content và đăng tuyển mới: 45']
→ [4 Sourcing thủ công trên LinkedIn/Facebook: 60']
     <-- bottleneck
→ [5 Đọc và lọc CV mới: 30']
→ [6 Nhập CV mới vào CRM/DB: 15']
     <-- có thể tạo thêm duplicate

FUTURE STATE — 5 bước, mục tiêu khoảng 40–45 phút

[1 Nhận JD và xác nhận tiêu chí bắt buộc: 5']
→ [2 Rule/filter + hybrid search database: 2–5']
→ [3 AI ranking + summary lý do match cho Top 20: 3–5']
→ [4 HR review evidence, trạng thái và chọn shortlist: 15']
     <-- Human boundary
→ [5 HR liên hệ ứng viên và cập nhật trạng thái: 15']

Fallback:
AI matching sai, dữ liệu quá cũ hoặc Top ứng viên không liên hệ được
→ HR chuyển sang sourcing ngoài
→ ghi lại lý do fail để cải thiện data, filter và ranking.

Bottleneck mới:
HR review + xác minh trạng thái.

Đây là bottleneck chấp nhận được vì recruiter cần kiểm soát
chất lượng, bias và quyết định liên hệ.
```

Before/after impact:

| Metric                  |                     Trước |                             Sau kỳ vọng | Ghi chú                                |
| ----------------------- | ------------------------: | --------------------------------------: | -------------------------------------- |
| Thời gian tạo shortlist |           Khoảng 190 phút |                            Dưới 45 phút | Target chính; cần đo baseline thật     |
| Nguồn ứng viên nội bộ   |          Chưa có baseline |                   Ít nhất 30% shortlist | Mục tiêu thử nghiệm, chưa phải dữ kiện |
| Số CV phải mở thủ công  |            Nhiều, chưa đo |                           Review Top 20 | AI phải kèm evidence                   |
| Bước thủ công           |          Hầu hết workflow |               Review, xác minh, liên hệ | HR vẫn quyết định                      |
| Bottleneck chính        | Search kém + sourcing mới |            Review + kiểm tra trạng thái | Human boundary                         |
| Risk mới                |    Bỏ sót CV, tốn chi phí | Bias, match sai, CV cũ, automation bias | Cần kiểm tra và rollback               |

## Problem Statement v0

| Field              | Nội dung                                                                                                                                        |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actor**          | Recruiter hoặc headhunter chịu trách nhiệm sourcing và tạo shortlist cho một JD mới.                                                            |
| **Workflow**       | Nhận JD → search database nội bộ → mở CV thủ công → kết quả kém → sourcing ngoài → nhận CV mới → nhập lại ATS/CRM.                              |
| **Bottleneck**     | Công cụ tìm kiếm nội bộ không giúp recruiter nhanh chóng tìm và đánh giá lại ứng viên phù hợp trong database lớn, cũ và thiếu cấu trúc.         |
| **Impact**         | Theo ước lượng ban đầu, workflow mất khoảng 190 phút/vị trí; phát sinh chi phí sourcing; kéo dài time-to-fill và tăng hồ sơ trùng.              |
| **Success Metric** | Sau khi có baseline: giảm thời gian tạo shortlist xuống dưới 45 phút; ít nhất 30% shortlist đến từ database; không giảm phone-screen pass rate. |
| **Boundary**       | Không tự loại, tự liên hệ hoặc quyết định tuyển; recruiter phải kiểm tra evidence, trạng thái và xác nhận shortlist.                            |

## Rule / Workflow / Agent

| Mức                     | Phương án                                                                             | Khi nào đủ                                                          | Rủi ro                                                 | Chọn?                   |
| ----------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------ | ----------------------- |
| **No AI / process fix** | Gom CV về một nguồn, làm sạch duplicate, cập nhật trạng thái và quy định nhập dữ liệu | Đủ nếu pain chủ yếu do dữ liệu phân tán hoặc không được cập nhật    | Tốn công vận hành; chưa giải quyết đối chiếu ngữ nghĩa | Dùng làm nền tảng       |
| **Rule**                | Structured filter, Boolean Search, tag, recency threshold, loại duplicate             | Đủ nếu CV và JD có field chuẩn, điều kiện rõ                        | Tag khó maintain; bỏ sót kỹ năng tương đương           | Dùng cho điều kiện cứng |
| **Workflow**            | Parse JD → filter → hybrid search → ranking/summary → HR review                       | Phù hợp vì workflow tuyến tính, AI chỉ hỗ trợ retrieval và ngôn ngữ | Match sai, bias, dữ liệu cũ; cần HR review             | **Chọn**                |
| **Agent**               | Agent tự lấy dữ liệu, hỏi thêm, liên hệ và cập nhật pipeline                          | Chỉ cần nếu hệ thống phải tự lập kế hoạch và chạy nhiều nhánh       | Quá nhiều permission, privacy và hiring risk           | Chưa chọn               |

Mức chọn:

```text
Workflow.
```

Vì sao:

- Data cleaning và điều kiện cứng có thể dùng process fix/rule.
- Hybrid search giúp kết hợp từ khóa, metadata và ngữ nghĩa.
- AI hỗ trợ tóm tắt lý do match nhưng không thay recruiter đánh giá.
- Recruiter vẫn review nên risk có thể kiểm soát.
- Chưa cần Agent vì workflow không cần tự lập kế hoạch động hoặc tự liên hệ ứng viên.

## Problem Statement v1

| Field                            | Nội dung                                                                                                                                                                                                     |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Actor**                        | Recruiter/headhunter chịu trách nhiệm tạo shortlist cho một JD mới tại công ty đã có database ứng viên lịch sử.                                                                                              |
| **Workflow**                     | Nhận và làm rõ JD → tìm database → mở và đánh giá CV → nếu kết quả kém thì sourcing ngoài → nhập CV mới về ATS/CRM.                                                                                          |
| **Bottleneck**                   | Recruiter không thể nhanh chóng tìm, xếp hạng và kiểm tra ứng viên phù hợp vì search chủ yếu dựa trên từ khóa, hồ sơ thiếu cấu trúc và trạng thái có thể đã cũ.                                              |
| **Impact**                       | Theo ước lượng hiện tại, khoảng 190 phút/vị trí; phát sinh chi phí sourcing, kéo dài time-to-fill và làm giảm giá trị của database đã đầu tư.                                                                |
| **Success Metric**               | Sau khi đo baseline: giảm thời gian tạo shortlist xuống dưới 45 phút; ít nhất 30% shortlist đến từ database; không giảm phone-screen pass rate; mọi gợi ý có evidence để HR kiểm tra.                        |
| **Boundary**                     | AI không tự loại, liên hệ, cam kết hoặc quyết định tuyển; không sử dụng tiêu chí không liên quan đến công việc; HR duyệt toàn bộ shortlist.                                                                  |
| **AI intervention point**        | Sau khi JD đã được recruiter xác nhận và trước bước mở/đọc thủ công hàng loạt CV.                                                                                                                            |
| **Mức chọn**                     | Workflow: process fix + rule/filter + hybrid search + AI summary + HR review.                                                                                                                                |
| **Rủi ro & người thật kiểm tra** | Risk: bias, match sai, duplicate, CV/contact cũ, rò rỉ dữ liệu và automation bias. Người thật review: recruiter xác minh evidence, trạng thái và quyết định liên hệ; quản trị viên kiểm soát quyền truy cập. |

## Final decision

Decision:

```text
Go với scope nhỏ ở mức pilot nội bộ,
chưa dùng để tự động ra quyết định tuyển dụng.
```

Pilot nhỏ nhất:

- Chọn 1 JD có tiêu chí tương đối rõ.
- Dùng một tập 200–500 CV đã được cấp quyền sử dụng.
- So sánh:
  1. Keyword/Boolean Search hiện tại.
  2. Structured filter + semantic search + AI summary.
- Trả về Top 20 ứng viên cho recruiter review.
- Không tự gửi email, không tự thay đổi trạng thái và không tự loại ứng viên.
- Đo:
  - thời gian tạo shortlist;
  - số CV phải mở;
  - tỷ lệ Top 20 được recruiter giữ lại;
  - tỷ lệ contact còn sử dụng được;
  - số lỗi match nghiêm trọng;
  - phone-screen pass rate nếu có thể theo dõi.

Exit / rollback:

- Nếu recruiter phải loại hơn 70% Top 20 trong hai pilot liên tiếp, hạ xuống process fix + rule/filter.
- Nếu ứng viên phù hợp nhưng phần lớn không liên hệ được, chuyển trọng tâm sang cập nhật trạng thái và candidate relationship management.
- Nếu AI trích sai kinh nghiệm hoặc không chỉ ra được evidence, không dùng ranking đó trong workflow.
- Nếu phát hiện dữ liệu không được phép sử dụng hoặc không thể kiểm soát quyền truy cập, dừng pilot.
- Nếu hybrid search không cải thiện đáng kể thời gian hoặc chất lượng so với keyword search, chọn No-Go cho phần AI.

Decision rationale:

- Problem, actor và workflow tương đối rõ.
- Có non-AI components bắt buộc.
- AI nằm ở các bước retrieval, ranking và explanation, không ôm toàn bộ workflow.
- Human review rõ ở bước shortlist và liên hệ.
- Pilot có scope nhỏ, metric và rollback cụ thể.
- Chưa chuyển sang Agent hoặc tự động ra quyết định tuyển dụng.

---
