# Xây dựng Chính phủ như là một nền tảng trong kỷ nguyên số

_(Bài viết đăng trên Tạp chí Thông tin và Truyền thông — Kỳ 2 - Số 346 (5/2019) — ISSN 1859–3550)_

Phát triển Chính phủ điện tử (CPĐT) đang là một nhiệm vụ trọng tâm, chiến lược của đất nước. Tuy nhiên hiện nay hầu hết các ứng dụng công nghệ thông tin (CNTT) trong CPĐT ở nước ta mới chỉ đóng vai trò như là công cụ hỗ trợ hoạt động. Trong bối cảnh của sự phát triển khoa học công nghệ hướng tới nền kinh tế số và hạ tầng công nghiệp 4.0, CNTT phải được xem như là nền tảng có thể làm thay đổi căn bản phương thức hoạt động, vận hành của Chính phủ.

#### **Chuyển đổi số của Chính phủ**

Năm 2014, Tổ chức Hợp tác và Phát triển kinh tế (OECD) lần đầu tiên đưa ra khuyến nghị về các chiến lược Chính phủ số \[1]. Khi đó tổ chức này đã phân biệt rõ sự khác biệt giữa Chính phủ điện tử (e-government), là cách sử dụng công nghệ để cải thiện các quy trình hiện tại, và Chính phủ số (digital government), là nơi các dịch vụ được thiết kế lại để đưa tới người dùng theo phương thức hoàn toàn mới, sáng tạo với sự hỗ trợ của công nghệ.

Cách tiếp cận để xây dựng hệ thống chính phủ điện tử theo phương thức truyền thống là thực hiện tin học hóa các quy trình đúng theo như cách quản lý vận hành hiện tại. Ví dụ mặc dù văn bản điện tử được đưa vào sử dụng nhưng toàn bộ quy trình ban hành văn bản vẫn được giữ nguyên theo cách thức thực hiện của văn bản giấy. Thậm chí nhiều khi còn phải sử dụng song hành cả hai phiên bản giấy và điện tử cho cùng một văn bản được phát hành. Từ đó dẫn đến hệ thống trở nên phức tạp và gây ra sự tốn kém, thiếu hiệu quả của các tiện ích công nghệ.

Chuyển đổi số trong chính phủ điện tử sẽ là bước đi để đổi mới toàn bộ các quy trình dựa trên tư duy áp dụng công nghệ để tối ưu hóa hiệu quả của các dịch vụ và quản trị công. Chính phủ số phải sử dụng dữ liệu điện tử như là nền tảng để vận hành toàn bộ hệ thống. Khi đó quá trình ban hành văn bản điện tử sẽ phải tối ưu, hiệu quả hơn so với khi dùng quy trình ban hành văn bản giấy như hiện nay. Thậm chí một số loại văn bản, ví dụ như giấy mời họp, sẽ không còn cần thiết nữa vì nó đã được thể hiện bằng một loại dữ liệu điện tử khác thay thế. Chính phủ số cũng có thể gọi là Chính phủ “xanh” bởi toàn bộ hoạt động sẽ là không giấy, người dùng chỉ khai thác các loại dữ liệu điện tử.

Hệ thống chính phủ điện tử hiện nay được xây dựng dựa trên một khung kiến trúc bao gồm các nguyên tắc chiến lược, kiến trúc nghiệp vụ, kiến trúc thông tin, kiến trúc ứng dụng và kiến trúc công nghệ. Trong khung kiến trúc này, công nghệ là yếu tố được thiết kế sau cùng, dùng để thực thi cho các quy trình và ứng dụng đã được đưa ra từ trước đó. Chính điều này là nguyên nhân làm giảm tính hiệu quả của việc áp dụng công nghệ khi chưa có tác động tới việc đổi mới quy trình. Thậm chí trong nhiều dự án, công nghệ có thể trở thành gánh nặng, gây ra nhiều tốn kém cho người sử dụng.

Một trong các ví dụ điển hình về sự thiếu hiệu quả là các dự án số hóa tài liệu hoặc xây dựng cơ sở dữ liệu nhưng không gắn với đổi mới quy trình. Chi phí để thực hiện số hóa của dự án thường là rất lớn, nhưng các dữ liệu tạo ra rất ít được khai thác. Ngoài ra dữ liệu cũng rất nhanh bị lỗi thời sau một thời gian ngắn, do không được duy trì cập nhật một cách thường xuyên theo một quy trình có tính bền vững.

