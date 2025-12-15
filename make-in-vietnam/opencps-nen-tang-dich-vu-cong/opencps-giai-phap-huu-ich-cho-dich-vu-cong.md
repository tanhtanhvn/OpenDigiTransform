# OpenCPS: Giải pháp Hữu ích cho Dịch vụ công

#### 1. Giới thiệu: Bối cảnh và Sự ra đời của OpenCPS

Trong bối cảnh Việt Nam đẩy mạnh xây dựng Chính phủ điện tử (CPĐT) theo mục tiêu đề ra tại Nghị quyết số 36a/NQ-CP, việc hiện đại hóa hệ thống dịch vụ công (DVC) đã trở thành một mệnh lệnh chiến lược, quyết định năng lực cạnh tranh quốc gia và hiệu quả cải cách hành chính. Nền tảng cho một chính phủ số thực thụ đòi hỏi không chỉ sự hiện đại hóa về giao diện, mà còn một cuộc cách mạng về kiến trúc hệ thống lõi. Tuy nhiên, các giải pháp dịch vụ công hiện có thường đối mặt với những thách thức cố hữu như thiếu tính đồng bộ, khó khăn trong việc tích hợp và liên thông giữa các cơ quan, cùng với nền tảng công nghệ cồng kềnh, phức tạp.

Để giải quyết các rào cản kiến trúc này, dự án _"Nghiên cứu, ứng dụng công nghệ nguồn mở xây dựng hệ thống phần mềm lõi dịch vụ công trực tuyến OpenCPS phù hợp Khung kiến trúc Chính phủ điện tử Việt Nam"_ đã được triển khai. Dự án do Công ty Cổ phần Phát triển nguồn mở và dịch vụ FDS thực hiện, với sự tài trợ từ Quỹ Đổi mới công nghệ quốc gia (NATIF), ra đời với sứ mệnh cung cấp một giải pháp công nghệ tiên tiến, kiến trúc linh hoạt và tuân thủ chặt chẽ các tiêu chuẩn kỹ thuật của Việt Nam.

#### 2. Kiến trúc và Triết lý cốt lõi của OpenCPS v2

OpenCPS phiên bản 2 (v2) được cấu thành từ các nguyên lý kiến trúc và triết lý phát triển tiên tiến, tạo nên nền tảng vững chắc cho việc triển khai các hệ thống dịch vụ công quy mô lớn và bền vững.

* Nền tảng công nghệ hiện đại: OpenCPS v2 được nâng cấp toàn diện, xây dựng trên nền tảng Liferay 7.1.1 CE GA2 với kiến trúc OSGi và Microservices. Kiến trúc này cho phép phân tách ứng dụng thành các module độc lập, giúp hệ thống trở nên linh hoạt, dễ dàng mở rộng, tùy biến và bảo trì mà không ảnh hưởng đến các thành phần khác.
* Triết lý nguồn mở: OpenCPS được phát triển theo mô hình tự do nguồn mở (FOSS), sử dụng giấy phép AGPL. Toàn bộ mã nguồn của sản phẩm được công bố công khai trên kho Github tại địa chỉ `https://github.com/VietOpenCPS`, cho phép cộng đồng cùng tham gia phát triển, giám sát và cải tiến, đảm bảo tính minh bạch và bền vững của sản phẩm.
* Tách biệt nghiệp vụ và quy trình: Thay vì phát triển phần mềm theo từng nghiệp vụ chuyên ngành cụ thể, OpenCPS áp dụng một cách tiếp cận đột phá về kiến trúc. Hệ thống được tách thành hai phần riêng biệt: một thành phần lõi quản lý việc tiếp nhận và xử lý hồ sơ theo quy trình một cách tổng quát, và các thành phần ứng dụng chuyên ngành quản lý cơ sở dữ liệu nghiệp vụ. Cách tiếp cận này giải quyết triệt để bài toán thiếu đồng bộ và khó tái sử dụng của các hệ thống cũ, cho phép OpenCPS trở thành một nền tảng linh hoạt có thể áp dụng cho mọi nghiệp vụ hành chính công mà không cần phát triển lại từ đầu.

#### 3. Các Giải pháp Công nghệ Nổi bật của OpenCPS

OpenCPS được kiến tạo từ một hệ thống các giải pháp công nghệ được tích hợp chặt chẽ, cho phép các cơ quan, đơn vị có thể tự chủ trong việc xây dựng và vận hành hệ thống dịch vụ công của mình.

**Phần mềm lõi và các Công cụ Hỗ trợ Linh hoạt**

Hệ thống được trang bị các công cụ quản trị mạnh mẽ, cho phép người dùng không chuyên về kỹ thuật có thể tùy biến hệ thống một cách dễ dàng.

