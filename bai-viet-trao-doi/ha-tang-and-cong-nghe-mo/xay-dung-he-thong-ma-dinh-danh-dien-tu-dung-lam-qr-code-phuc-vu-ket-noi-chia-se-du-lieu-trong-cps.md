# Xây dựng hệ thống mã định danh điện tử dùng làm QR Code phục vụ kết nối, chia sẻ dữ liệu trong CPS

_(Bài viết đăng ấn phẩm in Tạp chí TT\&TT số 10 — Tháng 10/2021)_

Mã định danh điện tử đang ngày càng trở nên phổ biến và không thể thiếu trong một xã hội số. Với sự phổ biến của thiết bị di động, các mã định danh điện tử được mã hóa dưới dạng QR Code có thể được ứng dụng trong mọi lĩnh vực của đời sống như tài chính, thương mại, dịch vụ, quản lý Nhà nước, v.v.. Vậy bản chất của mã QR Code được sử dụng như thế nào?

#### **Mã định danh điện tử dùng làm QR Code**

QRCode là một dạng mã vạch hai chiều dùng để mã hóa chuỗi kí tự bất kì dưới dạng hình ảnh. Khi dùng một máy quét đọc hình ảnh QRCode, máy tính sẽ nhận diện được chuỗi kí tự đã mã hóa để phân tích và xử lý. Thông thường, trong chuỗi kí tự sẽ chứa một mã định danh gắn với một đối tượng cần quản lý. Định dạng của chuỗi kí tự này sẽ do nhà thiết kế hệ thống quy định.

Tuy nhiên trên thực tế hiện nay có 2 định dạng của chuỗi kí tự mà QRCode thường dùng là: i) Địa chỉ URL liên kết đến một trang thông tin điện tử mô tả thông tin chi tiết của đối tượng gắn mã QRCode; ii) Chuỗi kí tự chứa thông tin mô tả và một mã số định danh duy nhất của đối tượng gắn QR Code. Mã số định danh duy nhất này sẽ được dùng để tham chiếu, tra cứu thông tin chi tiết về đối tượng trên một phần mềm ứng dụng chuyên dùng. Trong nhiều trường hợp QR Code có thể chỉ chứa đúng thông tin mã định danh duy nhất mà không bao gồm thêm bất cứ thông tin nào khác.

Như vậy, bản chất phía sau QR Code là một mã định danh điện tử được dùng bởi các ứng dụng. Tuy nhiên hiện nay, các mã định danh được tạo ra theo nhu cầu “tự phát” bởi các đơn vị phát triển ứng dụng. Chính vì vậy đang có tình trạng “loạn” mã QR Code trong sử dụng, gây ra nhiều bối rối cho người dùng. Một ví dụ gần đây, có nhiều loại mã định danh dạng QRCode đã được sinh ra để phục vụ cho các phần mềm ứng dụng khác nhau phục vụ cho mục đích chống dịch COVID-19 như NCovi, Bluezone, KhaiBaoYTe,…

Tại mỗi điểm đến, cùng lúc có nhiều mã QRCode được dán để người dùng quét bởi các ứng dụng khác nhau. Rõ ràng đây là một sự bất cập lớn cho người dùng vì bản chất mục đích của các mã QR Code này là dùng để định danh cho một điểm đến duy nhất. Vì vậy, trên nguyên tắc thì chúng ta cũng chỉ cần dùng một mã QR Code duy nhất cho tất cả các ứng dụng.

Để khắc phục được tình trạng loạn mã QRCode như kể trên, cần xây dựng một hệ thống tiêu chuẩn mã định danh điện tử được quy định thống nhất để phục vụ kết nối, chia sẻ dữ liệu. Bản thân QR Code đã là một tiêu chuẩn dùng cho hiển thị mã vạch. Nội dung cần được chuẩn hóa ở đây không phải là QR Code mà là cách mã hóa định danh cho các đối tượng thông tin được dùng trong các ứng dụng.

Trên thế giới, việc sử dụng các chuẩn mã định danh thống nhất để xác định các đối tượng quản lý không còn là mới. Mục đích chính của các chuẩn mã định danh là để tạo ra sự liên thông chia sẻ dữ liệu giữa các bên. Ví dụ, hệ thống mã định danh DOI (doi.org) đang được dùng phổ biến trong lĩnh vực thông tin khoa học công nghệ. Các mã DOI được quản lý thống nhất thông qua một tổ chức phi lợi nhuận hoạt động trên quy mô toàn cầu. Tổ chức này đảm bảo hạ tầng kĩ thuật cho việc đăng kí và sử dụng các mã DOI cho các tài nguyên số. Mỗi một mã DOI sẽ được hệ thống phân giải về một địa chỉ URL duy nhất là nơi cung cấp tài nguyên số có mã định danh tương ứng.

