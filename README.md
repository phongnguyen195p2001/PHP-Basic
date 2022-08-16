# PHP-Basic
## Introduction to web Technology(Giới thiệu về công nghệ web):
- Công nghệ Web đề cập đến các công cụ và kỹ thuật khác nhau được sử dụng trong quá trình giao tiếp giữa các loại thiết bị khác nhau qua internet. Trình duyệt web được sử dụng để truy cập các trang web. Trình duyệt web có thể được định nghĩa là các chương trình hiển thị văn bản, dữ liệu, hình ảnh, hoạt ảnh và video trên Internet. Các tài nguyên siêu liên kết trên World Wide Web có thể được truy cập bằng giao diện phần mềm do trình duyệt Web cung cấp.
### Công nghệ Web có thể được phân loại thành các phần sau:
- **World Wide Web (WWW):** World Wide Web dựa trên một số công nghệ khác nhau: Trình duyệt web, Ngôn ngữ đánh dấu siêu văn bản (HTML) và Giao thức truyền siêu văn bản (HTTP).
- **Web Browser(Trình duyệt web):** Trình duyệt web là một phần mềm ứng dụng để khám phá www (World Wide Web). Nó cung cấp giao diện giữa máy chủ và máy khách và yêu cầu máy chủ cung cấp các tài liệu và dịch vụ web.
- **Web Server(Máy chủ Web):** Máy chủ web là một chương trình xử lý các yêu cầu mạng của người dùng và phục vụ họ với các tệp tạo trang web. Việc trao đổi này diễn ra bằng cách sử dụng Giao thức truyền siêu văn bản (HTTP).
- **Web Pages(Trang Web):** Trang web là một tài liệu kỹ thuật số được liên kết với World Wide Web và bất kỳ ai được kết nối với internet có trình duyệt web đều có thể xem được.
- **Web Development(Phát triển Web):** Phát triển web đề cập đến việc xây dựng, tạo và duy trì các trang web. Nó bao gồm các khía cạnh như thiết kế web, xuất bản web, lập trình web và quản lý cơ sở dữ liệu. Đó là việc tạo ra một ứng dụng hoạt động trên internet, tức là các trang web.
## Introduction to HTML5 and CSS(Giới thiệu về HTML5 và CSS):
### HTML5
- **HTML** là viết tắt của Hyper Text Markup Language. Nó được sử dụng để thiết kế các trang web bằng ngôn ngữ đánh dấu. HTML là viết tắt của ngôn ngữ Siêu văn bản và Đánh dấu. Siêu văn bản xác định liên kết giữa các trang web. Ngôn ngữ đánh dấu được sử dụng để xác định tài liệu văn bản trong thẻ xác định cấu trúc của các trang web. HTML 5 là phiên bản thứ năm và hiện tại của HTML. Nó đã cải thiện đánh dấu có sẵn cho các tài liệu và đã giới thiệu các giao diện lập trình ứng dụng:application programming interfaces(API) và Mô hình Đối tượng Tài liệu:Document Object Model(DOM).
### CSS
- **C**ascading **S**tyle **S**heets, hay còn được gọi là **CSS**, CSS cho phép áp dụng cả kiểu(Style) cho các trang web ,bạn có thể làm cho trang web theo cách mình muốn như thay đổi màu phông chữ , khoảng cách và nhiều thứ khác.
## PHP Introduction
- Thuật ngữ PHP được viết tắt từ _Hypertext Preprocessor_ .PHP là một ngôn ngữ kịch bản(scripting languege) phía máy chủ đc thiết kế đặc biệt để phát triển web. PHP là một mã nguồn mở, được tải xuống và sử dingj miễn phí.
## PHP Syntax
- Một tập lệnh được thực thi trên máy chủ và dả về kết quả của HTML được ghi trở laiij trình duyệt, nó thường có các thẻ HTML và PHP.
## PHP Data Types
**Các biến có thể lưu trữ dữ liệu thuộc các kiểu khác nhau và các kiểu dữ liệu khác nhau có thể làm những việc khác nhau:**
- **String** : Trả về chuỗi.
`
    $a = "chuỗi";
`
- **Integer(int)** : Trả về số nguyên.
`
    $a = 1;
`
- **Float** : Trả về dạng số thập phân.
`
    $a = 2.5;
`
- **Boolen** : Trả về đúng hoặc sai.
`
  $x = true;
  $y = false;
`
- **Array** : Trả về mảng.
`
  $cars = array("Volvo","BMW","Toyota");
`
- **Object** : Trả về 1 đối tượng.
```
<?php
    class Car {
        public $color;
        public $model;
        public function __construct($color, $model) {
            $this->color = $color;
            $this->model = $model;
        }
        public function message() {
            return "My car is a " . $this->color . " " . $this->model . "!";
        }
    }

    $myCar = new Car("black", "Volvo");
    echo $myCar -> message();
    echo "<br>";
    $myCar = new Car("red", "Toyota");
    echo $myCar -> message();
?>
```
- **Null** : Trả về null(Không có giá trị nào đc gán cho nó).
`
  $x = "Hello world!";
  $x = null;
`
- **Resource** : Nó là việc lưu trữ một tham chiếu đến các hàm và tài nguyên bên ngoài PHP.
## PHP Variables, Constants and Array  
### Variables
- Các biến(Variables) trong chương trình được sử dụng để lưu trữ một số giá hoặc dữ liệu nào đó.Các biến có thể lưu chuỗi,giá trị kí tự,địa chỉ bộ nhớ và giá trị số.
- Mọi biến được khai báo trong PHP phải bắt đầu bằng dấu đô la ($), theo sau là tên biến.
### Constants
- Hằng số(Constands) là số nhận dạng hoặc tên đơn giản có thể được gán bất kỳ giá trị cố định nào .Tương tự như một biến ngoại trừ việc chúng không bao giờ có thể thay đổi được kể cả trong quá trình thực thi.
### Array
- Mảng(Array) trong PHP là một kiểu cấu trúc dữ liệu cho phép ta lưu trữ nhiều phần tử của kiểu dữ liệu tương tự dưới một biến duy nhất.Một mảng được tạo bằng cách sử dụng một hàm `array()` trong PHP hoặc có thể dùng bằng cách khai báo biến `$a = ["a","b","c"]`.
## PHP Operators