Khác với cách tiếp cận xây dựng hệ thống hướng ứng dụng của chính phủ điện tử hiện nay, chính phủ số sẽ được xây dựng hướng tới nền tảng, Cách tiếp cận hướng nền tảng khắc phục được hạn chế gặp phải của các hệ thống xây dựng theo mô hình đơn lập (silo) như hiện nay. Cụ thể, các ứng dụng thường được xây dựng theo các nhu cầu riêng biệt, tính cục bộ rất cao. Việc chia sẻ khai thác dữ liệu giữa các ứng dùng này thường gặp nhiều khó khăn do thiếu một nền tảng dùng chung.

#### **Chính phủ như là một nền tảng (GaaP)**

GaaP (Goverment as a Platform) là khái niệm thể hiện cho triết lí mới được áp dụng để thực hiện chuyển đổi số của chính phủ điện tử \[2]. Một bản chiến lược chính phủ số cần được xây dựng trước tiên như là cơ sở của toàn bộ kiến trúc hệ thống. Sau đó một nền tảng tích hợp bao gồm chính sách, nghiệp vụ và công nghệ cùng được thiết kế để mang lại sự đổi mới trong hoạt động của chính phủ. Nền tảng này sẽ được dùng để phát triển các loại hình ứng dụng khác nhau của chính phủ điện tử bao gồm G2C (dành cho công dân), G2B (dành cho doanh nghiệp), G2E (dành cho cán bộ công chức) và G2G (dành cho khối chính phủ).

<figure><img src="https://miro.medium.com/v2/resize:fit:319/1*fLz9PPoPktn7R7aPnn8pug.png" alt="" height="323" width="319"><figcaption><p><em>Hình 1. Khung kiến trúc xây dựng chính phủ như là một nền tảng</em></p></figcaption></figure>

Trong chính phủ như là một nền tảng, công nghệ thông tin không chỉ được xem ở khía cạnh thuần ứng dụng, mà còn có vai trò tác động tích cực tới sự thay đổi của các chính sách và nghiệp vụ. Ngay trong quá trình xây dựng luật, các khái niệm tồn tại trong không gian mạng đã được tìm hiểu và đưa vào áp dụng để hình thành một bức tranh về xã hội thông minh như giáo dục thông minh, y tế thông minh, nông nghiệp thông minh, du lịch thông minh. Các loại đối tượng điện tử như tiền mã hóa, chữ kí số, chứng từ điện tử,… được xác định giá trị pháp lý và quản lý như tài sản số trên môi trường mạng.

Nền tảng nghiệp vụ được xây dựng để cụ thể hóa chính sách. Nghiệp vụ thường được quy định bởi các văn bản dưới luật gồm các nghị đinh, thông tư và quyết định. Nền tảng tạo ra sự thống nhất và liên thông cho các nghiệp vụ của chính phủ trên môi trường mạng mà không bị phụ thuộc vào các ứng dụng cụ thể. Nền tảng cung cấp các nghiệp vụ lõi được dùng chung trong nhiều lĩnh vực của chính phủ có thể kể đến như: quản lý văn bản và lưu trữ điện tử, xác thực tài liệu điện tử, tiếp nhận giải quyết hồ sơ hành chính công tại bộ phận một cửa, dịch vụ công trực tuyến, đăng kí và xác minh thông tin trong cơ sở dữ liệu quốc gia, khảo sát điều tra và thống kê tổng hợp,…

_**Nền tảng công nghệ chuyển đổi số**_

Thay vì để công nghệ thông tin được ứng dụng một cách tự phát như hiện nay, trong chính phủ số công nghệ sẽ được chuẩn hóa dưới dạng các nền tảng. Nền tảng công nghệ cung cấp các dịch vụ dùng chung để xây dựng ứng dụng cho từng nghiệp vụ cụ thể hướng tới người dùng. Có thể có rất nhiều ứng dụng khác nhau được phát triển, nhưng do chúng đều cùng sử dụng dịch vụ dùng chung của nền tảng nên bảo đảm tính thống nhất về nghiệp vụ và dữ liệu được chia sẻ.