Còn có rất nhiều hệ thống mã định danh tiêu chuẩn khác được dùng trong công nghiệp và các lĩnh vực quản lý chuyên ngành. Chẳng hạn ở Việt Nam chúng ta đã áp dụng hệ thống mã định danh của GS1 (gs1.org) trong đăng kí mã số, mã vạch của sản phẩm hàng hóa; định danh phương tiện tàu biển theo tiêu chuẩn IMO; định danh hộ chiếu theo tiêu chuẩn ICAO; v.v.. Như vậy có thể thấy nhu cầu sử dụng các chuẩn mã định điện tử để kết nối, chia sẻ dữ liệu số là điều kiện cần để phát triển Chính phủ số ở nước ta.

#### **Mã định danh điện tử dùng trong kết nối, chia sẻ dữ liệu số**

Trong quá trình phát triển chính phủ điện tử ở Việt Nam, một số quy định về mã định danh điện tử cũng đã được ban hành nhằm mục đích tạo thuận lợi cho việc kết nối, chia sẻ dữ liệu số của cơ quan Nhà nước (CQNN). Cụ thể, Quyết định số 20/2020/QĐ-TTg của Thủ tướng quy định về mã định danh điện tử của các cơ quan, tổ chức để phục vụ kết nối, chia sẻ dữ liệu với các bộ, ngành, địa phương. Theo đó một cấu trúc mã định danh điện tử thống nhất được áp dụng cho tất cả các tổ chức bao gồm doanh nghiệp (DN), hợp tác xã, hộ kinh doanh, CQNN và các tổ chức, đơn vị khác. Như vậy mỗi tổ chức sẽ có một mã định danh điện tử bảo đám tính duy nhất và chính xác trong mọi giao dịch trao đổi dữ liệu số giữa các cơ quan, tổ chức.

Theo quy định tại Nghị định số 61/2018/NĐ-CP về việc thực hiện cơ chế một cửa, một cửa liên thông trong giải quyết thủ tục hành chính cho tổ chức, cá nhân, mỗi hồ sơ thủ tục hành chính cũng được cấp một mã định danh điện tử duy nhất. Mã này được hình thành trên cơ sở ghép nối chuỗi của 3 thông tin gồm: mã định danh cơ quan thực hiện giải quyết thủ tục hành chính (TTHC), ngày tiếp nhận hồ sơ và số thứ tự hồ sơ được tiếp nhận. Tương tự, Quyết định số 395/QĐ-BTTTT của Bộ TT\&TT ban hành hướng dẫn về sử dụng mã định danh văn bản trong các hệ thống thông tin. Mã định danh văn bản được hình thành trên cơ sở ghép nối chuỗi của 3 nhóm gồm: mã định danh cơ quan ban hành văn bản, năm ban hành và số, kí hiệu của văn bản.

Như vậy một số quy định ban đầu về sử dụng mã định danh điện tử cho dữ liệu đã được ban hành để giải quyết cho các nhu cầu thực tiễn là trao đổi dữ liệu về hồ sơ TTHC và văn bản của các CQNN. Hiện chưa có một nghiên cứu hoặc quy định về một hệ thống mã định danh điện tử có tính tổng thể phục vụ kết nối, chia sẻ dữ liệu toàn diện trong một chính phủ số. Thay vì ban hành các quy định rời rạc về sử dụng mã định danh điện tử như nói ở trên, chúng ta cần đưa ra một thiết kế về chuẩn hệ thống mã định danh điện tử có thể áp dụng toàn diện cho nhiều lĩnh vực quản lý khác nhau của CQNN. Hệ thống này được xây dựng dựa trên cơ sở của phương pháp khoa học và phù hợp với thực tiễn hiện đang áp dụng tại Việt Nam.