* Quản lý động: Cho phép người quản trị tự khai báo và cấu hình động danh mục các thủ tục hành chính, thành phần hồ sơ, và các loại danh mục dữ liệu dùng chung khác mà không cần can thiệp vào mã nguồn.
* Thiết kế Form động: Cung cấp công cụ đồ họa để thiết kế các tờ khai, giấy tờ kết quả với các trường dữ liệu tùy biến. Dựa trên thư viện alpacajs và JasperReport, công cụ này cho phép tạo ra các biểu mẫu điện tử (eForm) và xuất báo cáo PDF một cách linh hoạt mà không cần lập trình.
* Thiết kế Quy trình động: Người dùng có thể tự định nghĩa các bước xử lý, trạng thái hồ sơ, vai trò tham gia và các luồng công việc. Công cụ này trao quyền cho quản trị viên tự động hóa các bước quan trọng, tiêu tốn thời gian như cấp mã số tiếp nhận hồ sơ, tính phí dịch vụ yêu cầu thanh toán, hay phân công người xử lý trực tiếp ngay trong trình thiết kế quy trình.
* Công cụ Import/Export và Nâng cấp: Dự án đã xây dựng các phần mềm công cụ chuyên dụng để hỗ trợ việc nhập/xuất dữ liệu cấu hình hàng loạt từ các tệp Excel, cũng như các công cụ giúp quá trình cài đặt và nâng cấp phiên bản hệ thống diễn ra một cách tự động.

**Các Quy trình Công nghệ Đảm bảo Chất lượng và Vận hành**

Để đảm bảo OpenCPS không chỉ là một tập hợp các tính năng mà là một nền tảng vận hành cấp doanh nghiệp (enterprise-grade), dự án đã xây dựng và áp dụng một bộ quy trình công nghệ nghiêm ngặt trong suốt vòng đời sản phẩm.

* _Tích hợp và Phân phối liên tục (CI/CD):_ Tự động hóa toàn bộ quy trình từ kiểm thử đơn vị (unit-test), kiểm thử tích hợp (integration-test), tính toán độ phủ mã nguồn (code coverage) đến đóng gói và triển khai sản phẩm. Quy trình này giúp đảm bảo chất lượng của mọi mã nguồn đóng góp từ cộng đồng, tăng tốc độ phát hành và giảm thiểu lỗi.
* _Bảo đảm An toàn, An ninh thông tin:_ Xây dựng các chỉ tiêu kỹ thuật và quy trình chi tiết để hệ thống đáp ứng tiêu chuẩn an toàn an ninh thông tin cấp độ 3. Các biện pháp bảo vệ được áp dụng toàn diện trên cả bốn khía cạnh: hạ tầng mạng, hạ tầng máy chủ, ứng dụng và cơ sở dữ liệu.
* _Bảo đảm Hiệu năng và Mức độ sẵn sàng cao:_ Thiết lập quy trình xây dựng hệ thống theo mô hình cụm (cluster) và cân bằng tải (load balancing) ở cả ba tầng: tầng phân phối tải, tầng máy chủ ứng dụng và tầng cơ sở dữ liệu. Kiến trúc này đảm bảo hệ thống luôn sẵn sàng phục vụ, chịu được tải cao và có thể mở rộng một cách linh hoạt khi cần thiết.
* _Giám sát và Vận hành Hệ thống:_ Tự động hóa việc giám sát các thông số quan trọng của hệ thống như CPU, RAM, mạng, và lưu trữ. Hệ thống có khả năng ghi nhận nhật ký (log) tập trung và tự động thông báo các sự kiện bất thường qua email hoặc SMS, giúp đội ngũ vận hành phát hiện và xử lý sự cố kịp thời.
* _Đảm bảo Tiêu chuẩn Phần mềm Nguồn mở:_ Áp dụng các quy trình để sản phẩm OpenCPS đáp ứng các tiêu chuẩn đánh giá quốc tế dành cho phần mềm nguồn mở, cụ thể là điểm PoF (Potential of Forkability) dưới 25 và điểm OSMM (Open Source Maturity Model) trên 60. Dự án đã thành công trong việc đạt được các chỉ tiêu này, với điểm PoF cuối cùng là +25, đồng thời xác định các định hướng tối ưu hóa tiếp theo để gia tăng sự tin cậy của cộng đồng.

#### 4. Giải pháp hữu ích: Bước tiến về Sở hữu Trí tuệ