Trong kỉ nguyên của công nghiệp 4.0, rất nhiều công nghệ dựa trên Internet ra đời có thể được khai thác để xây dựng nền tảng công nghệ cho chính phủ số. Theo một báo cáo của Gartner \[3], chúng ta có thể phân loại các công nghệ được sử dụng cho nền tảng số chính phủ thành 5 nhóm chính như sau:

(i) Nhóm quản lý và phân tích dữ liệu gồm các công nghệ được dùng như là hạt nhân của hệ thống. Dữ liệu là “huyết mạch” của chính phủ số và được quản lý với các công nghệ dữ liệu lớn. Dữ liệu được khai thác sử dụng một cách thông minh dưới sự trợ giúp của các công nghệ về trí tuệ nhân tạo;

(ii) Nhóm trải nghiệm người dùng cung cấp các công nghệ hỗ trợ giao tiếp với người dân và doanh nghiệp thông qua các kênh như cổng thông tin điện tử, ứng dụng di động và mạng xã hội;

(iii) Nhóm xây dựng hệ sinh thái bằng các ứng dụng cung cấp dịch vụ công do doanh nghiệp tư nhân phát triển thông qua việc khai thác dữ liệu mở và các dịch vụ API;

(iv) Nhóm hệ thống thông tin quản lý cung cấp các dịch vụ hỗ trợ tác nghiệp được dùng nội bộ trong các cơ quan nhà nước;

(v) Nhóm mạng kết nối vạn vật IoT dùng công nghệ để tự động hóa tối đa các quy trình dịch vụ công của chính phủ thông qua hệ thống các cảm biến và thiết bị.

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*v_PIz9oNwZ_VEnLwUEHAaw.png" alt="" height="335" width="700"><figcaption><p><em>Hình 2. Phân loại các nhóm nền tảng công nghệ chuyển đổi số (nguồn Gartner)</em></p></figcaption></figure>

_**Đánh giá mức độ sẵn sàng chuyển đổi số**_

Chuyển đổi số của chính phủ điện tử có mục đích áp dụng các tiến bộ của công nghệ để đổi mới các hoạt động quản trị quốc gia nhằm thỏa mãn 4 nhóm tiêu chí lớn gồm: (i) thúc đẩy sự đổi mới và sáng tạo của toàn xã hội; (ii) tăng cường sự tham gia và mức độ hài lòng của người dân và doanh nghiệp đối với khu vực công; (iii) tạo môi trường cạnh tranh để phát triển nền kinh tế; và (iv) phát triển hạ tầng và nguồn lực ICT đáp ứng trình độ công nghệ của kỉ nguyên số. Đây cũng chính là các tiêu chí cơ sở dùng để xây dựng bộ chỉ tiêu đánh giá về mức độ sẵn sàng chuyển đổi số của một quốc gia. Theo một đánh giá mới nhất năm 2018 của Accenture \[4], 3 nước hiện nay đang có điểm đánh giá mức độ sẵn sàng chính phủ số cao nhất lần lượt là Singapore, Anh và Mỹ.

Trên bình diện quốc gia, Việt Nam cũng đã tham gia đánh giá xếp hạng chính thức ở một số bộ chỉ số có liên quan đến 4 nhóm tiêu chí ở trên gồm: chỉ số đổi mới sáng tạo toàn cầu (GII); chỉ số phát triển chính phủ điện tử (EGDI); và chỉ số năng lực cạnh tranh toàn cầu (GCI). Sử dụng kết quả xếp hạng của các bộ chỉ số này, chúng ta cũng có thể đánh giá được sơ bộ về mức độ sẵn sàng xây dựng chính phủ số. Ví dụ bảng xếp hạng năm 2018, Việt Nam đứng thứ 45 về chỉ số GII (thứ 4 khu vực ASEAN), thứ 88 về chỉ số EGDI (thứ 6 khu vực ASEAN), và thứ 77 về chỉ số GCI (thứ 7 khu vực ASEAN). Như vậy sơ bộ chúng ta đang xếp hạng ở mức trung bình của các nước trên thế giới, chưa nằm trong tốp 4 khu vực ASEAN về mức độ sẵn sàng chuyển đổi số.