Ngày nay để tương thích với sự hội nhập toàn cầu trên mạng Internet, hệ thống mã định danh điện tử khi xây dựng cần đáp ứng được hai tiêu chí cơ bản như sau. Thứ nhất, sử dụng chuẩn cấu trúc cú pháp URI (Uniform Resource Identifier) để định danh dữ liệu như là một tài nguyên số chia sẻ trên môi trường Web. Từ đó có thể mô hình hóa, biểu diễn ngữ nghĩa cho dữ liệu chia bằng ngôn ngữ của LOD (Linked Open Data). Đây là mức độ phát triển cao nhất bảo đảm sự tương hợp hoàn toàn về thông tin, dữ liệu trong kết nối, chia sẻ tự động giữa các bên mà không cần sự can thiệp của con người vào quá trình tích hợp các hệ thống.

Thứ hai mã định danh sử dụng phải là dạng vĩnh cửu (persitent identifiers). Tức là, mỗi mã định danh tạo ra chỉ được cấp cho đúng một đối tượng duy nhất và gắn với nó suốt trọn cả vòng đời (ngay kể cả khi đối tượng không còn tồn tại nữa). Do vậy một mã định danh đã dùng thì sẽ không được sử dụng lại cho bất kì đối tượng nào khác. Ngoài ra, mã định danh này phải không được gắn chặt cụ thể với một đường dẫn URL nào trên web, là nơi chứa thông tin gốc mô tả cụ thể về đối tượng. Do đó cấu trúc dùng cho mã định danh phải hoàn toàn độc lập với ứng dụng của nó.

Khi người dùng quét mã QR Code biểu diễn cho mã định danh của một đối tượng, phần mềm ứng dụng sẽ truy vấn tới một hệ thống phân giải mã định danh và nhận kết quả trả về là đường dẫn URL hướng tới một trang web chứa thông tin mô tả cho đối tượng cần tra cứu. Đơn vị khai thác sẽ phải có trách nhiệm đăng kí với tổ chức quản lý hệ thống phân giải này về đường dẫn URL sử dụng cho các mã định danh điện tử đã được cung cấp ra.

#### **Đề xuất chuẩn mở cho mã định danh điện tử phục vụ chia sẻ dữ liệu ở Việt Nam**

Sau đây, bài viết sẽ trình bày một đề xuất mở nhằm xây dựng một hệ thống mã định danh điện tử phục vụ kết nối, chia sẻ dữ liệu số ở Việt Nam goi tắt là VODI (Vietnam Open Data Identifiers). Hệ thống này sẽ đáp ứng đầy đủ cả hai tiêu chí cần thiết đã nêu ở trên và có sự kế thừa các quy định về mã định danh đã được ban hành dùng trong các CQNN.

Một cách tổng quát, tất cả thông tin, tri thức cần quản lý trong Chính phủ số có thể được mô hình hóa bằng một lược đồ khái niệm mức đỉnh (top ontology). Mọi tri thức quản lý đều có thể quy về thành 3 khái niệm mức đỉnh là Chủ thể — Hoạt động — Tư liệu (như minh họa trong hình vẽ). Mối quan hệ tổng quát của chúng là: Chủ thể tham gia các Hoạt động với Tư liệu được sử dụng. Chủ thể nắm quyền sở hữu các Tư liệu.

<figure><img src="https://miro.medium.com/v2/resize:fit:700/0*p6KeDYt5QcEhTslJ.jpg" alt="" height="218" width="700"><figcaption></figcaption></figure>

Hệ thống mã định danh sẽ được thiết kế để bao phủ hết tất cả các đối tượng thông tin được dẫn xuất từ 3 khái niệm mức đỉnh trên. Theo đó từ Chủ thể được phân thành hai nhánh là Cá Nhân và Tổ chức; từ Hoạt động phân thành Nhiệm vụ và Sự kiện; từ Tư liệu phân thành Tài liệu, Sáng tạo (phi vật chất), Sản phẩm (vật chất) và Hạ tầng (không gian địa lý). Chúng ta sẽ sử dụng một cú pháp URI tổng quát để định danh các đối tượng gồm 3 phần là:

**vodi:\<PhanLop>:\<MaDinhDanh>**

Trong đó:

\- **vodi** được dùng làm tên lược đồ định danh (scheme) theo quy tắc của URI

\- **\<PhanLop>** là định danh của các phân lớp dữ liệu bao gồm CaNhan, ToChuc, NhiemVu, SuKien, TaiLieu,… Ở đây chỉ định nghĩa tổng quát mã định danh cho 5 lớp ở mức đỉnh là Cá nhân, Tổ chức, Nhiệm vụ, Sự kiện, Tài liệu. Mã định danh dùng cho các đối tượng thuộc Sáng tạo, Sản phẩm, Hạ tầng sẽ được quy định theo các phân lớp khái niệm cụ thể của từng lĩnh vực quản lý chuyên ngành. Phạm vi của bài viết này sẽ được giới hạn ở mô tả cú pháp mã định danh cho 5 lớp ở mức đỉnh như Bảng mô tả định danh trong lược đồ vodi.

