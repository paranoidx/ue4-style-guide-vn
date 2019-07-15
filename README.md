# Unreal Engine 4 Style Guide Tiếng Việt
Vietnamese Translation on Allar UE4 Style Guide

Bảng dịch tiếng Việt tài liệu tiêu chuẩn (style guide) làm việc cả code và blueprint Style Guide với Unreal Engine 4 dựa trên nguyên bản của [Allar](https://github.com/Allar/ue4-style-guide).

Bảng dịch này có đóng góp thêm của người dịch [@Vũ Phạm](https://twitter.com/phamduongvu), không ghi chú trong tiêu chuẩn vị trí đóng góp. 

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

Phần biên dịch này vẫn giữ nguyên các hash tag tuy nhiên việc có tên miền riêng thì ai đó thấy hay, cứ donate tên miền tương ứng sẽ phù hợp hơn. Hoặc dùng chính liên kết ở đây https://github.com/paranoidx/ue4-style-guide-vn và thêm hash tag #, ví dụ: https://github.com/paranoidx/ue4-style-guide-vn#0.1

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
>Viết hoa mọi chữ cái đầu một từ và không có khoảng trắng. Ví dụ như: `DesertEagle`, `StyleGuide`, `ASeriesOfWords`.
>
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

>Tranh cãi cách viết code là vô nghĩa. Chỉ cần có một style guide và nên làm theo nó.

>#### "Part of being a good steward to a successful project is realizing that writing code for yourself is a Bad Idea™. If thousands of people are using your code, then write your code for maximum clarity, not your personal preference of how to get clever within the spec."
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

Điều này cũng nên áp dụng tương tự cho các group thảo luận về Unreal Engine ở Việt Nam trên Facebook như [Cộng Đồng Unreal Engine Việt](https://www.facebook.com/groups/unrealvn/).

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

1. [Tiêu Chuẩn Đặt Tên Tài Nguyên](#anc)
1. [Cấu Trúc Thư Mục](#structure)
1. [Blueprints](#bp)
1. [Static Meshes](#s)
1. [Particle Systems](#ps)
1. [Levels / Maps](#levels)
1. [Textures](#textures)

<a name="anc"></a>
<a name="1"></a>
## 1.Tiêu Chuẩn Đặt Tên Tài Nguyên 

Cách viết code tiêu chuẩn là phải đặt nặng vấn đề định danh một cách nghiêm ngặt. Một dự án có cách định danh tiêu chuẩn sẽ giúp dễ quản lý tài nguyên, tìm kiếm, đối chiếu tham khảo hay duy trì một cách nhẹ nhàng.

Đa số được sử dụng đánh dấu với prefixes chữ cái đầu tiên của từ định danh kiểu tài nguyên và thêm dấu gạch dưới.

<a name="base-asset-name"></a>
<a name="1.1"></a>
### 1.1 Định Danh Gốc Tên Tài Nguyên / Base Asset Name - `Prefix_BaseAssetName_Variant_Suffix`

>Ví dụ: Material Nhân Vat - M_Character (nên sử dụng định danh trong dự án là tiếng Anh nếu bạn muốn dễ dàng đặt câu hỏi, nhờ giúp đỡ hay làm việc với các developer trên thế giới).

>Hay thêm ví dụ: Texture Nhan Vat Phan Dien Diffuse - T_NhanVat_Evil_D 

Tất cả tài nguyên nên được có tên gốc _Base Asset Name_
Một cái tên gốc sẽ giúp nhóm hoặc liên hệ tài nguyên liên quan. Mọi tài nguyên tiếp diễn dưới dạng thuộc nhóm hệ cây theo tên này nên theo tiêu chuẩn `Prefix_BaseAssetName_Variant_Suffix`. 

Giữ nguyên mô hình `Prefix_BaseAssetName_Variant_Suffix` và sử dụng từ dễ hiểu cho định danh tài nguyên. Vài chi tiết tham khảo thêm dưới đây về qui luật.

`Prefix` và `Suffix` được hiểu như kiểu tài nguyên theo bảng [Asset Name Modifier](#asset-name-modifiers).

`BaseAssetName` - định danh gốc nên ngắn và dễ hiểu theo ngữ cảnh trong nhóm tài nguyên. Lấy ví dụ nếu như có một nhân vật tên Bob, mọi tài nguyên của Bob nên theo tên gốc `BaseAssetName` là `Bob`.

Để đảm bảo tính duy nhất (unique) và cụ thể hóa những biến đổi (variations - `Variant` - biến thể) theo sau tên của tài nguyên, `Variant` nên ngắn, dễ hiểu, thể hiện được tên thuộc về một nhóm tài nguyên mà nó là thành phần phụ (thành phần con) của định danh gốc. Lấy ví dụ nếu nhân vật Bob có nhiều skin biến thể khác nhau thì định danh gốc vẫn là `Bob` nhưng thêm biến đổi, như skin Evil sẽ thêm `Bob_Evil` và skin 'Retro' sẽ thêm `Bob_Retro`.

Để mang tính duy nhất nhưng có biến đổi chung chung của định danh tài nguyên, `Variant` sẽ là loại số bắt đầu bởi 01. Lấy ví dụ như tài nguyên mô hình 3D là các viên đá, nên được đặt tên `Rock_01`, `Rock_02`, `Rock_03`, ... 
Ngoại trừ vài ngoại lệ thì bạn gần như không cần thêm số có ba chữ số vào phần biến đổi. Nếu có hơn 100 tài nguyên, bạn nên cân nhắc để thêm định danh gốc hoặc sử dụng thêm biến thể về tên.  

Bạn có thể kết nối các biến thể tên tài nguyên với nhau theo loại tài nguyên tạo ra. Lấy ví dụ như bạn đang tạo ra một tài nguyên là mặt nền cho dự án [diễn họa kiến trúc](https://lamphimquangcao.tv/cach-mang-hoa-trong-nganh-dien-hoa-kien-truc/), bạn nên đặt tên theo cách sau đây với định danh gốc là:  `Flooring` và thêm xâu chuỗi mắc xích biến thể như `Flooring_Marble_01`, `Flooring_Maple_01`, `Flooring_Tile_Squares_01`.

<a name="1.1-examples"></a>
#### 1.1 Tổng Hợp Các Ví Dụ Định Danh Và Biến Thể

##### 1.1e1 Bob (lấy ví dụ nhân vật Bob)

| Kiểu Tài Nguyên             | Tên Tài Nguyên                                                  |
| ----------------------- | ---------------------------------------------------------- |
| Skeletal Mesh           | SK_Bob                                                     |
| Material                | M_Bob                                                      |
| Texture (Diffuse/Albedo)| T_Bob_D                                                    |
| Texture (Normal)        | T_Bob_N                                                    |
| Texture (Evil Diffuse)  | T_Bob_Evil_D                                               |

##### 1.1e2 Rocks (các loại mô hình 3D đá)

| Kiểu Tài Nguyên              | Tên Tài Nguyên                                                 |
| ----------------------- | ---------------------------------------------------------- |
| Static Mesh (01)        | S_Rock_01                                                  |
| Static Mesh (02)        | S_Rock_02                                                  |
| Static Mesh (03)        | S_Rock_03                                                  |
| Material                | M_Rock                                                     |
| Material Instance (Snow)| MI_Rock_Snow                                               |

<a name="asset-name-modifiers"></a>
<a name="1.2"></a>
### 1.2 Thêm Biến Thể Định Danh 

Khi định danh tài nguyên nên sử dụng tham khảo theo bảng tên dưới đây để thêm prefix và suffix vào định danh gốc [Base Asset Name](#base-asset-name).

#### Hạng Mục

> 1.2.1 [Thông Thường Chung Chung](#anc-common)

> 1.2.2 [Animations](#anc-animations)

> 1.2.3 [Artificial Intelligence - AI](#anc-ai)

> 1.2.4 [Blueprints](#anc-bp)

> 1.2.5 [Materials](#anc-materials)

> 1.2.6 [Textures](#anc-textures)

> 1.2.7 [Miscellaneous](#anc-misc)

> 1.2.8 [Paper 2D](#anc-paper2d)

> 1.2.9 [Physics](#anc-physics)

> 1.2.10 [Sound](#anc-sounds)

> 1.2.11 [User Interface](#anc-ui)

> 1.2.12 [Effects](#anc-effects)

<a name="anc-common"></a>
<a name="1.2.1"></a>
#### 1.2.1 Thông Thường Chung Chung

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Level / Map / Màn Chơi             |            |            | [Nên Được Để Trong Thư Mục "Maps"](#2.4) |
| Level (Persistent)      |            | _P         |                                  |
| Level (Audio)           |            | _Audio     |                                  |
| Level (Lighting)        |            | _Lighting  |                                  |
| Level (Geometry)        |            | _Geo       |                                  |
| Level (Gameplay)        |            | _Gameplay  |                                  |
| Blueprint               | BP_        |            |                                  |
| Material                | M_         |            |                                  |
| Static Mesh             | S_         |            | Có nhiều người dùng SM_. Chúng ta dùng S_.         |
| Skeletal Mesh           | SK_        |            |                                  |
| Texture                 | T_         | _?         | Xem thêm [Textures](#anc-textures)    |
| Particle System         | PS_        |            |                                  |
| Widget Blueprint        | WBP_       |            |                                  |

<a name="anc-animations"></a>
<a name="1.2.2"></a>
#### 1.2.2 Animations ![#](https://img.shields.io/badge/lint-supported-green.svg)

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Aim Offset              | AO_        |            |                                  |
| Aim Offset 1D           | AO_        |            |                                  |
| Animation Blueprint     | ABP_       |            |                                  |
| Animation Composite     | AC_        |            |                                  |
| Animation Montage       | AM_        |            |                                  |
| Animation Sequence      | A_         |            |                                  |
| Blend Space             | BS_        |            |                                  |
| Blend Space 1D          | BS_        |            |                                  |
| Level Sequence          | LS_        |            |                                  |
| Morph Target            | MT_        |            |                                  |
| Paper Flipbook          | PFB_       |            |                                  |
| Rig                     | Rig_       |            |                                  |
| Skeletal Mesh           | SK_        |            |                                  |
| Skeleton                | SKEL_      |            |                                  |

<a name="anc-ai"></a>
<a name="1.2.3"></a>
### 1.2.3 Artificial Intelligence (AI)

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| AI Controller           | AIC_       |            |                                  |
| Behavior Tree           | BT_        |            |                                  |
| Blackboard              | BB_        |            |                                  |
| Decorator               | BTDecorator_ |          |                                  |
| Service                 | BTService_ |            |                                  |
| Task                    | BTTask_    |            |                                  |
| Environment Query       | EQS_       |            |                                  |
| EnvQueryContext         | EQS_       | Context    |                                  |

<a name="anc-bp"></a>
<a name="1.2.4"></a>
### 1.2.4 Blueprints 

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Blueprint               | BP_        |            |                                  |
| Blueprint Component	  | BP_	       | Component  | I.e. BP_InventoryComponent       |
| Blueprint Function Library | BPFL_   |            |                                  |
| Blueprint Interface     | BPI_       |            |                                  |
| Blueprint Macro Library | BPML_      |            | Không nên sử dụng macro libraries nếu có thể được. |
| Enumeration             | E          |            | Không có Gạch Dưới (_).                   |
| Structure               | F or S     |            | Không có Gạch Dưới (_).                   |
| Tutorial Blueprint      | TBP_       |            |                                  |
| Widget Blueprint        | WBP_       |            |                                  |

<a name="anc-materials"></a>
<a name="1.2.5"></a>
### 1.2.5 Materials 

| Kiểu Tài Nguyên                    | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------------- | ---------- | ---------- | -------------------------------- |
| Material                      | M_         |            |                                  |
| Material (Post Process)       | PP_        |            |                                  |
| Material Function             | MF_        |            |                                  |
| Material Instance             | MI_        |            |                                  |
| Material Parameter Collection | MPC_       |            |                                  |
| Subsurface Profile            | SP_        |            |                                  |
| Physical Materials            | PM_        |            |                                  |
| Decal                         | M_, MI_    | _Decal     |                                  |

<a name="anc-textures"></a>
<a name="1.2.6"></a>
### 1.2.6 Textures 

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Texture                 | T_         |            |                                  |
| Texture (Diffuse/Albedo/Base Color)| T_ | _D      |                                  |
| Texture (Normal)        | T_         | _N         |                                  |
| Texture (Roughness)     | T_         | _R         |                                  |
| Texture (Alpha/Opacity) | T_         | _A         |                                  |
| Texture (Ambient Occlusion) | T_     | _O         |                                  |
| Texture (Bump)          | T_         | _B         |                                  |
| Texture (Emissive)      | T_         | _E         |                                  |
| Texture (Mask)          | T_         | _M         |                                  |
| Texture (Specular)      | T_         | _S         |                                  |
| Texture (Metallic)      | T_         | _M         |                                  |
| Texture (Packed)        | T_         | _*         | Xem thêm ghi chú phía dưới [đóng gói - packing](#anc-textures-packing). |
| Texture Cube            | TC_        |            |                                  |
| Media Texture           | MT_        |            |                                  |
| Render Target           | RT_        |            |                                  |
| Cube Render Target      | RTC_       |            |                                  |
| Texture Light Profile   | TLP        |            |                                  |

<a name="anc-textures-packing"></a>
<a name="1.2.6.1"></a>
#### 1.2.6.1 Texture Packing 

Rất phổ biến có thể thấy khi đóng gói nhiều lớp dữ liệu texture vào trong một file texture. Ví dụ của việc này là khi đóng gói Emissive, Roughness, Ambient Occlusion chung với kênh màu (R, G, B) của file hình. Để nhận ra được suffix, chỉ cần đơn giản chồng thêm suffix theo bảng trên. Lấy ví dụ: `_ERO`.

> Chấp nhận được để bao gồm thêm lớp Alpha/Opacity vào trong kênh alpha của Diffuse/Albedo, thêm suffix `A` với `_D` tùy chọn.

Gói 4 kênh dữ liệu vào trong một file texture (RGBA) là không nên ngoại trừ mask Alpha/Opacity trong kênh alpha của Diffuse/Albedo như một file texture có kênh alpha.

<a name="anc-misc"></a>
<a name="1.2.7"></a>
### 1.2.7 Miscellaneous - Linh Tinh 

| Kiểu Tài Nguyên                 | Prefix     | Suffix     | Ghi Chú                            |
| -------------------------- | ---------- | ---------- | -------------------------------- |
| Animated Vector Field      | VFA_       |            |                                  |
| Camera Anim                | CA_        |            |                                  |
| Color Curve                | Curve_     | _Color     |                                  |
| Curve Table                | Curve_     | _Table     |                                  |
| Data Asset                 | *_         |            | Prefix nên dựa theo class. |
| Data Table                 | DT_        |            |                                  |
| Float Curve                | Curve_     | _Float     |                                  |
| Foliage Type               | FT_        |            |                                  |
| Force Feedback Effect      | FFE_       |            |                                  |
| Landscape Grass Type       | LG_        |            |                                  |
| Landscape Layer            | LL_        |            |                                  |
| Matinee Data               | Matinee_   |            |                                  |
| Media Player               | MP_        |            |                                  |
| Object Library             | OL_        |            |                                  |
| Redirector                 |            |            | 'Phần này cần được chỉnh sửa sớm' .   |
| Sprite Sheet               | SS_        |            |                                  |
| Static Vector Field        | VF_        |            |                                  |
| Substance Graph Instance   | SGI_       |            |                                  |
| Substance Instance Factory | SIF_       |            |                                  |
| Touch Interface Setup      | TI_        |            |                                  |
| Vector Curve               | Curve_     | _Vector    |                                  |

<a name="anc-paper2d"></a>
<a name="1.2.8"></a>
### 1.2.8 Paper 2D ![#](https://img.shields.io/badge/lint-supported-green.svg)

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Paper Flipbook          | PFB_       |            |                                  |
| Sprite                  | SPR_       |            |                                  |
| Sprite Atlas Group      | SPRG_      |            |                                  |
| Tile Map                | TM_        |            |                                  |
| Tile Set                | TS_        |            |                                  |

<a name="anc-physics"></a>
<a name="1.2.9"></a>
### 1.2.9 Physics ![#](https://img.shields.io/badge/lint-supported-green.svg)

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Physical Material       | PM_        |            |                                  |
| Physical Asset	  | PHYS_      |            |                                  |
| Destructible Mesh       | DM_        |            |                                  |

<a name="anc-sounds"></a>
<a name="1.2.10"></a>
### 1.2.10 Sounds - Âm Thanh 

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Dialogue Voice          | DV_        |            |                                  |
| Dialogue Wave           | DW_        |            |                                  |
| Media Sound Wave        | MSW_       |            |                                  |
| Reverb Effect           | Reverb_    |            |                                  |
| Sound Attenuation       | ATT_       |            |                                  |
| Sound Class             |            |            | Không để prefix/suffix. Nên đặt vào thư mục SoundClasses |
| Sound Concurrency       |            | _SC        | Nên đặt tên theo sau một class SoundClass |
| Sound Cue               | A_         | _Cue       |                                  |
| Sound Mix               | Mix_       |            |                                  |
| Sound Wave              | A_         |            |                                  |

<a name="anc-ui"></a>
<a name="1.2.11"></a>
### 1.2.11 User Interface - Giao Diện

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Font                    | Font_      |            |                                  |
| Slate Brush             | Brush_     |            |                                  |
| Slate Widget Style      | Style_     |            |                                  |
| Widget Blueprint        | WBP_       |            |                                  |

<a name="anc-effects"></a>
<a name="1.2.12"></a>
### 1.2.12 Effects - Hiệu Ứng 

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Particle System         | PS_        |            |                                  |
| Material (Post Process) | PP_        |            |                                  |

**[⬆ Trở Về Đầu Mục Lục](#table-of-contents)**