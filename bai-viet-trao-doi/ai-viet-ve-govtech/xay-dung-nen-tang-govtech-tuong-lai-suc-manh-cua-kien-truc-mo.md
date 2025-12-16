# Xây dựng Nền tảng GovTech Tương lai: Sức mạnh của Kiến trúc Mở

GovTech, hay Công nghệ Chính phủ, không đơn thuần là việc số hóa các dịch vụ công. Theo Ngân hàng Thế giới (World Bank), đây là một cuộc cách mạng toàn diện nhằm hiện đại hóa các chức năng cốt lõi của chính phủ, đặt con người vào trung tâm và thúc đẩy sự tham gia tích cực của công dân. Cách tiếp cận này tạo ra một sự tương phản rõ rệt với mô hình cũ, vốn tồn tại nhiều thập kỷ qua với các ứng dụng đơn khối, đặc thù cho từng cơ quan, được kết nối với nhau qua các tích hợp điểm-tới-điểm mong manh và dễ đổ vỡ.

Tầm nhìn về một nền tảng GovTech hiện đại là xây dựng một hệ thống mô-đun, linh hoạt, được kết nối qua các giao diện lập trình ứng dụng (API) và lấy người dùng làm trung tâm. Thay vì mỗi cơ quan tự xây dựng một hệ thống riêng biệt, mô hình mới hướng đến việc tạo ra các khối xây dựng (building blocks) có thể tái sử dụng trên toàn chính phủ. Bài viết này sẽ phân tích một mô hình kiến trúc cho Nền tảng Phát triển Ứng dụng GovTech dựa trên các công nghệ nguồn mở, một phương pháp chiến lược nhằm tăng tốc độ phát triển, giảm chi phí và thúc đẩy sự đổi mới sáng tạo trong khu vực công.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

#### 1. Tầm nhìn chiến lược: "Chính phủ như một Nền tảng" (Government as a Platform - GaaP)

Nền tảng cho kiến trúc GovTech hiện đại là tầm nhìn chiến lược "Chính phủ như một Nền tảng" (GaaP). Khái niệm này mô tả một cơ sở hạ tầng cốt lõi dùng chung, bao gồm các hệ thống, công nghệ và quy trình số được chia sẻ trên toàn bộ các cơ quan chính phủ. Thay vì hoạt động như những thực thể riêng lẻ, các cơ quan có thể tận dụng nền tảng chung này để xây dựng và cung cấp dịch vụ một cách hiệu quả và đồng bộ.

Dựa trên Khuôn khổ Mô hình Chính phủ số của Liên Hợp Quốc, tầm nhìn GaaP được thúc đẩy bởi các nguyên tắc cốt lõi sau:

* Lấy dữ liệu làm trung tâm (Data centricity): Mọi quyết định và dịch vụ đều phải được xây dựng dựa trên dữ liệu. Dữ liệu được coi là tài sản chiến lược của quốc gia, cần được quản lý, chia sẻ và khai thác một cách hiệu quả và an toàn.
* Lấy người dân làm trung tâm (Human-centered service delivery): Các dịch vụ công phải được thiết kế xoay quanh nhu cầu và các sự kiện trong đời sống thực tế của người dân và doanh nghiệp, thay vì theo cấu trúc tổ chức của các cơ quan chính phủ. Nói cách khác, chính phủ phải tự tổ chức lại xung quanh các sự kiện trong đời sống của người dân (như sinh con, bắt đầu kinh doanh, nghỉ hưu) thay vì bắt người dân phải hiểu cấu trúc của bộ máy hành chính.
* Cách tiếp cận toàn chính phủ (Whole-of-government approach): Phá vỡ các "silo" dữ liệu và nghiệp vụ đang tồn tại giữa các bộ, ngành, địa phương. Các cơ quan cần hợp tác và chia sẻ thông tin liền mạch để cung cấp trải nghiệm dịch vụ thống nhất cho người dân.
* Hạ tầng số dùng chung (Digital infrastructure): Xây dựng các khối nền tảng công nghệ có thể tái sử dụng trên toàn quốc, chẳng hạn như định danh số, thanh toán, trao đổi dữ liệu, để tránh lãng phí nguồn lực và đẩy nhanh tốc độ triển khai dịch vụ mới.

#### 2. Kiến trúc của Nền tảng Phát triển Ứng dụng GovTech

Một nền tảng GovTech hiện đại được cấu thành từ nhiều lớp kiến trúc, mỗi lớp đảm nhiệm một chức năng riêng biệt nhưng phối hợp chặt chẽ với nhau để tạo thành một hệ thống hoàn chỉnh.