\- **\<MaDinhDanh>** là chuỗi kí tự mã định danh được quy định cho từng phân lớp trong lược đồ vodi.

<figure><img src="https://miro.medium.com/v2/resize:fit:700/0*Hmc4WuezCrrvej3V.jpg" alt="" height="473" width="700"><figcaption><p><em>Bảng mô tả mã định danh trong lược đồ vodi.</em></p></figcaption></figure>

Nghiệp vụ quản lý cho các đối tượng thuộc 3 phân nhánh còn lại (Sáng tạo, Sản phẩm, Hạ tầng) rất đa dạng và thường có tính đặc thù của các lĩnh vực chuyên ngành. Do vậy việc quy định mã định danh cho các phân lớp con sẽ được cụ thể hóa bởi các Bộ/Ngành phụ trách quản lý lĩnh vực. Ví dụ, Bộ GTVT sẽ đưa ra quy định mã định danh đối với phân lớp Phương tiện (vodi:PhuongTien), Bộ KH\&CN sẽ quy định mã định danh cho các Sở hữu công nghiệp (vodi:SHCN), Bộ VHTTDL sẽ quy định mã định danh cho các tác phẩm văn học nghệ thuật (vodi:TPVHNT), v.v..

Cần lưu ý, mã định danh điện tử sẽ không được sử dụng đồng nhất với các mã số quản lý được cấp phục vụ cho các mục đích xử lý nghiệp vụ chuyên ngành. Ví dụ một nhiệm vụ có thể được cấp mã số quản lý riêng trong lĩnh vực KH\&CN, mã số TABMIS dùng để quản lý cấp kinh phí nhiệm vụ trong lĩnh vực kế hoạch tài chính. Mặc dù có nhiều mã số quản lý khác nhau nhưng mã định danh điện tử của nó sẽ phải là duy nhất. Chỉ trong một vài trường hợp cá biệt, mã định danh điện tử sẽ được tạo lập trùng với mã số quản lý được cấp, ví dụ mã định danh của cá nhân và của các đơn vị kinh doanh.

Ngoài ra, cấu trúc mã định danh điện tử đã được quy định chuẩn cho các phân lớp ở mức đỉnh sẽ phải được áp dụng cho tất các đối tượng thuộc các phân lớp dẫn xuất của nó. Không được phép tạo ra một cấu trúc mã định danh mới cho các lớp con. Ví dụ các đối tượng thuộc lớp Bác sĩ sẽ phải sử dụng chung mã định danh điện tử của Cá nhân. Tuy nhiên để phục vụ công tác quản lý chuyên ngành y tế, trong dữ liệu thuộc tính của Bác sĩ có thể bổ sung thêm mã số quản lý được cấp riêng cho nhân viên y tế. Bên cạnh việc bắt buộc phải cấp mã định danh điện tử theo chuẩn như trong đề xuất này, đối với mỗi lớp đối tượng con có thể sử dụng thêm các loại chuẩn mã định danh khác được áp dụng theo quy định của lĩnh vực quản lý chuyên ngành (ví dụ mã DOI, mã GS1,…).

Rõ ràng, mã định danh điện tử là một chuỗi kí tự sinh ra để dùng cho máy tính xử lý (thông qua quét hình ảnh QR Code). Nó thường dài và khó nhớ nên người dùng sẽ gặp khó khăn trong việc nhập mã vào các ứng dụng. Để khắc phục điểm yếu này, chúng ta có thể bổ sung vào lược đồ VODI một không gian mã định danh dùng cho tên riêng (vodi:TenGoi). Nếu như so sánh các mã định danh thông thường tương tự như địa chỉ IP của máy tính, thì định danh bằng tên riêng sẽ giống như tên miền dùng cho địa chỉ IP đó.

Ví dụ một cá nhân có thể được định danh thêm bằng tên riêng, chẳng hạn vodi:TenGoi:NguyenVanA, để ánh xạ với mã định danh điện tử dùng cho cá nhân dạng chữ số như vodi:CaNhan:001075123456. Một tổ chức hoạt động phi lợi nhuận sẽ được sự ủy quyền của Nhà nước để thực hiện thống nhất trong tổ chức quản lý việc đăng kí và sử dụng các mã định danh dùng tên riêng.

