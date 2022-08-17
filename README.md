# PHP-Basic

## Introduction to web Technology(Giới thiệu về công nghệ web):

- Công nghệ Web đề cập đến các công cụ và kỹ thuật khác nhau được sử dụng trong quá trình giao tiếp giữa các loại thiết
  bị khác nhau qua internet. Trình duyệt web được sử dụng để truy cập các trang web. Trình duyệt web có thể được định
  nghĩa là các chương trình hiển thị văn bản, dữ liệu, hình ảnh, hoạt ảnh và video trên Internet. Các tài nguyên siêu
  liên kết trên World Wide Web có thể được truy cập bằng giao diện phần mềm do trình duyệt Web cung cấp.

### Công nghệ Web có thể được phân loại thành các phần sau:

- **World Wide Web (WWW):** World Wide Web dựa trên một số công nghệ khác nhau: Trình duyệt web, Ngôn ngữ đánh dấu siêu
  văn bản (HTML) và Giao thức truyền siêu văn bản (HTTP).
- **Web Browser(Trình duyệt web):** Trình duyệt web là một phần mềm ứng dụng để khám phá www (World Wide Web). Nó cung
  cấp giao diện giữa máy chủ và máy khách và yêu cầu máy chủ cung cấp các tài liệu và dịch vụ web.
- **Web Server(Máy chủ Web):** Máy chủ web là một chương trình xử lý các yêu cầu mạng của người dùng và phục vụ họ với
  các tệp tạo trang web. Việc trao đổi này diễn ra bằng cách sử dụng Giao thức truyền siêu văn bản (HTTP).
- **Web Pages(Trang Web):** Trang web là một tài liệu kỹ thuật số được liên kết với World Wide Web và bất kỳ ai được kết
  nối với internet có trình duyệt web đều có thể xem được.
- **Web Development(Phát triển Web):** Phát triển web đề cập đến việc xây dựng, tạo và duy trì các trang web. Nó bao gồm
  các khía cạnh như thiết kế web, xuất bản web, lập trình web và quản lý cơ sở dữ liệu. Đó là việc tạo ra một ứng dụng
  hoạt động trên internet, tức là các trang web.

## Introduction to HTML5 and CSS(Giới thiệu về HTML5 và CSS):

### HTML5

- **HTML** là viết tắt của Hyper Text Markup Language. Nó được sử dụng để thiết kế các trang web bằng ngôn ngữ đánh dấu.
  HTML là viết tắt của ngôn ngữ Siêu văn bản và Đánh dấu. Siêu văn bản xác định liên kết giữa các trang web. Ngôn ngữ
  đánh dấu được sử dụng để xác định tài liệu văn bản trong thẻ xác định cấu trúc của các trang web. HTML 5 là phiên bản
  thứ năm và hiện tại của HTML. Nó đã cải thiện đánh dấu có sẵn cho các tài liệu và đã giới thiệu các giao diện lập
  trình ứng dụng:application programming interfaces(API) và Mô hình Đối tượng Tài liệu:Document Object Model(DOM).

### CSS

- **C**ascading **S**tyle **S**heets, hay còn được gọi là **CSS**, CSS cho phép áp dụng cả kiểu(Style) cho các trang web
  ,bạn có thể làm cho trang web theo cách mình muốn như thay đổi màu phông chữ , khoảng cách và nhiều thứ khác.

## PHP Introduction

- Thuật ngữ PHP được viết tắt từ _Hypertext Preprocessor_ .PHP là một ngôn ngữ kịch bản(scripting languege) phía máy chủ
  đc thiết kế đặc biệt để phát triển web. PHP là một mã nguồn mở, được tải xuống và sử dingj miễn phí.

## PHP Syntax

- Một tập lệnh được thực thi trên máy chủ và dả về kết quả của HTML được ghi trở laiij trình duyệt, nó thường có các thẻ
  HTML và PHP.

## PHP Data Types

**Các biến có thể lưu trữ dữ liệu thuộc các kiểu khác nhau và các kiểu dữ liệu khác nhau có thể làm những việc khác
nhau:**

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