Trong nước, chúng ta cũng có các bộ chỉ số được đánh giá hàng năm có thể dùng để ước lượng mức độ sẵn sàng xây dựng chính phủ số các địa phương. Đó là chỉ số sẵn sàng phát triển ứng dụng công nghệ thông tin và truyền thông (ICT Index); chỉ số đánh giá hiệu quả quản trị và hành chính công cấp tỉnh (PAPI); và chỉ số năng lực cạnh tranh cấp tỉnh (PCI).

_**Các mô hình xây dựng chính phủ như là một nền tảng**_

Có nhiều mô hình tiếp cận để xây dựng nền tảng của chính phủ số \[5]. Mỗi mô hình xây dựng sẽ có những ưu nhược điểm riêng và cần phải được lựa chọn phù hợp với đặc điểm cụ thể của từng quốc gia. Mô hình đầu tiên là xây dựng một nền tảng tập trung cho toàn bộ chính phủ. Mô hình này có thể triển khai khi chính phủ đã quy định rõ ràng một đầu mối chịu trách nhiệm toàn bộ quá trình chuyển đổi số ở cấp độ quốc gia. Kiểu nền tảng này cung cấp một điểm truy cập tập trung (một cửa) cho tất cả các thông tin và dịch vụ của chính phủ. Mô hình xây dựng một nền tảng toàn chính phủ sẽ thích hợp đối với các quốc gia có quy mô dân số và địa lý nhỏ tương đương với một bang hoặc một thành phố lớn trên thế giới. Ưu điểm chính của mô hình này là có tốc độ triển khai nhanh, tính đồng bộ cao. Tuy nhiên nó cũng đòi hỏi phải xây dựng một bộ máy chuyên trách, đủ tầm năng lực và có đủ quyền lực làm thay đổi cơ chế vận hành của chính phủ.

Mô hình thứ hai dựa trên nguyên lý xây dựng ngang hàng. Nền tảng của chính phủ được xây dựng trên cơ sở tích hợp của các dịch vụ được xây dựng hướng theo các nghiệp vụ chuyên ngành. Mô hình này đòi hỏi sự tăng cường về chia sẻ dữ liệu giữa các nền tảng nghiệp vụ khác nhau trong chính phủ. Kiểu xây dựng nền tảng ngang hàng phù hợp với những quốc gia thiếu một nền tảng dùng chung cho dịch vụ công. Nó thường hướng tới việc tập trung vào cải thiện từng hệ thống nghiệp vụ dùng cho các cơ quan ngành dọc ở tất cả các cấp độ từ trung ương tới địa phương.

Mô hình thứ ba là xây dựng nền tảng hệ sinh thái. Đây là cách tiếp cận mà chính phủ đóng vai trò chính là nhà kết nối trong một nền tảng mở và hướng tới kết quả. Chính phủ thực hiện hợp tác và cung cấp dịch vụ công cùng với các doanh nghiệp tư nhân và tổ chức phi chính phủ. Quá trình xã hội hóa dịch vụ công làm thúc đẩy các quan hệ đối tác và khuyến khích sự đổi mới, sáng tạo ra các giá trị mới. Các nhà quản lý tin rằng chính phủ số là nơi ươm mầm cho các nền tảng xây dựng dựa trên mô hình kinh doanh để hình thành hệ sinh thái của nhiều đối tác. Kiểu xây dựng nền tảng hệ sinh thái là cách tiếp cận phù hợp nhất để thực thi các chính sách có mối quan hệ phức tạp mà rất khó để quản lý bởi chỉ một nhà cung cấp dịch vụ (vd., lĩnh vực quản lý đào tạo nghề và việc làm cho thanh niên). Nền tảng xây dựng theo mô hình hệ sinh thái phải có tính mở hoàn toàn để khuyến khích sự tham gia của tất cả các bên vào việc thiết kế, cung cấp các dịch vụ gia tăng.

Mô hình thứ tư là xây dựng nền tảng dùng nguồn lực số đông. Nếu như mô hình hệ sinh thái chỉ là mở rộng xã hội hóa việc cung cấp dịch vụ công cho các đối tác bên ngoài, mô hình này mở rộng để khai thác nguồn lực của số đông người dân, doanh nghiệp, các tổ chức chính phủ và phi chính phủ trong việc cùng giải quyết một vấn đề mới của xã hội. Kiểu nền tảng này giống như một mạng xã hội, nơi tất cả mọi người đều có thể tham gia đóng góp như nhau. Các ý kiến, thông tin phản ánh của người dân và doanh nghiệp được thu thập thông qua mạng xã hội và được sử dụng như là một nguồn dữ liệu đầu vào quan trọng để cải thiện các hoạt động của chính phủ.