#### **Triển khai áp dụng hệ thống mã định danh điện tử thống nhất trong Chính phủ số**

Chuẩn mã định danh điện tử VODI có tính mở rất lớn để tất cả các cá nhân, tổ chức đều có thể tạo lập và chia sẻ dữ liệu số cùng với mã định danh điện tử do mình sinh ra. Chỉ cần có mã định danh được CQNN cấp sau khi đăng kí là các cá nhân, tổ chức đã có thể tham gia vào quá trình kết nối, chia sẻ dữ liệu của Chính phủ số. Cũng giống như việc sử dụng tên miền, các mã định danh điện tử do cá nhân, tổ chức sinh ra sẽ phải được đăng kí thông tin mô tả cho cơ quan quản lý các hệ thống phân giải mã định danh. Khi đó các ứng dụng chỉ cần quét QRCode biểu diễn mã định danh là có thể biết được đầy đủ các thông tin mô tả của đối tượng quản lý; đồng thời cũng có thể dẫn hướng truy cập vào địa chỉ trang web nơi chứa thông tin gốc.

Chúng ta cần áp dụng các chuẩn mở về công nghệ để không hạn chế số lượng các nhà cung cấp hệ thống phân giải mã định danh. Người dùng có quyền tự do lựa chọn nhà cung cấp để đăng kí thông tin mô tả cho các mã định danh điện tử mà mình tạo ra. Qua đó tạo ra sự cạnh tranh công bằng trong việc xây dựng hạ tầng kĩ thuật giúp kết nối, chia sẻ dữ liệu dùng cho Chính phủ số.

Sự ra đời của hệ thống mã định danh điện tử thống nhất sẽ là nền tảng kĩ thuật số dùng để liên thông, chia sẻ dữ liệu ở mức liên ngành trong toàn quốc. Giải pháp kĩ thuật đưa ra giúp giải quyết triệt để vấn đề hợp nhất các nguồn dữ liệu được quản lý phân mảnh tại các cơ quan, ngành, lĩnh vực khác nhau. Cùng với việc hình thành các cơ sở dữ liệu, kho dữ liệu dùng chung ở quy mô cấp Quốc gia, Bộ/ngành và Tỉnh thành \[1], việc kết nối, chia sẻ dữ liệu cũng sẽ trở nên thực sự thuận tiện và dễ dàng. Khi đó số lượng các ứng dụng được phát triển để khai thác và chia sẻ dữ liệu với các kho dùng chung sẽ không bị hạn chế, mà ngược lại càng nhiều thì càng tốt. Nó đối lập hoàn toàn với cách tiếp cận giải quyết các bất cập do không chia sẻ dữ liệu của nhiều ứng dụng hiện nay bằng việc xây dựng một ứng dụng duy nhất. Cách làm sau sẽ dẫn tới độc quyền, hạn chế sự cạnh tranh và làm lùi bước tiến trình chuyển đổi số của Chính phủ hiện nay.

Một Chính phủ số sẽ phải thực sự đóng vai trò là nền tảng (Government as a Platform). Chính phủ chỉ nên tập trung vào việc tạo dựng hạ tầng kĩ thuật cho việc kết nối, chia sẻ dữ liệu và chú trọng tới mở dữ liệu. Việc phát triển các ứng dụng cần được mở tự do và do thị trường quyết định. Huy động sức mạnh sáng tạo của toàn xã hội trong việc tạo ra các ứng dụng có ích cho người dùng sẽ thúc đẩy quá trình chuyển đổi số được thực hiện nhanh và hiệu quả nhất.

Trong Chính phủ số, tất cả dữ liệu tạo lập đều phải gắn với mã định danh điện tử để phục vụ kết nối, chia sẻ. Nó là một yêu cầu bắt buộc trong quản lý chất lượng của nguồn dữ liệu. Tất cả các dữ liệu không có mã định danh sẽ không được phép sử dụng làm nguồn chính thức trong các hoạt động quản lý của CQNN. Chúng sẽ chỉ có giá trị phục vụ làm nguồn tham khảo giống như các nguồn thông tin công cộng có thể bóc tách được dữ liệu từ trên mạng Internet./.

#### **Tài liệu tham khảo**

\[1] Tạ Tuấn Anh, “Mô hình kiến trúc và công nghệ xây dựng kho dữ liệu dùng chung phục vụ phát triển chính phủ số”. Tạp chí TT\&TT số 7 tháng 7/2021.