**Lớp Hạ tầng Tính toán (Compute Infrastructure)**

Lớp hạ tầng là nền móng của toàn bộ hệ thống. Trong kỷ nguyên số, hạ tầng này phải được thiết kế theo triết lý đám mây-gốc (cloud-native) và phi máy chủ (serverless). Điều này cho phép các ứng dụng có thể chạy linh hoạt trên bất kỳ môi trường đám mây nào đã được chứng nhận, giúp tối ưu hóa chi phí, tăng khả năng mở rộng và tránh phụ thuộc vào một nhà cung cấp duy nhất.

Song song đó, việc áp dụng các thông lệ DevOps là yêu cầu bắt buộc. DevOps thay thế các phương pháp vận hành IT truyền thống bằng cách tự động hóa và tích hợp chặt chẽ các quy trình phát triển (Development) và vận hành (Operations), giúp tăng tốc độ triển khai phần mềm, cải thiện độ tin cậy và thúc đẩy văn hóa hợp tác.

**Lớp Nền tảng Dữ liệu (Data Platform)**

Dữ liệu là mạch máu của chính phủ số. Lớp này chịu trách nhiệm quản lý, lưu trữ và tạo điều kiện cho việc trao đổi dữ liệu an toàn, hiệu quả trên toàn chính phủ. Mô hình kiến trúc lý tưởng là một "Kho dữ liệu chung quốc gia" (National data commons), kết hợp giữa sức mạnh của _hồ dữ liệu (data lake)_ để lưu trữ dữ liệu thô quy mô lớn và sự linh hoạt của _lưới dữ liệu (data mesh)_ để quản trị dữ liệu phân tán. Kiến trúc này cho phép thực hiện các truy vấn phức tạp và triển khai các mô hình học máy trên toàn bộ kho dữ liệu của chính phủ.

Nguyên tắc cốt lõi của lớp này là "dữ liệu mở theo mặc định" (open by default). Dữ liệu công phải được cung cấp ở định dạng máy đọc được (machine-readable) và không độc quyền (non-proprietary), cho phép người dân, doanh nghiệp và các nhà phát triển dễ dàng truy cập và tái sử dụng, từ đó tạo ra các giá trị kinh tế - xã hội mới.

Một hình mẫu thành công điển hình là nền tảng trao đổi dữ liệu liên-cơ quan an toàn X-Road của Estonia. X-Road cho phép các cơ quan chính phủ chia sẻ dữ liệu một cách bảo mật và tin cậy mà không cần tạo ra các cơ sở dữ liệu tập trung, cồng kềnh.

**Lớp Hạ tầng số Công cộng (Digital Public Infrastructure - DPI)**

Lớp Hạ tầng số Công cộng (DPI) bao gồm các khối xây dựng (building blocks) có thể tái sử dụng mà mọi ứng dụng và dịch vụ công đều phụ thuộc vào. Việc chuẩn hóa các khối DPI giúp tăng tốc độ phát triển và giảm chi phí đáng kể. Các thành phần DPI cốt lõi bao gồm:

* Định danh số (Digital Identity): Đây là nền tảng của mọi giao dịch số. Tầm nhìn Identity 2.0 không chỉ cung cấp danh tính cho con người và doanh nghiệp mà còn cho cả máy móc và các tác nhân phần mềm. India Stack với hệ thống định danh sinh trắc học lớn nhất thế giới Aadhaar là một ví dụ điển hình về sức mạnh của DPI, giúp hàng tỷ người dân Ấn Độ tiếp cận dịch vụ tài chính và công.
* Thanh toán có thể lập trình (Programmable Payments): Một hạ tầng thanh toán được token hóa, cho phép tích hợp các hợp đồng thông minh (smart contracts) và thực hiện các khoản thanh toán tự động, theo quy tắc. Ví dụ, hệ thống có thể tự động giải ngân trợ cấp khi một cột mốc trong dự án được xác minh.
* Điều phối Dịch vụ (Service Orchestration): Một cấu trúc cho phép các dịch vụ và tác vụ được kết hợp linh hoạt như những "viên gạch Lego". Điều này cho phép các cơ quan chính phủ nhanh chóng tạo ra các quy trình dịch vụ mới, chẳng hạn như quy trình đăng ký khai sinh hoặc đăng ký kinh doanh, bằng cách ghép nối các tác vụ có sẵn từ nhiều cơ quan khác nhau.

Sức mạnh thực sự của các khối DPI này được thể hiện ở Lớp Ứng dụng, nơi chúng được kết hợp lại để tạo ra các dịch vụ liền mạch, đáp ứng nhu cầu thực tế của người dân.