#### **Phát triển chính phủ như là một nền tảng ở Việt Nam**

Quá trình xây dựng chính phủ điện tử ở nước ta đã được khởi động từ rất sớm bắt đầu bằng đề án IT 2000. Tuy nhiên cho đến nay chúng ta vẫn chưa thực sự xây dựng được một hệ thống chính phủ điện tử có tính tổng thể. Ứng dụng CNTT trong các cơ quan nhà nước còn rất rời rạc, hiệu quả thực tiễn mang lại còn rất nhỏ. Trong khi đó lúc này trên thế giới xuất hiện làn sóng chuyển dịch số ở tất cả các quốc gia phát triển. Đây chính là thời cơ để chúng ta cùng thay đổi, xây dựng một nền tảng hiện đại cho chính phủ số mà không phải bỏ chi phí để xây dựng hệ thống với các công nghệ cũ. Mặc dù là nước đứng đầu về chỉ số sẵn sàng chính phủ số, Singapore cũng mới ban hành sách trắng về chiến lược chính phủ số trong năm 2018 \[6]. Do vậy nếu bắt đầu ngay từ bây giờ thì Việt Nam cũng sẽ không đi sau quá muộn so với thế giới.

Không giống các nước nhỏ như Singapore, việc xây dựng một nền tảng tập trung toàn chính phủ rất khó khả thi tại Việt Nam. Xây dựng nền tảng theo mô hình ngang hàng sẽ phù hợp hơn với phương thức tổ chức quản lý chuyên môn theo ngành dọc của các bộ ngành. Tuy nhiên cần tránh việc chia nhỏ nền tảng theo chiều ngang như cách tiếp cận làm ứng dụng hiện nay tại các địa phương. Lý thuyết đã chỉ ra không tồn tại mô hình xây dựng nền tảng theo chiều ngang. Với mỗi lĩnh vực chuyên ngành, ví dụ như quản lý hộ tịch, quản lý đăng kí doanh nghiệp,…. thì chỉ cần thiết lập một cổng dịch vụ công duy nhất là nơi người dân truy cập thực hiện thủ tục hành chính trực tuyến trong phạm vi cả nước. Không nên thiết lập các dịch vụ công trực tuyến tại địa phương vì rất thiếu hiệu quả. Tại đây chỉ cần đưa vào vận hành hệ thống một cửa điện tử, là ứng dụng dùng để tiếp nhận hồ sơ trực tiếp của người làm thủ tục. Hệ thống một cửa điện tử của các địa phương bắt buộc phải sử dụng dịch vụ của các nền tảng nghiệp vụ chuyên ngành trong quá trình thiết lập và xử lý hồ sơ.

Bên cạnh xây dựng các nền tảng ngang hàng, chúng ta cũng cần nghiên cứu lựa chọn các lĩnh vực có tính chất phù hợp hơn để xây dựng nền tảng hệ sinh thái hoặc nền tảng dùng nguồn lực số đông. Ví dụ như các lĩnh vực quản lý lao động-việc làm-bảo hiểm, quản lý du lịch có đặc thù là cần sự tham gia của rất nhiều đối tác để hình thành hệ sinh thái. Do vậy đối với các lĩnh vực quản lý có nhiều bên thì nên ưu tiên đi theo cách tiếp cận mô hình hệ sinh thái.

