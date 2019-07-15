# Unreal Engine 4 Style Guide Tiếng Việt
Vietnamese Translation on Allar UE4 Style Guide

Bảng dịch tiếng Việt tài liệu tiêu chuẩn làm việc cả code và blueprint Style Guide với Unreal Engine 4 dựa trên nguyên bản của [Allar](https://github.com/Allar/ue4-style-guide).

Theo nguyên bản Allar cho biết dựa theo rất nhiều trên [Airbnb Javascript Style Guide](https://github.com/airbnb/javascript).

Epic Games cũng có một bộ tiêu chuẩn dành cho coding C++, tham khảo thêm về [codebase ở đây](https://docs.unrealengine.com/en-US/Programming/Development/CodingStandard/index.html). 

## Unreal Engine 4 Linter Plugin
Allar có thiết kế một plugin giúp tự động kiểm soát các tài nguyên có trong project Unreal Engine 4 theo style guide, tuy nhiên hiện nay đã không còn hoạt động và không còn cập nhật với các bảng Unreal Engine mới, xem thêm tại market [the Unreal Engine marketplace](https://www.unrealengine.com/marketplace/linter).

## Thảo Luận Thêm Về Style Guide Này

Gamemakin LLC có một kênh Discord tại http://discord.gamemak.in với kênh #linter nếu như các bạn muốn thảo luận về mọi thứ liên quan style guid hay plugin Linter. 

## Liên Kết Tới Tài Liệu Của Allar Theo Đề Mục

Đây là liên kết do Allar tạo ra theo bảng gốc. 

Với mỗi phần của Allar style guide đã được đánh số để dễ tham khảo và dễ tạo liên kết tới. Bạn có thể liên kết tới bất cứ phần nào một cách trực tiếp bằng cách để một cái hash tag và đề mục số theo phần đó vào cuối cùng của chuỗi http://ue4.style.

Lấy ví dụ bạn muốn gửi ai đó phần đầu tiên của style guide, bạn sẽ cần bỏ thêm hash tag và đề mục số '#0.1' vào đầu chuỗi. Ví dụ: http://ue4.style#0.1 .

Phần biên dịch này vẫn giữ nguyên các hash tag tuy nhiên việc có tên miền riêng thì ai đó thấy hay, cứ donate tên miền tương ứng sẽ phù hợp hơn.

## Địa Phương Hóa Hay Biên Dịch

Với tư liệu gốc thì reposity của Allar không cho phép tạo thêm nhánh mà họ đề nghị tự tạo nhánh vào các reposity có sẵn đã dịch hoặc tự tạo mới.

* [Tiếng Việt](https://github.com/skylens-inc/ue4-style-guide/blob/master/README.md) bởi Vũ Phạm [@phamduongvu](https://twitter.com/phamduongvu) / [Rainstorm Film](https://www.rainstormfilm.com).
* [Tiếng Hàn Quốc](https://github.com/ymkim50/ue4-style-guide/blob/master/README_Kor.md) bởi ymkim50
* [Tiếng Nga](https://github.com/CosmoMyzrailGorynych/ue4-style-guide-rus/blob/master/README.md) bởi CosmoMyzrailGorynych
* [Tiếng Nhật](https://github.com/akenatsu/ue4-style-guide/blob/master/README.jp.md) bởi akenatsu
* [Tiếng Trung Quốc](https://github.com/skylens-inc/ue4-style-guide/blob/master/README.md) bởi Beijing Skylens Tech.

## Thuật Ngữ Quan Trọng

<a name="terms-level-map"></a>
##### Levels/Maps - cấp độ bản đồ, màn chơi

Từ "map" thông thường được chỉ đến như hiểu là "một màn chơi" và có thể sử dụng tùy theo ngữ cảnh. Để hiểu rõ hơn về lịch sử thuật ngữ màn chơi tham khảo thêm qua [Wikipedia ở đây](https://en.wikipedia.org/wiki/Level_(video_gaming).

<a name="terms-cases"></a>
##### Nhận Biết Chữ Hoa

Có nhiều cách thể hiện đặt tên khi lập trình hay làm việc với BluePrint. Đây là một số cách đặt tên có chữ hoa:

>###### PascalCase - Kiểu Pascal
>
>Viết hoa mọi chữ cái đầu một tự và không có khoảng trắng. Ví dụ như: `DesertEagle`, `StyleGuide`, `ASeriesOfWords`.

>###### camelCase - Kiểu Lạc Đà
>
>Cách này tương tự như viết code Java, chữ cái đầu tiên không viết hoa, mỗi từ liền sau đó đều viết hoa ký tự đầu tiên. Ví dụ: `desertEagle`, `styleGuide`, `aSeriesOfWords`.
>
>
>###### Snake_case - Kiểu Rắn
>
>Chữ cái đầu tiên có thể viết hoa hay không thì tùy nhưng mỗi từ cách nhau bằng dấu gạch dưới, cái này là kiểu viết code C++ trước đây. Ví dụ: `desert_Eagle`, `Style_Guide`, `a_Series_of_Words`.

<a name="terms-var-prop"></a>
##### Variables / Properties (Biến và Thuộc Tính)

Các từ biến và thuộc tính được sử dụng tùy theo ngữ cảnh. Đôi lúc cùng được sử dụng trong cùng một ngữ cảnh:

<a name="terms-property"></a>
###### Property (Thuộc Tính)

Thông thường sẽ được ref tới một biến đã được định nghĩa trong một class. Lấy ví dụ: nếu `BP_Barrel` đã có 1 biến `bExploded`, `bExploded` đôi lúc sẽ được hiểu là thuộc tính của class `BP_Barrel`.

When in the context of a class, often used to imply accessing previously defined data.

<a name="terms-variable"></a>
###### Variable (Biến)

Thường được biết là biến định nghĩa như tham số của hàm hoặc biến cục bộ trong một hàm.

Theo ngữ cảnh của một class, thường sẽ được hiểu như kiểu được định nghĩa và ý nghĩa của giá trị. 

<a name="0"></a>
## 0. Principles / Kỷ Luật

Các vấn đề đặt để và kỷ luật được lấy từ [idomatic.js style guide](https://github.com/rwaldron/idiomatic.js/).

<a name="0.1"></a>
### 0.1 Nếu dự án UE4 của bạn đã có một style guide, bạn nên làm theo

Nếu như bạn đang làm việc với một team đã có style guide thì bạn nên tông trọng làm theo dự án. Bất cứ mâu thuẫn nào giữa việc đã có style guide và thêm style guide này là không cần thiết.  

Style guide nên được cập nhật liên tục và cũng nên được đổi mới nếu có lợi ích sử dụng.

>#### "Arguments over style are pointless. There should be a style guide, and you should follow it."
>[_Rebecca Murphey_](https://rmurphey.com)

>Tranh cãi cách viết code là vô nghĩa. Chỉ cần có một style guid và nên theo nó.

>####"Part of being a good steward to a successful project is realizing that writing code for yourself is a Bad Idea™. If thousands of people are using your code, then write your code for maximum clarity, not your personal preference of how to get clever within the spec."
>[_Idan Gazit_](https://twitter.com/idangazit)

>Cách để một dự án thành công là không tôn sùng việc viết code theo chủ nghĩa cá nhân. Nếu như code của bạn được sử dụng bởi người khác, thì viết code cần phải rõ ràng, không chỉ để tham khảo cá nhân hay làm cho mọi thứ ghê ghớm lên.

<a name="0.2"></a>
### 0.2 Mọi cấu trúc, tài nguyên, và code trong UE4 cần được thống nhất như một người viết, không cần biết bao nhiêu người cống hiến

Chuyển từ một dự án này sang cái khác cần sự dễ dàng, không phải tạo ra việt đào tạo lại về style và cấu trúc. Thoải mái với một style guide đồng nhất sẽ tránh việc tự đoán hay mù mờ.

Nó cũng giúp tăng năng suất làm việc và duy trì năng suất, chỉ cần đi theo các chỉ thị nhiệm vụ. Đây là một style guide được thực tiễn hóa tốt nhất, theo style guide này sẽ giúp tối thiểu hóa khó khăn khi giải quyết vấn đề.

<a name="0.3"></a>
### 0.3 Đừng để bạn bè tạo ra các style tồi 

Cố gắn điều chỉnh những ai đang không theo style guide này hoặc đang làm việc mà không có style nào. 

Khi làm việc trong một team hay đang thảo luận ở discord [Unreal Slackers](http://join.unrealslackers.org/), sẽ dễ dàng nhận được giúp đỡ hay giúp ai đó khi mọi thứ đồng nhất. Không ai muốn giúp một phiên bản Blueprint nhầy nhụa hay phải xử lý tài nguyên với những định danh khó hiểu. 

Nếu như bạn đang giúp ai đó mà họ đang làm việc trên một style guide khác nhưng đồng nhất, bạn nên theo họ. Nếu họ không có bất cứ style guide nào thì chỉ họ về tài liệu này.

<a name="0.4"></a>
### 0.4 Nếu một đội dự án không có style guid thì đó không phải đội của tôi

Lần đầu tiên tham gia một đội ngũ làm Unreal Engine 4, bạn nên đặt câu hỏi xem liệu họ có làm việc trên một style guide không. Nếu câu trả lời là không bạn cần thấy nghi ngờ về khả năng thực hiện công việc của đội này.

<a name="0.5"></a>
### 0.5 Đừng có phá luật

Gamemakin LLC không phải là một luật sư, nhưng đừng cố tạo ra các hành động phạm pháp khi làm việc trên một dự án UE4, bao gồm không giới hạn:

* Đừng phân phối nội dung không có bản quyền
* Đừng lấy tài liệu bản quyền hay tài nguyên sỡ hữu của bất cứ ai
* Đừng đánh cắp nội dung
* Theo rõ chỉ thị hay nội qui của nội dung

<a name="toc"></a>
## Mục Lục Nội Dung Chính Của Unreal Engine Style Guide Bản Tiếng Việt

1. [Tiêu Chuẩn Đặt Tên tài Nguyên](#anc)
1. [Cấu Trúc Thư Mục](#structure)
1. [Blueprints](#bp)
1. [Static Meshes](#s)
1. [Particle Systems](#ps)
1. [Levels / Maps](#levels)
1. [Textures](#textures)