Một trong những kết quả khoa học công nghệ mang tính nền tảng của dự án là việc gửi đăng ký một giải pháp hữu ích tại Cục Sở hữu Trí tuệ, khẳng định giá trị công nghệ lõi và sự sáng tạo của đội ngũ phát triển. Tên giải pháp hữu ích là: _"Phương pháp được thực hiện bằng hệ thống máy tính để thực thi các bước xử lý trong quy trình quản lý công việc cộng tác theo mô hình liên tổ chức"_.

Về bản chất, giải pháp này tạo ra một 'ngôn ngữ chung' cho các hệ thống độc lập. Bằng cách mô hình hóa quy trình của mỗi bên và liên kết chúng thông qua các mã số cộng tác được trao đổi tự động, nó cho phép các hồ sơ được xử lý liên thông một cách liền mạch, loại bỏ các bước can thiệp thủ công và đảm bảo tính minh bạch từ đầu đến cuối.

#### 5. Hiệu quả Thực tiễn: Triển khai và Tác động

Hiệu quả của OpenCPS đã được chứng minh qua việc triển khai thành công tại nhiều cơ quan nhà nước cấp Bộ và cấp Tỉnh. Tính đến nay, giải pháp đã được tin cậy triển khai tại 08 bộ ngành và 03 tỉnh thành, minh chứng cho khả năng đáp ứng đa dạng và quy mô lớn.

Dưới đây là bảng thống kê kết quả triển khai tại một số đơn vị tiêu biểu:

<table data-header-hidden><thead><tr><th width="61.94140625"></th><th width="202.88671875"></th><th></th></tr></thead><tbody><tr><td><strong>STT</strong></td><td><strong>Đơn vị triển khai</strong></td><td><strong>Kết quả nổi bật (Số liệu thống kê)</strong></td></tr><tr><td>1</td><td>Bộ Giao thông Vận tải</td><td>401 Dịch vụ công, 982 tài khoản cán bộ, 11.487 hồ sơ khởi tạo.</td></tr><tr><td>2</td><td>Bộ Xây dựng</td><td>49 Dịch vụ công, 176 tài khoản cán bộ, 12.539 hồ sơ khởi tạo.</td></tr><tr><td>3</td><td>Tỉnh Đồng Tháp</td><td>1.781 Dịch vụ công, 3.662 tài khoản cán bộ, 101.173 hồ sơ khởi tạo.</td></tr><tr><td>4</td><td>Bộ Kế hoạch và Đầu tư</td><td>249 Dịch vụ công, 66 tài khoản cán bộ, 6.339 hồ sơ khởi tạo.</td></tr></tbody></table>

Những con số trên cho thấy OpenCPS không chỉ là một giải pháp lý thuyết mà đã trở thành một công cụ được tin dùng trong thực tiễn. Hơn nữa, OpenCPS đã đóng góp như một thành phần quan trọng của nền tảng chính phủ số FlexDigital. Đây là nền tảng "Make in VietNam" đầu tiên được phát triển dựa trên nguồn mở, góp phần hiện thực hóa "Chương trình chuyển đổi số quốc gia đến năm 2025, định hướng đến năm 2030".

#### 6. Kết luận

Dự án OpenCPS đã hoàn thành xuất sắc mục tiêu đề ra, mang đến một giải pháp phần mềm lõi dịch vụ công trực tuyến toàn diện và hiệu quả. Với nền tảng công nghệ hiện đại theo kiến trúc Microservices, triết lý nguồn mở minh bạch, và một hệ thống công cụ tùy biến linh hoạt, OpenCPS đã giải quyết được những bài toán cốt lõi về tính đồng bộ và khả năng tích hợp của các hệ thống dịch vụ công tại Việt Nam.

Việc tuân thủ nghiêm ngặt Khung kiến trúc Chính phủ điện tử Việt Nam, kết hợp với các quy trình sản xuất chuyên nghiệp (CI/CD, an toàn thông tin, giám sát hiệu năng), đã tạo ra một sản phẩm không chỉ mạnh mẽ về tính năng mà còn đáng tin cậy về chất lượng và an toàn. Thành công trong việc triển khai thực tế tại nhiều Bộ, ngành và địa phương, cùng với việc được công nhận giải pháp hữu ích về sở hữu trí tuệ, đã khẳng định vị thế của OpenCPS. Hơn cả một sản phẩm, OpenCPS đã khởi tạo một hệ sinh thái công nghệ mở, quy tụ các doanh nghiệp công nghệ lớn như Viettel và CMC, định hình một hướng đi bền vững cho các sản phẩm công nghệ "Make in Vietnam" phục vụ chính phủ số. Đây là một sản phẩm tiêu biểu, đóng góp thiết thực vào mục tiêu cải cách hành chính và thúc đẩy sự phát triển của chính phủ số quốc gia.