Vai trò xây dựng nền tảng có ý nghĩa quyết định tới sự thành công của quá trình chuyển đổi số. Chúng ta đã bắt đầu tiến hành xây dựng các ứng dụng quản lý văn bản và điều hành tác nghiệp trong các cơ quan nhà nước từ những năm 2000. Tuy nhiên cho đến nay vẫn chưa hoàn thành xong việc kết nối liên thông trao đổi văn bản điện tử giữa các cơ quan nhà nước trên toàn quốc. Việc xây dựng một trục liên thông văn bản quốc gia chỉ là một giải pháp kĩ thuật, công nghệ dùng để kết nối, trao đổi gửi nhận dữ liệu trong cách tiếp cận hướng ứng dụng truyền thống. Trong chính phủ số, chúng ta cần có một nền tảng quản lý tài liệu điện tử quốc gia. Nó là nền tảng duy nhất thực thi đầy đủ các chính sách và nghiệp vụ về văn thư lưu trữ, ban hành văn bản trong các cơ quan nhà nước. Tất cả các văn bản điện tử tạo ra (dù có dùng bất kì ứng dụng nào) được quy định phải sử dụng dịch vụ lưu trữ điện tử trên nền tảng đám mây của chính phủ. Từ đó nền tảng tạo ra sẽ giải quyết được triệt để các bài toán nghiệp vụ về trao đổi văn bản giữa các cơ quan nhà nước, lưu trữ tìm kiếm thống tin văn bản trong CSDL quốc gia. Khi đưa vào vận hành nền tảng quản lý tài liệu điện tử quốc gia này, chúng ta sẽ tiết kiệm được rất nhiều kinh phí bỏ ra để xây dựng và tích hợp nhiều ứng dụng riêng biệt như quản lý văn bản, công báo điện tử, thư viện số,…

Rõ ràng, chuyển đổi số không chỉ đơn thuần là việc ứng dụng công nghệ. Nó là quá trình tạo ra chính phủ số dựa trên một hệ sinh thái bao gồm các tác nhân liên quan đến Chính phủ, các tổ chức phi chính phủ, doanh nghiệp, tổ chức xã hội và người dân. Chính phủ số khai thác công nghệ như là một nền tảng để thúc đẩy sự tạo ra và truy cập các dữ liệu, dịch vụ và nội dung từ các bên thông qua sự tương tác với đầu mối quản lý chính là các cơ quan nhà nước.

Tổng kết lại, Việt Nam đang có thời cơ nhưng cũng là thách thức để xây dựng được một chính phủ số hiện đại bắt kịp thời đại công nghiệp 4.0. Quá trình chuyển đổi số đòi hỏi phải có sự đổi mới toàn diện về tư duy so với cách làm truyền thống của chính phủ điện tử. Ngoài ra bằng nội lực chúng ta cũng phải có khả năng sáng tạo công nghệ, tự làm chủ việc thiết kế và xây dựng các nền tảng dùng riêng cho Việt Nam.

#### **Tài liệu tham khảo**

\[1] OECD (2014), Recommendation of the Council on Digital Government Strategies, [http://www.oecd.org/gov/digital-government/Recommendation-digital-government-strategies.pdf](http://www.oecd.org/gov/digital-government/Recommendation-digital-government-strategies.pdf)

\[2] Tom Loosemore (2018), Making government as a platform real, [https://public.digital/2018/09/25/making-government-as-a-platform-real/](https://public.digital/2018/09/25/making-government-as-a-platform-real/)

\[3] Gartner (2018), A Digital Government Technology Platform Is Essential to Government Transformation, [https://www.gartner.com/en/doc/344044-a-digital-government-technology-platform-is-essential-to-government-transformation](https://www.gartner.com/en/doc/344044-a-digital-government-technology-platform-is-essential-to-government-transformation)

\[4] Accenture (2018), Government as a platform readiness index, [https://www.accenture.com/acnmedia/PDF-83/Accenture-GaaP-2018-Readiness-Index.pdf](https://www.accenture.com/_acnmedia/PDF-83/Accenture-GaaP-2018-Readiness-Index.pdf)

\[5] Accenture (2018), Four platforms for government, [https://www.accenture.com/us-en/insights/public-service/four-platforms-for-government](https://www.accenture.com/us-en/insights/public-service/four-platforms-for-government)

\[6] Smart Nation Singapore, [https://www.smartnation.sg/](https://www.smartnation.sg/)

**PS**: Bài này đã được trình bày tại Hội thảo Truyền thông mới trong kỷ nguyên chuyển đổi số, Hà nội, ngày 11 tháng 4 năm 2019.&#x20;

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*EoLMDgaB3qLf3HC6hdGw9w.jpeg" alt="" height="467" width="700"><figcaption><p>Hình ảnh tác giả tham dự buổi hội thảo tháng 04 năm 2019</p></figcaption></figure>