```php
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

- Các biến(Variables) trong chương trình được sử dụng để lưu trữ một số giá hoặc dữ liệu nào đó.Các biến có thể lưu
  chuỗi,giá trị kí tự,địa chỉ bộ nhớ và giá trị số.
- Mọi biến được khai báo trong PHP phải bắt đầu bằng dấu đô la ($), theo sau là tên biến.

### Constants

- Hằng số(Constands) là số nhận dạng hoặc tên đơn giản có thể được gán bất kỳ giá trị cố định nào .Tương tự như một biến
  ngoại trừ việc chúng không bao giờ có thể thay đổi được kể cả trong quá trình thực thi.

### Array

- Mảng(Array) trong PHP là một kiểu cấu trúc dữ liệu cho phép ta lưu trữ nhiều phần tử của kiểu dữ liệu tương tự dưới
  một biến duy nhất.Một mảng được tạo bằng cách sử dụng một hàm `array()` trong PHP hoặc có thể dùng bằng cách khai báo
  biến `$a = ["a","b","c"]`.

## PHP Operators

- Các toán tử(Operators) được sử dụng để thực hiện các phép toán đơn giản như cộng ,trừ ,nhân ,...

### Kí hiệu

| Operator | Name        | Syntax      | Operation                           |
|:---------|:------------|:------------|:------------------------------------|
| +        | Cộng        | $x + $y     | Tính tổng phép tính                 |
| -        | Trừ         | $x - $y     | Trừ phép tính                       |
| *        | Nhân        | $x * $y     | Nhân phép tính                      |
| /        | Chia        | $x / $y     | Chia phép tính                      |
|**        | Lũy thừa    | $x ** $y    | $x được nâng lên thành lũy thừa $y  |
|**        | Mô đun      | $x % $y     | Phần còn lại của $x chia cho $y     |

## Control Structures

### if else statement

- Câu lệnh if / else thực thi một khối mã nếu một điều kiện được chỉ định là đúng. Nếu điều kiện sai, một khối mã khác
  có thể được thực thi.

````php
<?php
    $t = date("H");

    if ($t < "20") {
        echo "Have a good day!";
    } else {
        echo "Have a good night!";
    }
?>
````

### else if statement

- Câu lệnh if ... elseif ... else thực thi các mã khác nhau cho nhiều hơn hai điều kiện.

````php
<?php
$t = date("H");

if ($t < "10") {
    echo "Have a good morning!";
} elseif ($t < "20") {
    echo "Have a good day!";
} else {
      echo "Have a good night!";
  }
?>
````

### switch case

- Câu lệnh switch tương tự như một loạt câu lệnh if trên cùng 1 biểu thức,được sử dụng để thực hiện các hành động khác
  nhau dựa trên các điều kiện khác nhau.

````php
<?php
    $favcolor = "red";

    switch ($favcolor) {
        case "red":
            echo "Your favorite color is red!";
            break;
        case "blue":
            echo "Your favorite color is blue!";
            break;
        case "green":
            echo "Your favorite color is green!";
            break;
        default:
            echo "Your favorite color is neither red, blue, nor green!";
    }
?>
````

### Loops

- Thường thì khi bạn viết mã, bạn muốn cùng một khối mã chạy đi chạy lại một số lần nhất định. Vì vậy, thay vì thêm một
  số dòng mã gần như bằng nhau trong một tập lệnh, chúng ta có thể sử dụng các vòng lặp.

#### Trong PHP, chúng ta có các loại vòng lặp sau:

- **while**
- **do...while**
- **for**
- **foreach**

### while

- Lặp qua một khối mã miễn là điều kiện được chỉ định là đúng.

```php
<?php
$x = 1;

while($x <= 5) {
  echo "The number is: $x <br>";
  $x++;
}
?>
```

### do while

- Lặp qua một khối mã một lần và sau đó lặp lại vòng lặp miễn là điều kiện chỉ định đúng.

```php
<?php
$x = 1;