**Lớp Ứng dụng và Giao diện Người dùng (Application and User Interface)**

Đây là lớp trên cùng của kiến trúc, nơi các dịch vụ công được tạo ra bằng cách sử dụng các khối xây dựng từ lớp DPI và tương tác trực tiếp với người dùng cuối. Tầm nhìn cho lớp này là một giao diện người dùng đa phương thức (multimodal shell), bao gồm chat, giọng nói, web và các công nghệ thực tế tăng cường. Mục tiêu là để chính phủ "gặp gỡ người dùng ở nơi họ đang ở", thay vì buộc họ phải tìm đến các cổng thông tin phức tạp.

Một ví dụ thực tế tại Việt Nam là việc 10 địa phương đã tích hợp dịch vụ công trên nền tảng Zalo. Cách tiếp cận này giúp chính quyền tiếp cận hiệu quả 75 triệu người dùng thường xuyên của ứng dụng này, cho phép người dân truy cập dịch vụ công ngay trên một nền tảng quen thuộc mà không cần cài đặt thêm ứng dụng mới.

#### 3. Tại sao Phải là Nguồn Mở?

Việc ưu tiên sử dụng công nghệ nguồn mở trong kiến trúc GovTech không chỉ là một lựa chọn kỹ thuật mà còn là một quyết định chiến lược mang lại nhiều lợi ích to lớn.

1. Tiếp cận nhân tài chất lượng và năng động: Các nhà phát triển tài năng nhất thường muốn làm việc với các công nghệ và framework hiện đại, được công nhận rộng rãi trong cộng đồng. Việc sử dụng nguồn mở giúp các cơ quan chính phủ thu hút và giữ chân nhân tài công nghệ. Hiện nay, nhiều cơ quan chính phủ trên thế giới đã có hồ sơ trên GitHub để chia sẻ mã nguồn và hợp tác với cộng đồng.
2. Thúc đẩy hệ sinh thái kinh tế số: Khi chính phủ xây dựng trên các nền tảng mở, họ tạo ra cơ hội cho các công ty khởi nghiệp (startup) và các doanh nghiệp công nghệ trong nước tham gia vào việc phát triển các ứng dụng và dịch vụ tùy chỉnh. Điều này tạo ra một thị trường GovTech sôi động và thúc đẩy sự phát triển của nền kinh tế số quốc gia.
3. Tránh phụ thuộc vào nhà cung cấp (Vendor Lock-in): Việc sử dụng các tiêu chuẩn và nền tảng mở giúp chính phủ không bị trói buộc vào công nghệ độc quyền của một nhà cung cấp duy nhất. Điều này không chỉ là một lợi ích về mặt kỹ thuật hay kinh tế, mà còn là một trụ cột của chủ quyền số quốc gia, đảm bảo chính phủ luôn nắm quyền kiểm soát hạ tầng và dữ liệu chiến lược của mình.
4. Minh bạch và Tiết kiệm chi phí: Mã nguồn mở cho phép bất kỳ ai cũng có thể xem xét, kiểm tra và cải tiến, tạo ra sự minh bạch và tin cậy cao hơn. Đồng thời, việc sử dụng các giải pháp nguồn mở thường giúp tiết kiệm đáng kể chi phí bản quyền so với các sản phẩm thương mại.

#### Kết luận: Xây dựng Chính phủ Số Linh hoạt và Bền vững

Việc xây dựng Nền tảng Phát triển Ứng dụng GovTech dựa trên kiến trúc mở và công nghệ nguồn mở không còn là một lựa chọn, mà là một con đường chiến lược tất yếu. Mô hình này mang lại những lợi ích vượt trội: tăng tốc độ cung cấp dịch vụ công, giảm đáng kể chi phí vận hành, tăng cường an ninh mạng một cách toàn diện, thúc đẩy một hệ sinh thái đổi mới sáng tạo và nâng cao tính minh bạch, trách nhiệm giải trình của chính phủ.

Quan trọng hơn, mô hình "Chính phủ như một Nền tảng" không chỉ là một sự thay đổi về công nghệ, mà là một sự chuyển đổi văn hóa từ các cơ quan hoạt động độc lập sang một hệ sinh thái hợp tác. Đây là sự dịch chuyển từ tư duy "xây dựng các hệ thống đóng" sang "cung cấp các khối xây dựng có thể tái sử dụng", cho phép sự đổi mới sáng tạo bùng nổ từ cả khu vực công và tư nhân. Đây chính là con đường để các quốc gia xây dựng một chính phủ số thực sự hiệu quả, linh hoạt và phục vụ người dân ngày một tốt hơn trong kỷ nguyên số.
