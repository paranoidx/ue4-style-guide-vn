# Unreal Engine 4 Style Guide Tiếng Việt
Vietnamese Translation on Allar UE4 Style Guide

Bảng dịch tiếng Việt tài liệu tiêu chuẩn làm việc cả code và blueprint Style Guide với Unreal Engine 4 dựa trên nguyên bản của [Allar](https://github.com/Allar/ue4-style-guide).

Theo nguyên bản Allar cho biết dựa theo rất nhiều trên [Airbnb Javascript Style Guide](https://github.com/airbnb/javascript).

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

* [Tiếng Việt](https://github.com/skylens-inc/ue4-style-guide/blob/master/README.md) bởi Vũ Phạm / [Rainstorm Film](https://www.rainstormfilm.com).
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

###### PascalCase - Kiểu Pascal

Viết hoa mọi chữ cái đầu một tự và không có khoảng trắng. Ví dụ như: `DesertEagle`, `StyleGuide`, `ASeriesOfWords`.

###### camelCase - Kiểu Lạc Đà

Cách này tương tự như viết code Java, chữ cái đầu tiên không viết hoa, mỗi từ liền sau đó đều viết hoa ký tự đầu tiên. Ví dụ: `desertEagle`, `styleGuide`, `aSeriesOfWords`.


###### Snake_case - Kiểu Rắn

Chữ cái đầu tiên có thể viết hoa hay không thì tùy nhưng mỗi từ cách nhau bằng dấu gạch dưới, cái này là kiểu viết code C++ trước đây. Ví dụ: `desert_Eagle`, `Style_Guide`, `a_Series_of_Words`.

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
## 0. Principles

These principles have been adapted from [idomatic.js style guide](https://github.com/rwaldron/idiomatic.js/).