do {
  echo "The number is: $x <br>";
  $x++;
} while ($x <= 5);
?>
```

### for

- Lặp qua một khối mã một số lần được chỉ định.

```php
<?php
for ($x = 0; $x <= 10; $x++) {
  echo "The number is: $x <br>";
}
?>
```

### foreach

- Lặp qua một khối mã cho mỗi phần tử trong một mảng.

```php
<?php
$colors = array("red", "green", "blue", "yellow");

foreach ($colors as $value) {
  echo "$value <br>";
}
?>
```

## String Functions

-Các hàm chuỗi PHP là một phần của lõi PHP. Không cần cài đặt để sử dụng các chức năng này.

1. Hàm `chunk_split()` : Tách một chuỗi thành một loạt các phần nhỏ hơn.

<details><summary><b>Demo</b></summary>
<p>

```php 
<?php
  $str = "Hello world!";
  echo chunk_split($str,1,".");
?>
```

Return : H.e.l.l.o. .w.o.r.l.d.!.

</p>
</details>

2. Hàm `implode()` : Trả về một chuỗi từ các phần tử của một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
$arr = array('Hello','World!','Beautiful','Day!');
echo implode(" ",$arr);
?>
```

Return: Hello World! Beautiful Day!

</p>
</details>

3. Hàm `explode()` : Ngắt một chuỗi thành một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
$str = "Hello world. It's a beautiful day.";
print_r (explode(" ",$str));
?> 
```

Return: Array ( [0] => Hello [1] => world. [2] => It's [3] => a [4] => beautiful [5] => day. )

</p>
</details>

4. Hàm `echo()` : Đầu ra một hoặc nhiều chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo "Hello!"
?> 
```

Return: Hello!

</p>
</details>

5. Hàm `join()` : Giống mới hàm `implode()`

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
$arr = array('Hello','World!','Beautiful','Day!');
echo join(" ",$arr);
?> 
```

Return: Hello World! Beautiful Day!

</p>
</details>

6. Hàm `md5()` : Hàm mã hóa MD5.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
$str = "Hello";
echo md5($str);
?> 
```

Return: 8b1a9953c4611296a827abf8c47804d7

</p>
</details>

7. Hàm `str_ireplace()` : Thay thế một số ký tự bằng một số ký tự khác trong một chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo str_ireplace("WORLD","Peter","Hello good world!");

?> 
```

Return: Hello good Peter!

</p>
</details>

8. Hàm `str_repeat()` : Lặp lại một chuỗi một số lần được chỉ định.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo str_repeat("Wow",13);
?> 
```

Return: WowWowWowWowWowWowWowWowWowWowWowWowWow

</p>
</details>

9. Hàm `str_replace()` : Thay thế một số ký tự bằng một số ký tự khác trong một chuỗi gần giống hàm `str_ireplace()`.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo str_replace("world","Peter","Hello world!");
?> 
```

Return: Hello Peter!

</p>
</details>

10. Hàm `str_shuffle()` : Trộn ngẫu nhiên tất cả các ký tự của một chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo str_shuffle("Hello World");
?> 
```

Return: oldlre loWH

</p>
</details>

11. Hàm `str_split()` : Chia một chuỗi thành một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
print_r(str_split("Hello"));
?> 
```

Return: Array ( [0] => H [1] => e [2] => l [3] => l [4] => o )

</p>
</details>

12. Hàm `str_word_count()` : Đếm số từ trong một chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo str_word_count("Hello world!");
?> 
```

Return: 2

</p>
</details>

13. Hàm `stripos()` : Tìm vị trí xuất hiện đầu tiên của  một chuỗi bên trong chuỗi khác.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo stripos("I love php, I love php too!","PHP");
?> 
```

Return: 7

</p>
</details>

14. Hàm `strlen()` : Tìm vị trí xuất hiện đầu tiên của  một chuỗi bên trong chuỗi khác.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo strlen("Hello");
?> 
```

Return: 5

</p>
</details>

15. Hàm `substr()` : Trả về một phần của chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php 
<?php
echo substr("Hello world",6);
?> 
```

Return: world

</p>
</details>

## Array Functions

## File handling