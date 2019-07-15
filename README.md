# Unreal Engine 4 Style Guide Tiếng Việt
Vietnamese Translation on Allar UE4 Style Guide

Bảng dịch tiếng Việt tài liệu tiêu chuẩn (style guide) làm việc cả code và blueprint Style Guide với Unreal Engine 4 dựa trên nguyên bản của [Allar](https://github.com/Allar/ue4-style-guide).

Bảng dịch này có đóng góp thêm của người dịch [@Vũ Phạm](https://twitter.com/phamduongvu), không ghi chú trong tiêu chuẩn vị trí đóng góp. 

Theo nguyên bản Allar cho biết dựa theo rất nhiều trên [Airbnb Javascript Style Guide](https://github.com/airbnb/javascript).

Epic Games cũng có một bộ tiêu chuẩn dành cho coding C++, tham khảo thêm về [codebase ở đây](https://docs.unrealengine.com/en-US/Programming/Development/CodingStandard/index.html). 

Hiểu về cách định dạng văn bản của file README.MD theo GitHub nên tham khảo tài liệu của GitHub về [GitHub formatting ở đây](https://help.github.com/en/enterprise/2.17/user/articles/basic-writing-and-formatting-syntax)

## Unreal Engine 4 Linter Plugin
Allar có thiết kế một plugin giúp tự động kiểm soát các tài nguyên (asset) có trong project Unreal Engine 4 theo style guide, tuy nhiên hiện nay đã không còn hoạt động và không còn cập nhật với các bảng Unreal Engine mới, xem thêm tại market [the Unreal Engine marketplace](https://www.unrealengine.com/marketplace/linter).

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
##### Cách Nhận Biết Chữ Hoa

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
>
>Tranh cãi cách viết code là vô nghĩa. Chỉ cần có một style guide và nên làm theo nó.

>#### "Part of being a good steward to a successful project is realizing that writing code for yourself is a Bad Idea™. If thousands of people are using your code, then write your code for maximum clarity, not your personal preference of how to get clever within the spec."
>[_Idan Gazit_](https://twitter.com/idangazit)
>
>Cách để một dự án thành công là không tôn sùng việc viết code theo chủ nghĩa cá nhân. Nếu như code của bạn được sử dụng bởi người khác, thì viết code cần phải rõ ràng, không chỉ để tham khảo cá nhân hay làm cho mọi thứ ghê ghớm lên.

<a name="0.2"></a>
### 0.2 Mọi cấu trúc, tài nguyên (asset), và code trong UE4 cần được thống nhất như một người viết, không cần biết bao nhiêu người cống hiến

Chuyển từ một dự án này sang cái khác cần sự dễ dàng, không phải tạo ra việt đào tạo lại về style và cấu trúc. Thoải mái với một style guide đồng nhất sẽ tránh việc tự đoán hay mù mờ.

Nó cũng giúp tăng năng suất làm việc và duy trì năng suất, chỉ cần đi theo các chỉ thị nhiệm vụ. Đây là một style guide được thực tiễn hóa tốt nhất, theo style guide này sẽ giúp tối thiểu hóa khó khăn khi giải quyết vấn đề.

<a name="0.3"></a>
### 0.3 Đừng để đồng đội tạo ra các style tồi 

Cố gắng điều chỉnh những ai đang không theo style guide này hoặc đang làm việc mà không có style nào. 

Khi làm việc trong một team hay đang thảo luận ở discord [Unreal Slackers](http://join.unrealslackers.org/), sẽ dễ dàng nhận được giúp đỡ hay giúp ai đó khi mọi thứ đồng nhất. Không ai muốn giúp một phiên bản Blueprint nhầy nhụa hay phải xử lý tài nguyên (asset) với những định danh khó hiểu. 

Điều này cũng nên áp dụng tương tự cho các group thảo luận về Unreal Engine ở Việt Nam trên Facebook như [Cộng Đồng Unreal Engine Việt](https://www.facebook.com/groups/unrealvn/).

Nếu như bạn đang giúp ai đó mà họ đang làm việc trên một style guide khác nhưng đồng nhất, bạn nên theo họ. Nếu họ không có bất cứ style guide nào thì chỉ họ về tài liệu này.

<a name="0.4"></a>
### 0.4 Nếu một đội dự án không có style guid thì đó không phải đội của tôi

Lần đầu tiên tham gia một đội ngũ làm Unreal Engine 4, bạn nên đặt câu hỏi xem liệu họ có làm việc trên một style guide không. Nếu câu trả lời là không bạn cần thấy nghi ngờ về khả năng thực hiện công việc của đội này.

<a name="0.5"></a>
### 0.5 Đừng có phá luật

Gamemakin LLC không phải là một luật sư, nhưng đừng cố tạo ra các hành động phạm pháp khi làm việc trên một dự án UE4, bao gồm không giới hạn:

* Đừng phân phối nội dung không có bản quyền
* Đừng lấy tài liệu bản quyền hay tài nguyên (asset) sỡ hữu của bất cứ ai
* Đừng đánh cắp nội dung
* Theo rõ chỉ thị hay nội qui của nội dung

<a name="table-of-contents"></a>
## Mục Lục Nội Dung Chính Của Unreal Engine Style Guide Bản Tiếng Việt

1. [Tiêu Chuẩn Đặt Tên Tài Nguyên (asset)](#anc)
1. [Cấu Trúc Thư Mục](#structure)
1. [Blueprints](#bp)
1. [Static Meshes](#s)
1. [Particle Systems](#ps)
1. [Levels / Maps](#levels)
1. [Textures](#textures)

<a name="anc"></a>
<a name="1"></a>
## 1.Tiêu Chuẩn Đặt Tên Tài Nguyên (asset) 

Cách viết code tiêu chuẩn là phải đặt nặng vấn đề định danh một cách nghiêm ngặt. Một dự án có cách định danh tiêu chuẩn sẽ giúp dễ quản lý tài nguyên (asset), tìm kiếm, đối chiếu tham khảo hay duy trì một cách nhẹ nhàng.

Đa số được sử dụng đánh dấu với prefixes chữ cái đầu tiên của từ định danh kiểu tài nguyên và thêm dấu gạch dưới.

<a name="base-asset-name"></a>
<a name="1.1"></a>
### 1.1 Định Danh Gốc Tên Tài Nguyên / Base Asset Name - `Prefix_BaseAssetName_Variant_Suffix`

>Ví dụ: Material Nhân Vat - M_Character (nên sử dụng định danh trong dự án là tiếng Anh nếu bạn muốn dễ dàng đặt câu hỏi, nhờ giúp đỡ hay làm việc với các developer trên thế giới).
>
>Hay thêm ví dụ: Texture Nhân Vật Phản Diện Kênh Diffuse - T_NhanVat_Evil_D 

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
>
> 1.2.2 [Animations](#anc-animations)
>
> 1.2.3 [Artificial Intelligence - AI](#anc-ai)
>
> 1.2.4 [Blueprints](#anc-bp)
>
> 1.2.5 [Materials](#anc-materials)
>
> 1.2.6 [Textures](#anc-textures)
>
> 1.2.7 [Miscellaneous](#anc-misc)
>
> 1.2.8 [Paper 2D](#anc-paper2d)
>
> 1.2.9 [Physics](#anc-physics)
>
> 1.2.10 [Sound](#anc-sounds)
>
> 1.2.11 [User Interface](#anc-ui)
>
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
#### 1.2.2 Animations 

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
### 1.2.8 Paper 2D 

| Kiểu Tài Nguyên              | Prefix     | Suffix     | Ghi Chú                            |
| ----------------------- | ---------- | ---------- | -------------------------------- |
| Paper Flipbook          | PFB_       |            |                                  |
| Sprite                  | SPR_       |            |                                  |
| Sprite Atlas Group      | SPRG_      |            |                                  |
| Tile Map                | TM_        |            |                                  |
| Tile Set                | TS_        |            |                                  |

<a name="anc-physics"></a>
<a name="1.2.9"></a>
### 1.2.9 Physics 

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

<a name="2"></a>
<a name="structure"></a>
## 2. Content Directory Structure

Cũng quan trọng giống như định danh tên tài nguyên, cấu trúc thư mục của một dự án cũng phải theo một qui luật. Tiêu chuẩn định danh tài nguyên và nội dung cấu trúc thư mục là đi cùng nhau, phá luật chỉ đem lại khủng hoảng và xào xáo tài nguyên dự án không cần thiết.

Có nhiều cách để sắp xếp nội dung của một dự án UE4. Với cách sắp xếp thư mục đang đề ra sẽ cho phép chọn lọc (fileter) và tìm kiếm thông qua Content Browser để những ai làm việc và tìm tài nguyên của kiểu tài nguyên cụ thể thay vì cấu trúc thông thường là nhóm các kiểu tài nguyên vào một folder.

> Nếu như bạn đang dùng prefix

> If you are using the prefix [Thêm Biến Thể Định Danh ](#1.2) như trên, việc dùng folder để chứa tài nguyên cùng kiểu như `Meshes`, `Textures`, và `Materials` là kém thực tiễn vì kiểu tài nguyên đã được dễ dàng sắp xếp theo prefix cũng như chọn lọc (filter) trong Content Browser.

<a name="2e1"><a>
### 2e1 Ví Dụ Cấu Trúc Thư Mục Dự Án
<pre>
|-- Content
    |-- <a href="#2.2">GenericShooter</a>
        |-- Art (Tài Nguyên Nghệ Thuật)
        |   |-- Industrial
        |   |   |-- Ambient
        |   |   |-- Machinery
        |   |   |-- Pipes
        |   |-- Nature
        |   |   |-- Ambient
        |   |   |-- Foliage
        |   |   |-- Rocks
        |   |   |-- Trees
        |   |-- Office
        |-- Characters (Tài Nguyên Nhân Vật)
        |   |-- Bob
        |   |-- Common
        |   |   |-- <a href="#2.7">Animations</a>
        |   |   |-- Audio
        |   |-- Jack
        |   |-- Steve
        |   |-- <a href="#2.1.3">Zoe</a>
        |-- <a href="#2.5">Core</a> (Phần lõi)
        |   |-- Characters
        |   |-- Engine
        |   |-- <a href="#2.1.2">GameModes</a>
        |   |-- Interactables
        |   |-- Pickups
        |   |-- Weapons
        |-- Effects (Hiệu Ứng)
        |   |-- Electrical
        |   |-- Fire
        |   |-- Weather
        |-- <a href="#2.4">Maps</a> (Màn Chơi)
        |   |-- Campaign1
        |   |-- Campaign2
        |-- <a href="#2.8">MaterialLibrary</a> (Thư Viện Vật Liệu)
        |   |-- Debug
        |   |-- Metal
        |   |-- Paint
        |   |-- Utility
        |   |-- Weathering
        |-- Placeables (Các Sự Kiện Nhặt, Lượm, Loot)
        |   |-- Pickups
        |-- Weapons (Vũ Khí)
            |-- Common
            |-- Pistols
            |   |-- DesertEagle
            |   |-- RocketPistol
            |-- Rifles
</pre>

Nguyên nhân theo cấu trúc này được liệt kê theo hạng mục phụ phía dưới đây.

### Các Hạng Mục 

> 2.1 [Tên Thư Mục](#structure-folder-names)
>
> 2.2 [Top-Level Folders / Thư Mục Trên Cùng](#structure-top-level)
>
> 2.3 [Developer Folders / Thư Mục Dev](#structure-developers)
>
> 2.4 [Maps / Màn Chơi](#structure-maps)
>
> 2.5 [Core / Lõi](#structure-core)
>
> 2.6 [`Assets` và `AssetTypes`](#structure-assettypes)
>
> 2.7 [Large Sets](#structure-large-sets)
>
> 2.8 [Material Library / Thư Viện Vật Liệu](#structure-material-library)

<a name="2.1"></a>
<a name="structure-folder-names"><a>
### 2.1 Folder Names

Đây là các qui luật thông thường đặt tên folder trong một cấu trúc nội dung.

<a name="2.1.1"></a>
#### 2.1.1 Luôn Sử Dụng [PascalCase](#terms-cases)

**PascalCase** chỉ đến cách đặt tên với một ký tự viết hoa và thay vì dùng dấu cách - khoảng trắng giữa các từ, mỗi từ liền kề nhau với ký tự hoa đầu tiên của từ. Lấy ví dụ: `DesertEagle`, `RocketPistol`, và `ASeriesOfWords`.

* *Xem thêm về [Cách Nhận Biết Chữ Hoa](#terms-cases)* *

<a name="2.1.2"></a>
#### 2.1.2 Không Bao Giờ Dùng Dấu Cách - Khoảng Trắng

Nhấn mạnh [2.1.1](#2.1.1), không bao giờ dùng dấu cách. Dấu cách sẽ làm fail các công cụ và các xử lý hàng loạt. Lý tưởng nhất phần root của dự án cũng không nên đặt dấu cách và đặt ở nào đó không phải là phần vùng hệ thống, ví dụ: `D:\Project` thay vì để ở `C:\Users\My Name\My Documents\Unreal Projects` 

<a name="2.1.3"></a>
#### 2.1.3 Không Bao Giờ Dùng Ký Tự Unicode Hay Các Kiểu Symbol

Nếu tên của một trong các nhân vật được đặt tên là **'Zoë'**, tên của folder nên là `Zoe`. Các ký tự Unicode còn tệ hơn [khoảng trắng - dấu cách](#2.1.2), nó làm cho FAIL khi xử lý từ các công cụ hay các thành phần của UE4 không hỗ trợ Unicode hay cả phần đường dẫn.

Cũng thêm vào đó, nếu dự án của bạn có các [lỗi không giải thích được](https://answers.unrealengine.com/questions/101207/undefined.html) và máy tính của bạn có user name là ký tự Unicode, lấy ví dụ tên bạn là `Zoë`, mọi dự án đang được lưu tại folder `My Documents` sẽ gây ra lỗi này. Chỉ cần di chuyển thư mục dự án theo thay đổi `D:\Project` sẽ chỉnh được lỗi bí ẩn này. 

Sử dụng các ký tự ngoài `a-z`, `A-Z`, và `0-9` như là `@`, `-`, `_`, `,`, `*`, và `#` cũng gây ra nhiều đau khổ trong quá trình truy tìm lỗi trên các nền tảng khác nhau, source control và làm hại các công cụ.

<a name="2.2"></a>
<a name="structure-top-level"><a>
### 2.2 Sử Dụng Một Tên Folder Trên Cùng 'Top Level Folder' Cho Tài Nguyên Dự Án 

Tất cả tài nguyên (asset) dự án nên được chứa trong một folder sau tên folder dự án. Lấy ví dụ, nếu như tên của của dự án là 'Generic Shooter, **mọi thành phần nội dung** của dự án phải được đặt trong `Content/GenericShooter`.

Nội dung thư mục `Developers` không phải dành cho tài nguyên (asset) mà dự án của bạn dựa theo đó, nên nó không phải là một dự án cụ thể. Xem thêm [Developer Folders](#2.3)

> The `Developers` folder is not for assets that your project relies on and therefore is not project specific. Chi tiết xem thêm [Developer Folders / Thư Mục Dev](#2.3).

Có rất nhiều lý do để phải tiếp cận phương án này.

<a name="2.2.1"></a>
#### 2.2.1 Không Nên Có Kiểu Tài Nguyên Dạng Global Assets

Thông thường the qui cách (style guide) code được viết, bạn thường được biết rằng không nên để namspace dạng global và điều này cũng ứng dụng tương tự cho folder. Khi tài nguyên (asset) nằm bên ngoài folder dự án sẽ gây rất nhiều khó khăn trong việc theo một cấu trúc folder cũng như đau khổ trong quản lý tài nguyên.

Mỗi tài nguyên (asset) nên có mục đích dùng, nếu không thì nó không thuộc về dự án. Nếu như một tài nguyên chỉ dùng để thử nghiệm thì nó không nên nằm trong thư mục dự án mà nên để trong thư mục dev [`Developer`](#2.3).

<a name="2.2.2"></a>
#### 2.2.2 Giảm Thiểu Lỗi Phát Sinh Khi Migration 

Khi làm việc trên nhiều dự án, rất thông thường sẽ thấy team sao chép tài nguyên (asset) của dự án này sang dự án khác nếu như nó có lợi cho cả hai. Khi cần thực hiện việc này, cách tốt nhất là dùng chức năng Migrate có sẵn trong Content Browser, nó không chỉ sao chép mỗi tài nguyên (asset) mà sẽ sao chép cả những tài nguyên (asset) tham chiếu phụ thuộc.  

Các mẫu tài nguyên tham chiếu phụ thuộc (dependencies) là thứ dễ gây đau đầu nhất. Nếu tài nguyên của hai dự án mà đều không có thư mục **Top Level Folder** và cũng như chúng có cùng tên hay đã được thuyên chuyển (migrated) từ trước, một cú migrate mới có thể dễ dàng xóa sổ mọi thay đổi với tài nguyên (asset) hiện tại.

Đó cũng là lý do vì sao đội ngũ Marketplace của Epic cũng ép buột dùng chính sách tương tự khi đăng ký (submit) tài nguyên (asset).

Sau một lần migration, công cụ 'Replace References' giúp an toàn việc thuyên chuyển tài nguyên, sử dụng thông qua Content Browser sẽ tạm dừng và chỉ ra các tài nguyên không nằm trong một _ _top level folder_ _ của dự án. Một khi tài nguyên đã được thuyên chuyển hoàn toàn, không nên có thêm một _ _top level folder_ _ trong Content. Cách làm này đảm bảo _100%_ an toàn trong việc thuyên chuyển.

<a name="2.2.2e1"></a>
##### 2.2.2e1 Ví Dụ Về Master Material

Lấy ví dụ bạn làm một vật liệu master (để thừa kế hay instance) trong dự án để có thể tái sử dụng trong một dự án khác nên bạn sẽ thuyên chuyển qua. Nếu tài nguyên này không nằm trong *top level folder*, có thể nó sẽ được đặt tên `Content/MaterialLibrary/M_Master`. Nếu dự án đích không có vật liệu cùng tên, sẽ không có phiền toái gì xảy ra.

Khi cùng thao tác trên cả hai dự án, tiến trình lặp lại có thể thay đổi mục đích dùng vật liệu master cũng là bình thường khi phát triển dự án.

Rắc rối nảy sinh khi, lấy ví dụ, một artist của một trong hai dự án tạo ra các set lắp ghép static mesh và rồi ai đó muốn dùng các set lắp ghép đó vào dự án thứ hai. Nếu như artist đã tạo ra tài nguyên sử dụng vật liệu instance dựa trên `Content/MaterialLibrary/M_Master`, khi thực hiện thuyên chuyển (migration) có khả năng xảy ra lỗi cho việc tài nguyên đã thuyên chuyển trước đó là chính `Content/MaterialLibrary/M_Master`.

Đây là lỗi khó đoán và giải thích. Người thực hiện thao tác thuyên chuyển static meshes có thể không phải cũng là người đã thông thuộc vật liệu master của cả hai dự án, và họ cũng có thể không nhận biết thực thể instance đang dựa trên vật liệu master. Công cụ Migrate đòi hỏi toàn bộ hệ phái sinh tham chiếu phụ thuộc, nên nó sẽ ép để lấy `Content/MaterialLibrary/M_Master` khi sao chép tài nguyên này sang dự án khác và **ghi đè** lên cái có sẵn.

Ngay tại điểm này nếu vật liệu master của cả hai dự án là không tương thích, rũi ro tàn phá hệ vật liệu phái sinh thừa kế theo hoàn toàn xảy ra, chỉ bởi vì đơn giản nó không được chứa trong một *top level folder*. Bây giờ thì công việc đơn giản của migrate tài nguyên static meshes trở thành một công việc khó nhằn.  

<a name="2.2.3"></a>
#### 2.2.3 Các Mẫu, Templates, và Nội Dung Trên Marketplace Là Không Rũi Ro

Mở rộng thêm phần [2.2.2 Giảm Thiểu Lỗi Phát Sinh Khi Migration](#2.2.2), nếu như thành viên trong team quyết định thêm vào nội dung mẫu, file template, hoặc các tài nguyên họ đã mua từ marketplace, chắc chắc nó được bảo đảm sẽ không gây tranh chấp với dự án đang làm ngoại trừ khi dự án của bạn không có trong một *top level folder* với tên định danh duy nhất. 

Tuy nhiên cũng không nên hoàn toàn tin tưởng vào nội dung trên marketplace [Top-Level Folders / Thư Mục Trên Cùng](#2.2). Có rất nhiều nội dung tài nguyên được tạo mới có *top level folder* nhưng cũng đi kèm khả năng có sự hiệu chỉnh tài nguyên có sẵn khi dùng mẫu của Epic Sample Content thường được đặt trong folder `Content`.

Điều này còn tồi tệ hơn khi hai nội dung mua từ marketplace cùng sử dụng chung nội dung của Epic Sample Content. Nếu như tất cả tài nguyên của bạn được đặt để trong một folder cụ thể, bao gồm cả thư mục mẫu đã được dời vào trong thư mục của bạn, dự án của bạn không bao giờ xảy ra lỗi. 

#### 2.2.4 DLC, Sub-Projects, Và Patches Rất Dễ Để Duy Trì 

Nếu bạn tính phát hành DLC hay hàng loạt dự án phụ (sub-projects) liên kết, tài nguyên theo các dự án này nên có *top level folder* riêng biệt. Nó giúp khi bạn cook một bảng DLC tách biệt khỏi dự án chỉnh đầy thuận lợi. Dự án phụ cũng dễ thuyên chuyển hơn mà không tốn công. Nếu cần phải thay đổi vật liệu của tài nguyên hay thêm tài nguyên nào đó đè lên cái có sẵn trong một bảng vá (patch), bạn cứ bỏ vào trong một thư mục patch và làm việc thuận lợi không lo phá hỏng dự án chính.

<a name="2.3"></a>
<a name="structure-developers"></a>
### 2.3 Sử Dụng Folder Dev Cho Việc Tự Thử Nghiệm 

Trong quá trình phát triển dự án, thành viên trong team thường có một nơi như "sand box" để tự thử nghiệm mà không lo làm hỏng phần lõi dự án. Các bảng thử nghiệm này có thể dở dang, thành viên cũng vẫn có thể muốn đặt tài nguyên lên máy chủ source control của dự án. Không phải team nào cũng dùng folder Dev, team nào dùng thư mục này hay gặp trở ngại trong việc quản lý tài nguyên khi đăng ký lên source control.

Thường dễ xảy ra lỗi khi thành viên vô tình dùng các tài nguyên chưa sẵn sàng sử dụng sau đó sẽ gây ra lỗi mặc dù tài nguyên đó đã được xóa. Lấy ví dùng một tranh chấp kinh hoàng có thể xảy ra khi một artist nào đó tạo ra các tài nguyên kiểu set module và vẫn đang loay hoay chỉnh sửa kích thước để phù hợp với grid snapping. Một bạn thiết kế màn chơi thấy tài nguyên này thú vị, có thể đem dùng ngập tràn trong các màn chơi mà không biết rằng sau đó tài nguyên trên sẽ bị xóa đi. Đây là cơ hội cho drama.

Nếu các tài nguyên này được để vào thư mục Dev, các bạn thiết kế màn chơi sẽ hiểu rằng không bao giờ nên đụng vào. Content Browser có một chức năng trong View Options giúp giấu đi các thư mục Dev (mặc nhiên sẽ không hiển thị) giúp tránh tai họa xảy ra khi vô tình dùng tài nguyên đang bào chế chưa phát hành.

Một khi tài nguyên này đã sẵn sàng để dùng, chỉ cần đơn giản "move" nó sang thư mục cụ thể và chỉnh sửa các [redirectors](https://docs.unrealengine.com/en-US/Engine/Basics/Redirectors/index.html). Đây có nghĩa là đăng ký cho tài nguyên đã xong quá trình bào chế, có thể an toàn sử dụng cho sản xuất.

<a name="2.4"></a>
<a name="structure-maps"></a>
### 2.4 Tất Cả File Map [<sup>Màn Chơi</sup>](#terms-level-map) Phải Để Trong Folder Tên Maps

File màn chơi (map) rất đặc biệt và thông dụng cho mỗi dự án để nó có hệ thống đặt tên riêng, đặc biệt là khi làm việc với dạng sub-level hay streaming level. Không quan tâm cách tổ chức hay hệ thống màn chơi thế nào trên mỗi dự án, tất cả màn chơi levels phải được để trong `/Content/Project/Maps`.

Kêu ai đó mở cụ thể một màn chơi lên mà không cần chỉ chỗ nào để là cứu rỗi về thời gian và tạo động lực trong cuộc sống dòn dã hơn. Thông dụng là các thư mục con trong thư mục `Maps` như `Maps/Campaign1/` hay `Maps/Arenas` chứa các màn chơi theo mục đích, miễn chúng đảm bảo nằm trong `/Content/Project/Maps`.

Nó giúp đơn giản hóa công việc cooking cho các kỹ sư. Sẽ rất suy sụp để truy cập toàn bộ thư mục dự án để tìm file. Các màn chơi nếu cùng nằm trong một thư mục thì sẽ khó vô tình lỡ không cook sót map nào đó. Nó cũng giúp dễ dàng hơn quá trình thực hiện lighting script hay khi kiểm tra chất lượng. 

<a name="2.5"></a>
<a name="structure-core"></a>
### 2.5 Sử Dụng Tên `Core` Cho Folder Chứa Blueprints Thiết Yếu Cũng Như Assets Khác

Dùng folder `/Content/Project/Core` chứa tài nguyên cơ bản để một dự án vận hành. Lấy ví dụ: `GameMode`, `Character`, `PlayerController`, `GameState`, `PlayerState` hay các Blueprints tương tự nên để vào đây.

Nó cũng tương đồng với thông điệp "Không Đụng Vô". Các thành viên không phải kỹ sư không có lý dó để truy cập vào folder `Core`. Cũng kèm theo kỹ năng code tốt trên một style guide, các designer có thể xử lý gameplay thông qua các class con mà hàm đã được expose. Các bạn thiết kế màn chơi (world builder) nên sử dụng Blueprints sẵn có trong các thư mục thay vì cố dùng các class nền tảng.

Lấy ví dụ như trong dự án có nhiều asset cần thu thập trong màn chơi, nên có một class cơ sở Pickup trong thư mục `Core/Pickups` định ra các hành vi cơ sở cho việc thu thập. Những kiểu thu thập cụ thể như Máu hay Đạn nên để trong folder `/Content/Project/Placeables/Pickups/`. Các game designer có thể dùng hay tùy chỉnh các kiểu thu thập trong folder này nhưng không đụng vào `Core/Pickups` vì nó có thể gây lỗi phát sinh dẫn đến không thực hiện được hành vi thu thập.

<a name="2.6"></a>
<a name="structure-assettypes"></a>
### 2.6 Không Nên Đặt Tên Folder Là `Assets` Hay `AssetTypes`

<a name="2.6.1"></a>
#### 2.6.1 Tạo Ra Một Folder Tên `Assets` Là Dư Thừa 

Mọi tài nguyên (asset) là assets.

<a name="2.6.2"></a>
#### 2.6.2 Tạo Ra Một Thư Mục Tên `Meshes`, `Textures`, Hay `Materials` Đều Dư Thừa. 

Mọi tên tài nguyên được đặt với kiểu tài nguyên để nhận biết. Dùng các tên này chỉ gây ra dưa thừa và dễ dàng bị thay thế hay Content Browser sẽ filter.

Muốn nhìn thấy chỉ mỗi static mesh trong `Environment/Rocks/` ? đơn giản chỉ cần bật tính năng view options trong Content Browser filter Static Mesh, tài nguyên cũng sẽ được sắp xếp theo sẵn ký tự. 

Muốn nhìn thấy cả static meshes và skeletal meshes? Chỉ cần bật tính năng filter cho cả hai, điều này cũng giúp tránh khả năng chọn `Control-Click` cùng lúc hai thư mục khi xem dạng cây Content Browser.

> Điều này cũng giải thích việc đặt nguyên tên tài nguyên không ích lợi. Dùng `S_` prefix cho static mesh tiết kiệm chỉ 2 ký tự trong khi dùng `Meshes/` prefix chiếm dụng tới 7 ký tự.

Không làm theo qui luật này cũng dễ xảy ra việc ai đó đem static mesh hay texture bỏ vào thư mục Materials.

<a name="2.7"></a>
<a name="structure-large-sets"></a>
### 2.7 Các Set Khổng Lồ Có Thư Mục Cấu Trúc Riêng 

Điều này là ngoại lệ mang tính ứng dụng cho mục [2.6](#2.6).

Có nhiều loại tài nguyên tập hợp của một số lượng khủng về các file phát sinh liên quan mà mỗi tài nguyên lại mang một mục đích duy nhất. Hai thứ thông dụng nhất là Animation và Audio. Nếu đang dùng trên 15+ mỗi loại tài nguyên này thì chúng nên ở cùng một folder.

Lấy ví dụ: animation được dùng chung trên nhiều nhân vật nên để ở `Characters/Common/Animations` và có thư mục con cho mục đích cụ thể `Locomotion` hay `Cinematic`.

> Điều này không liên quan đến dạng asset như texture hay vật liệu. Việc dùng folder `Rocks` là thông dụng khi có rất nhiều texture đi kèm nếu như có một số lượng lớn các loại rocks, tuy nhiên mỗi texture này liên đới đến một loại rock cụ thể thì nên có tên riêng biệt liên đới theo loại rock đó. Ngay cả khi texture này không thuộc vào thư viện vật liệu [Material Library / Thư Viện Vật Liệu](#2.8).

<a name="2.8"></a>
<a name="structure-material-library"></a>
### 2.8 `MaterialLibrary` / Thư Viện Vật Liệu

Nếu cách dự án bạn dùng là kiểu vật liệu master, các loại vật liệu theo lớp, hoặc bất cứ dạng tái sử dụng vật liệu hay texture mà không thuộc về một subset hay tài nguyên nào, nên để tất cả các tài nguyên vật liệu này vào `Content/Project/MaterialLibrary`.

> Đây cũng là cách dự án dễ để ép buột dùng chính sách 'use material instances only' (chỉ dùng vật liệu instance). Nếu mọi thành viên đều làm việc với vật liệu instance thì nơi duy nhất chứa vật liệu gốc (master) chính là folder này. Bạn rất dễ dàng kiểm tra vật liệu cơ sở này trên các folder khác mà không phải `MaterialLibrary`.

Thư mục `MaterialLibrary` không cần chỉ chứa mỗi vật liệu. Các kiểu texture tính năng dùng chung, hàm vật liệu và các thứ khác kiểu tương tự cũng nên chứa vào đây phục vụ chung mục đích. Lấy ví dụ, một texture noise nên được lưu vào `MaterialLibrary/Utility`.

Mọi kiểu thử nghiệm hay vật liệu đang debug lưu tại `MaterialLibrary/Debug`. Điều này giúp loại bỏ vật liệu hỏng, thử nghiệm khỏi quá trình shipping và cũng cách ly khỏi tài nguyên đi vào sản xuất hay có những tham chiếu gẫy lỗi. 

<a name="2.9"></a>
<a name="structure-no-empty-folders"></a>
### 2.9 Không Để Thư Mục Rỗng 

Đơn giản là không nên để bất cứ thư mục rỗng nào. Nó tạo rác trong Content Browser.

Nếu bạn tìm thấy trong Content Browser có một thư mục rỗng mà không xóa được, bạn nên thử: 
1. Đảm bảo rằng đang dùng Source Control.
1. Cho chạy ngay Fix Up Redirectors. 
1. Truy cập tới thư mục trên đĩa cứng và xóa tài nguyên bên trong. 
1. Đóng editor.
1. Đảm bảo là trạng thái source control đang sync (Ví dụ, nếu có dùng Perforce, nó đang chạy Reconcile Offline Work trên thư mục nội dung).
1. Mở editor. Kiểm tra là mọi thứ vẫn làm việc được. Nếu không thì quay lại xem cái gì gây ra nguyên nhân không hoạt động. 
1. Đảm bảo thư mục đã hoàn toàn bị xóa. 
1. Ghi nhận thay đổi - Submit lên source control.

**[⬆ Back to Top](#table-of-contents)**

<a name="3"></a>
<a name="bp"></a>
## 3. Blueprints 

Mục này sẽ tập trung vào các class Blueprint. Nếu có thể, hãy theo qui luật tiêu chuẩn code của [Epic's Coding Standard](https://docs.unrealengine.com/latest/INT/Programming/Development/CodingStandard).

### Các Hạng Mục

> 3.1 [Compiling / Biên Dịch](#bp-compiling)

> 3.2 [Variables / Biến](#bp-vars)

> 3.3 [Functions / Hàm](#bp-functions)

> 3.4 [Graphs](#bp-graphs)

<a name="3.1"></a>
<a name="bp-compiling"></a>
### 3.1 Compiling / Biên Dịch 

Mọi Blueprint cần được biên dịch không lỗi, không báo. Phải chỉnh ngay nếu có những mầm mống này hiện ra vì nó sẽ gây ra những sự cố trầm trọng hơn vô cùng đáng sợ.

**Không bao giờ** tải lên source control các Blueprint đang bị hỏng. Nếu như phải chứa nó trên source control hãy dùng chức năng Stash *Git* hay Shelve *Mercurial* blueprint đó.

Tìm hiểu thêm về:
- [Stash](https://git-scm.com/book/en/v1/Git-Tools-Stashing) 
- [Shelve](https://docs.microsoft.com/en-gb/azure/devops/repos/tfvc/suspend-your-work-manage-your-shelvesets?view=azure-devops)

Các Blueprint hỏng gây ra xáo trộn và thể hiện dưới nhiều dạng khác nhau, như là hỏng các tham chiếu ref, các hành vi không kiểm soát, không cook được, hoặc tự biên dịch lại không cần thiết. Một Blueprint hỏng có sức mạnh tàn phá toàn bộ game của bạn.

<a name="3.2"></a>
<a name="bp-vars"></a>
### 3.2 Variables / Biến 

Từ `variable` và `property` dùng thay cho nhau.

#### Hạng Mục

> 3.2.1 [Naming / Định Danh](#bp-vars)

> 3.2.2 [Editable / Các Biến Có Thể Hiệu Chỉnh](#bp-vars-editable)

> 3.2.3 [Categories / Phân Loại](#bp-vars-categories)

> 3.2.4 [Access / Truy Cập](#bp-vars-access)

> 3.2.5 [Advanced](#bp-vars-advanced)

> 3.2.6 [Transient](#bp-vars-transient)

> 3.2.7 [Config](#bp-vars-config)

<a name="3.2.1"></a>
<a name="bp-var-naming"></a>
#### 3.2.1 Định Danh

<a name="3.2.1.1"></a>
<a name="bp-var-naming-nouns"></a>
##### 3.2.1.1 Danh Từ 

Mọi biến không phải boolean đều phải rõ ràng, rõ nghĩa, và hiểu theo nghĩa danh từ.

<a name="3.2.1.2"></a>
<a name="bp-var-naming-case"></a>
##### 3.2.1.2 PascalCase 

Mọi biến không phải boolean đều phải ở dạng [PascalCase](#terms-cases).
Tức ghi hoa ký tự đầu tiên của mỗi từ, không khoảng trắng - dấu cách.

<a name="3.2.1.2e"></a>
###### 3.2.1.2e Các Ví Dụ:

Rõ nghĩa, không phải dạng boolean, viết hoa ký tự đầu tiên, không dùng dấu cách.

* `Score`
* `Kills`
* `TargetPlayer`
* `Range`
* `CrosshairColor`
* `AbilityID`

<a name="3.2.1.3"></a>
<a name="bp-var-bool-prefix"></a>
##### 3.2.1.3 Sử Dụng `b` Prefix Cho Kiểu Dữ Liệu Boolean

Tất cả biến Boolean phải được đặt tên theo [PascalCase](#terms-cases) với prefixed chữ `b` viết thường.

Ví Dụ: dùng `bDead` và `bEvil`, **KHÔNG PHẢI** `Dead` và `Evil`.

Editor của UE4 tự bỏ chữ `b` viết thường ra khỏi node khi hiển thị biến.

<a name="3.2.1.4"></a>
<a name="bp-var-bool-names"></a>
##### 3.2.1.4 Định Danh Boolean

<a name="3.2.1.4.1"></a>
###### 3.2.1.4.1 Thông Tin Chung Và Trạng Thái Độc Lập 

Mọi biến Boolean phải được định danh tính từ khi có thể nếu đang thể hiện thông tin chung. Đừng bỏ thêm những từ hay câu ý đồ đặt câu hỏi như `Is`. Đây là phần dành riêng cho dùng trong Hàm functions.

Ví dụ: `bDead` và `bHostile` **KHÔNG PHẢI** `bIsDead` và `bIsHostile`

Tránh dùng nghĩa động từ như `bRunning`. Động từ dẫn đến trạng thái phức tạp.

<a name="3.2.1.4.2"></a>
###### 3.2.1.4.2 Trạng Thái Phức Tạp  

Không dùng biến boolean để thể hiện dạng phức tạp hay phụ thuộc. Điều này gây khó dễ để thêm hay bớt và khó đọc. Dùng kiểu liệt kê (enumeration) thay cho việc đó.

Ví dụ: 
- Khi định nghĩa vũ khí, **KHÔNG NÊN DÙNG** `bReloading` và `bEquipping` nếu vũ khí không thể sử dụng cả hai trạng thái nạp đạn hay trang bị. Hãy đặt dạng liệt kê (enumeration) `EWeaponState` và sử dụng biến với các kiểu đặt trạng thái liệt kê `WeaponState`. Điều này giúp dễ thêm trạng thái cho vũ khí.

- **Không dùng** `bRunning` nếu cũng cần cả `bWalking` hoặc `bSprinting`. Nên đặt ra một enumeration dễ hiểu với tên các trạng thái.

<a name="3.2.1.5"></a>
<a name="bp-vars-naming-context"></a>
##### 3.2.1.5 Cân Nhắc Ngữ Cảnh 

Mọi tên biến không nên dư thừa với ngữ cảnh cũng như các biến tham chiếu luôn có ngữ cảnh phù hợp.

<a name="3.2.1.5e"></a>
###### 3.2.1.5e Ví Dụ:

Nên cân nhắc đặt tên Blueprint `BP_PlayerCharacter`.

Còn đây là **Bèo**

* `PlayerScore`
* `PlayerKills`
* `MyTargetPlayer`
* `MyCharacterName`
* `CharacterSkills`
* `ChosenCharacterSkin`

Tất cả tên biến trên rất dư thừa. Các biến tên kiểu đó ngụ ý rằng các biến đang thuộc về `BP_PlayerCharacter`. Nên đặt như sau.

**Good**

* `Score`
* `Kills`
* `TargetPlayer`
* `Name`
* `Skills`
* `Skin`

<a name="3.2.1.6"></a>
<a name="bp-vars-naming-atomic"></a>
##### 3.2.1.6 _Không Nên_ Thêm Kiểu Tên Nguyên Tử / Nguyên Tố

**Cần coi lại phần này khi tác giả dùng chữ Atomic, hiện tạm dịch là thành tố kiểu nguyên tử, nguyên tố, tức thành tố gốc tạo nên nhưng dễ gây khó hiểu cho người đọc Việt Nam**

**_ _Ví dụ không đặt tên kiểu FloatBullet, chữ Float chính là ý nói Atomic_ _**

Thành tố nguyên tử hay nguyên tố đặt tên cho biến là dạng đặt tên theo kiểu dữ liệu, như booleans, integers, floats, and enumerations.

Kiểu Strings và Vectos luôn được xem là dạng nguyên tố nếu theo kiểu làm việc với Blueprints.

> Khi vectors chứa ba giá trị floats, vectors cũng có thể thay đổi cả cụm, tương tự cho rotators.

> _Đừng_ để biến Text là kiểu nguyên tố, chúng có bí mật ẩn chứa các hàm địa phương hóa (như theo ngôn ngữ). Định dạng kiểu nguyên tố của chuỗi chính là chuỗi `String` các ký tự không phải `Text`.


Tên biến kiểu thành phần nguyên tố không nên được đặt tên cho biến.

Ví dụ: 
**Good**

* `Score`
* `Kills`
* `Description` 

**Bèo**

* `ScoreFloat`
* `FloatKills`
* `DescriptionString`

Ngoại lệ của qui luật này là khi biến giới thiệu một loạt số lượng của cái gì đó để đếm _và_ khi sử dụng tên không có kiểu dữ liệu đi kèm thật không dễ đọc.

Ví dụ: một chức năng tự tạo ra hàng rào cần liên tục tạo ra cây rào là biến đếm X. Lưu X vào `NumPosts` hay `PostsCount` thay vì `Posts` sẽ khó đọc hơn. `Posts` (có "s số nhiều" cũng dễ gây ra việc nhầm là mảng của biến `Post` "không có s, số ít".

<a name="3.2.1.7"></a>
<a name="bp-vars-naming-complex"></a>
##### 3.2.1.7 Thêm Kiểu Tên Non-Atomic Cho Biến
Non-atomic hay biến phức tạp là biến thể hiện dữ liệu như một tập các biến nguyên tố. Structs, Classes, Interfaces, và nguyên tố (primitives) ẩn giấu các hành vi như `Text` và `Name` đều hợp lệ cho luật này. 

> Mảng Array của một tập hợp các biến kiểu atomic là danh sách của các biến, mảng Array không thay đổi tính atomic của kiểu dữ liệu

Kiểu biến này nên chứa thêm kiểu dữ liệu đi kèm để giữ được ý nghĩa của ngữ cảnh.

Nếu một class chứa một instance của một biến phức tạp, lấy ví dụ như `BP_PlayerCharacter` sở hữu `BP_Hat`, nó nên được lưu như kiểu dữ liệu mà không thay đổi lên tên. 

Ví dụ: Dùng `Hat`, `Flag`, và `Ability` **Chứ Không Phải** `MyHat`, `MyFlag`, và `PlayerAbility`.

Nếu một class không có sở hữu giá trị của biến phức tạp, nên dùng danh từ đi kèm cho kiểu biến.

Ví dụ: Nếu `BP_Turret` có khả năng mục tiêu vào `BP_PlayerCharacter`, nên lưu mục tiêu của nó là `TargetPlayer` khi ngữ cảnh được làm rõ là tham chiếu tới biến dữ liệu khác mà nó không sỡ hữu. 

<a name="3.2.1.8"></a>
<a name="bp-vars-naming-arrays"></a>
##### 3.2.1.8 Arrays / Mảng 

Arrays theo tên và luật như hướng dẫn ở trên nhưng nên thêm số nhiều.

Ví dụ: Dùng thêm số nhiều `Targets`, `Hats`, và `EnemyPlayers`, **Chứ Không Phải** `TargetList`, `HatArray`, `EnemyPlayerArray`.


<a name="3.2.2"></a>
<a name="bp-vars-editable"></a>
#### 3.2.2 Các Biến Có Thể Hiệu Chỉnh 

Mọi biến đều an toàn để thay đổi giá trị hay để thay đổi hành vi của một Blueprint cần nên thêm đánh dấu kiểm `Editable`.

Ngược lại, mọi biến không an toàn để thay đổi giá trị hay không muốn expose cho designer thì _Không Nên_ đánh dấu `Editable`, trừ phi vì lý do kỹ thuật thì biến đó nên đánh dấu là `Expose On Spawn`.

Không nên quá cứng nhắc khi đánh dấu kiểm `Editable`.

<a name="3.2.2.1"></a>
<a name="bp-vars-editable-tooltips"></a>
##### 3.2.2.1 Tooltips / Chú Giải

Mọi biến đánh dấu kiểm `Editable`, bao gồm các biến đánh dấu có thể thay đổi bao gồm cả biến được đánh dấu `Expose On Spawn`, nên đợc có để chú giải `Tooltip` nhằm giải thích tác dụng giá trị tạo ảnh hưởng lên chức năng của Blueprint.

<a name="3.2.2.2"></a>
<a name="bp-vars-editable-ranges"></a>
##### 3.2.2.2 Slider And Value Ranges ![#](https://img.shields.io/badge/lint-unsupported-red.svg)

Mọi biến đánh dấu kiểm `Editable` nên làm kiểu thanh trượt và có khoảng giá trị (clamp) không nên để _tự set_ giá trị.

Ví dụ: một Blueprint tạo ra các cây hàng rao có thể tùy chỉnh biến `PostsCount` và nếu giá trị đầu vào bằng -1 là thật không phù hợp. Dùng range để đánh dấu 0 là tối thiểu.

Nếu biến có thể hiệu chỉnh được dùng ở Construction Script, nên dùng một thanh trượt phù hợp để ai đó không vô tình để vào một biến quá lớn gây crash editor.

Một giá trị có range chỉ cần nếu biên có thể đoán. Trong khi đó một thanh trượt sẽ hạn chế việc nhập giá trị quá lớn.

<a name="3.2.3"></a>
<a name="bp-vars-categories"></a>
#### 3.2.3 Categories / Phân Loại 

Nếu một clas có số lượng biến ít thì không cần phân loại. 

Nếu một class có 5++ số lượng biến, tất cả biến thay đổi nên được đưa vào phân loại category phổ biến là `Config`.

Nếu một class có số lượng biến lớn, tất cả các biến hiệu chỉnh được `Editable` nên được phân loại thành nhiều hạng mục nhỏ sử dụng `Config` là gốc. Các loại biến không hiệu chỉnh được nên đặt vào hạng mục giải thích chức năng.

> Bạn có thể phân loại hạng mục nhỏ bằng cách dùng ký tự `|`, ví dụ như `Config | Animations`

Ví dụ: Một class vũ khí có tập biến có thể được phân loại như sau: 

	|-- Config
	|	|-- Animations
	|	|-- Effects
	|	|-- Audio
	|	|-- Recoil
	|	|-- Timings
	|-- Animations
	|-- State
	|-- Visuals

<a name="3.2.4"></a>
<a name="bp-vars-access"></a>
#### 3.2.4 Variable Access Level / Cấp Truy Cập Biến 

Với C++, biến có tư duy của cấp độ truy cập. 
- **Public** có nghĩa là code truy cập được biến từ bên ngoài class. 
- **Protected** nghĩa là chỉ có Class đó và bất cứ thừa kế Child nào đều có thể truy cập biến.
- **Private** nghĩa chỉ bản thân class đó truy cập biến. 

Blueprint không có kiểu định hình tư duy **protected** hiện tại.

Xem như biến đánh dấu kiểm `Editable` là dạng biến **Public**, và kiểu biến không hiệu chỉnh được là biến **protected**.

<a name="3.2.4.1"></a>
<a name="bp-vars-access-private"></a>
##### 3.2.4.1 Biến Dạng Private 

Ngoại trừ khi biến chỉ truy cập được bên trong class nếu đã được định nghĩa và không bao giờ là class con, không nên đánh dấu biến là kiểu **private**. Cho đến khi biến có thể đánh dấu `protected`, chỉ để hẳn private khi nào biết chính xác muốn giới hạn class con dùng.

<a name="3.2.5"></a>
<a name="bp-vars-advanced"></a>
#### 3.2.5 Advanced Display / Hiển Thị Thêm 

Nếu một biến có thể được hiệu chỉnh nhưng ít khi dùng, hãy đánh dấu là `Advanced Display`. Nó giúp biến sẽ ẩn đi và chỉ hiển thị khi nào click vào phần advanced display (mũi tên).

Để tìm thấy phần tùy chọn `Advanced Display`, nó được liệt kê trong phần option của biến, click mũi tên mở rộng.

<a name="3.2.6"></a>
<a name="bp-vars-transient"></a>
#### 3.2.6 Transient Variables / Biến Tạm

Các loại biến tạm không cần giá trị được lưu hay load lên hay được khởi tạo giá trị zero hay null. Điều này phù hợp việc tạo tham chiếu tới đối tượng và actor khác mà giá trị là không biết tại thời điểm chạy chương trình. Điều này ngăn editor lưu một tham chiếu, giải phóng nhanh lưu và load của class Blueprint.

Vì vậy nên biến tạm nên luôn được khởi tạo là zero hay null. Nếu không sẽ khó mà debug.

<a name="3.2.7"></a>
<a name="bp-vars-config"></a>
#### 3.2.8 Config Variables 

Không dùng đánh dấu kiểm `Config Variable`. Điều này gây khó dễ cho designer kiểm soát chức năng Blueprint. Chỉ nên dùng khi viết code C++ cho các giá trị biến hiếm khi dùng tới. 

<a name="3.3"></a>
<a name="bp-functions"></a>
### 3.3 Functions, Events, và Event Dispatchers / Hàm Sự Kiện và Các Loại Sự Kiện Dispatcher

Phần này mô tả cách làm việc với hàm, sự kiện và các kiểu sự kiện dispatcher. Bất cứ gì ứng dụng cho hàm đều phù hợp với các loại còn lại. 

<a name="3.3.1"></a>
<a name="bp-funcs-naming"></a>
#### 3.3.1 Function Naming / Định Danh Hàm

Cách đặt tên hàm functions, events, và event dispatchers rất quan trọng. Dựa trên chỉ phần tên có thể tự hiểu được chức năng. Lấy ví dụ:

* Có phải là thuần một hàm ? 
* Có phải nó đang thông tin thay đổi của trạng thái (State) ? 
* Có phải là handler?
* Có phải là [RPC (Remote Procedure Calls)](https://docs.unrealengine.com/en-US/Gameplay/Networking/Actors/RPCs/index.html) ? 
* Chức năng ?

Các kiểu câu hỏi trên hoàn toàn hiểu được qua việc đặt tên phù hợp. 

<a name="3.3.1.1"></a>
<a name="bp-funcs-naming-verbs"></a>
#### 3.3.1.1 Mọi Hàm Đều Nên Đặt Tên Là Động Từ 

Tất cả hàm và sự kiện đều thực thi một hành vi nào đó, cho dù là lấy thông tin, tính toán dữ liệu, hay làm cho cái gì nổ. Bởi vậy mọi hàm đều bắt đầu là một động từ. Có thể để tên là một câu thể hiện làm điều gì đó nếu được và có nghĩa trong ngữ cảnh.

Với loại hàm `OnRep`, event handlers, và event dispatchers là ngoại lệ theo qui luật này.

Ví dụ Tốt: 

* `Fire` - đây là một ví dụ tốt nếu đó là nhân vật hay class vũ khí (có nghĩa là bắn, khai hỏa). Nó sẽ tồi nếu là cái thùng, cỏ hay một class nào đó tối nghĩa hơn. 
* `Jump` - sẽ phù hợp nếu là class nhân vật, nếu không thì sẽ rất tối nghĩa.
* `Explode`
* `ReceiveMessage`
* `SortPlayerArray`
* `GetArmOffset`
* `GetCoordinates`
* `UpdateTransforms`
* `EnableBigHeadMode`
* `IsEnemy` - cái này có động từ tobe "Is" ["Is" là một động từ](http://writingexplained.org/is-is-a-verb)

Ví dụ tồi:

* `Dead` - Là Chết ? Sẽ Chết ?
* `Rock`
* `ProcessData` - Tối nghĩa, không có ý nghĩa theo ngữ cảnh
* `PlayerState` - Đây là danh từ và tối nghĩa theo ngữ cảnh
* `Color` - Đây là động từ không có ngữ cảnh và tối nghĩa nếu là danh từ 

<a name="3.3.1.2"></a>
<a name="bp-funcs-naming-onrep"></a>
#### 3.3.1.2 Thuộc Tính Dấu Kiểm RepNotify Cho Phần Hàm Luôn Luôn `OnRep_Variable` 

Mọi hàm để phản ảnh kiểu lập lại (dùng theo chức năng network) nên ở dạng `OnRep_Variab`. Đây là bắt buột khi biên tập Blueprint. Nếu như đang viết C++ một dạng hàm `OnRep` cũng nên theo cách viết này khi expose cho Blueprint.

<a name="3.3.1.3"></a>
<a name="bp-funcs-naming-bool"></a>
#### 3.3.1.3 Kiểu Hàm Thông Tinh Trả Về Giá Trị Boolean Nên Là Loại Đặt Câu Hỏi 

Khi viết một hàm không thay đổi trạng thái (state) hoặc hiệu chỉnh một đối tượng hay đơn thuần chỉ lấy thông tin, trạng thái hoặc tính toán giá trị yes/no, nó nên là đặt tên kiểu một câu hỏi. Cái này cũng theo luật [đặt tên là động từ](#bp-funcs-naming-verbs)

Điều này cực kỳ quan trọng nếu một câu hỏi không được đưa ra, nó có thể cho là hàm đó đang thực thi một chức năng và giá trị trả về là kết quả thực thi thành công.

Ví dụ tốt:

* `IsDead`
* `IsOnFire`
* `IsAlive`
* `IsSpeaking`
* `IsHavingAnExistentialCrisis`
* `IsVisible`
* `HasWeapon` - ["Has" là một động từ.](http://grammar.yourdictionary.com/parts-of-speech/verbs/Helping-Verbs.html)
* `WasCharging` - ["Was" là động từ quá khứ của "be".](http://grammar.yourdictionary.com/parts-of-speech/verbs/Helping-Verbs.html) Sử dụng "was" khi tham chiếu tới 'previous frame' hoặc 'previous state'.
* `CanReload` - ["Can" là một động từ.](http://grammar.yourdictionary.com/parts-of-speech/verbs/Helping-Verbs.html)

Ví dụ bèo:

* `Fire` - Đang bắn ? Sẽ bắn ? Thực thi bắn?
* `OnFire` - Có thể bị hiểu nhầm với sự kiện event dispatcher cho việc bắn.
* `Dead` - Chết chưa ? sẽ chết ? 
* `Visibility` - Có hiển thị không ? để hiển thị ? một kiểu tên đặt ra với điều kiện khá bay bổng.

