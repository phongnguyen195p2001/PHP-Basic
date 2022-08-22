# PHP-Basic

## Introduction to web Technology(Giới thiệu về công nghệ web):

- Công nghệ web là một thuật ngữ chung đề cập đến nhiều ngôn ngữ và gói đa phương tiện được sử dụng kết hợp với nhau, để
  tạo ra các trang web. Mỗi công nghệ có chức năng riêng biệt và cần yêu cầu sử dụng kép ít nhất thêm một công nghệ
  khác.

### Công nghệ Web có thể được phân loại thành các phần sau:

#### Server Side Rendering (SSR):

- Gọi nó là server-side rendering là vì phần lớn logic sẽ được xử lý ở server:

    - Khi người dùng vào một trang web, trình duyệt sẽ gửi GET request tới web server.
    - Web server sẽ nhận request, đọc dữ liệu từ database.
    - Web server sẽ render HTML, trả về cho browser để hiển thị cho người dùng

#### Client Side Rendering (CSR):

- Client Side Rendering tức là việc render HTML, CSS sẽ được thực hiện ở client (Tức JavaScript ở trình duyệt)

- Cách tiếp cận này được tiếp sức mạnh từ các framework Javascript và các thư viện. Luồng chính của một trang web render
  trong trường hợp Client-side rendering như sau:

    - Người dùng gửi request tới webiste
    - Thay vì một server, một con CDN có thể được sử dụng để gửi HTML, CSS và các file hỗ trợ cho người dùng.
    - Trình duyệt tải HTML và JS trong khi nhìn thấy một biểu tượng loading
    - Sau khi trình duyệt lấy JS về, nó sẽ tạo các yêu cầu API thông qua Ajax và lấy về các nội dung động và xử lí chúng
      để render ra nội dung cuối cùng.
    - Sau khi server phản hồi, nội dung cuối cùng sẽ được render sử dụng quá trình xử lí DOM trên trình duyệt người
      dùng.

##### Front End:

- Front-end được tạo ra bởi 3 loại ngôn ngữ cơ bản là HTML, CSS và JavaScript. Các lập trình viên Front-end sẽ cần đảm
  bảo nội dung hiển thị tốt trên mọi nền tảng khác nhau.

###### Các công nghệ Front End frameworks:

![alt text](https://lh5.googleusercontent.com/Hfnut8UXHDCnft_l065ubj0XCOolACcvSLWGg2eiJWQHnO8o-L5KCOT4w_ZAP4FoNbk4YSCKPOfREwIpbu0lTZIk8QFCRT30NKtgTDCCAxHcA3QAAMTYbSrgk2tsSvUMzP-eKvCG)

##### Back End:

- BackEnd là những phần bên trong bao gồm: máy chủ, ứng dụng và cơ sở dữ liệu.

###### Các công nghệ Back End frameworks:

![alt text](https://d3hi6wehcrq5by.cloudfront.net/itnavi-blog/2020/04/Backend-l%C3%A0-g%C3%AC-3.jpg)

### Khác nhau giữa SSR và CSR:

- **SSR**: Người dũng sẽ gửi request đến thẳng sever rồi phía sever reder ra html giả về phía người dùng.
- **CSR**: Người dùng sẽ gửi request đến sever rồi phía sever giả về một cục JS và reder ra html giả về phía người dùng.

## Introduction to HTML5 and CSS(Giới thiệu về HTML5 và CSS):

### HTML5

- **HTML(Hypertext Markup Language)** là một nền tảng tương tự như Microsoft Word giúp người dùng thiết kế thành phần
  trong website, cấu trúc các trang, chuyên mục hoặc các thiết kế các ứng dụng… Vậy, chức năng chủ yểu của nền tảng này
  chính là tạo bố cục và định dạng website.

- **HTML5** là một ngôn ngữ lập trình được phát triển trên nền tảng ngôn ngữ HTML và quan trọng nhất của World Wide
  Web (WWW). Nó được sử dụng để thiết kế và cấu trúc các website, hỗ trợ cho đa phương tiện tối đa nhưng vẫn giúp cho
  website thân thiện với mọi người dùng và mọi thiết bị, các chương trình máy tính, trình duyệt web.

#### Sự khác biết giữa HTML và HTML5

- **HTML5 hỗ trợ nhiều ứng dụng hơn**:Một số ứng dụng như SVG,canvas... được HTML5 hỗ chợ , nhưng dùng HTML thì phải
  dùng các phương tiện bổ trợ.
- _Lưu dữ liệu tạm_ **HTML5** sử dụng web **SQL databases, application cache** còn HTML chỉ dùng cache của trình duyệt.
- _JavaScript chạy trong web browser_ .**HTML5** hỗ trợ hoàn toàn JavaScript chạy trên web browser còn Html ở phiên bản
  cũ hơn thì không thực hiện được.
- _Các element:_ **HTML5** tích hợp các element mới mẻ và quan trọng như summary, time, aside, audio, command, data,
  datalist, details, embed, wbr, figcaption, figure, footer, header, article, hgroup, bdi, canvas, keygen, mark, meter,
  nav, output, progress, rp, rt, ruby, section, source, track, video… Bên cạnh đó, nó cũng được loại bỏ các elements lỗi
  thời trong HTML như isindex, noframes, acronym, applet, basefont, dir, font, frame, frameset, big, center, strike….

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
<h1>Hello!</h1>
</body>
</html>
```

### CSS

- **C**ascading **S**tyle **S**heets, hay còn được gọi là **CSS**, CSS cho phép áp dụng cả kiểu(Style) cho các trang web
  ,bạn có thể làm cho trang web theo cách mình muốn như thay đổi màu phông chữ , khoảng cách và nhiều thứ khác.

#### Các cách viết css

- Độ ưu tiên theo số thứ thự 1,2,3:

1. Viết trong thẻ của html (attribute):

```html
<p style="color: black;font-style: normal"></p>
```

2. Viết css trong file html:

```html

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style>
        h1 {
            color: black;
            font-style: normal;
        }
    </style>
</head>
<body>
<h1>Hello!</h1>
</body>
</html>
```

3. viết trong file css:

```css
h1 {
    color: black;
    font-size: 20px;
}
```

## PHP Introduction
/var/www/prj1
- Thuật ngữ PHP được viết tắt từ _Hypertext Preprocessor_ .PHP là một ngôn ngữ kịch bản(scripting languege) phía máy chủ
  đc thiết kế đặc biệt để phát triển web. PHP là một mã nguồn mở, được tải xuống và sử dingj miễn phí.

## PHP Syntax

- Một tập lệnh được thực thi trên máy chủ và dả về kết quả của HTML được ghi trở laiij trình duyệt, nó thường có các thẻ
  HTML và PHP.

## PHP Data Types

**Các biến có thể lưu trữ dữ liệu thuộc các kiểu khác nhau và các kiểu dữ liệu khác nhau có thể làm những việc khác
nhau:**

- **String** : Kiểu chuỗi.
  `
  $a = "chuỗi";
  `
- **Integer(int)** : Kiểu số nguyên.
  `
  $a = 1;
  `
- **Float** : Kiểu số thập phân.
  `
  $a = 2.5;
  `
- **Boolen** : Trả về đúng hoặc sai.
  `
  $x = true;
  $y = false;
  `
- **Array** : Kiểu mảng.
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

| Operator | Name                | Syntax   | Operation                          |
|:---------|:--------------------|:---------|:-----------------------------------|
| +        | Cộng                | $x + $y  | Tính tổng phép tính                |
| -        | Trừ                 | $x - $y  | Trừ phép tính                      |
| *        | Nhân                | $x * $y  | Nhân phép tính                     |
| /        | Chia                | $x / $y  | Chia phép tính                     |
| **       | Lũy thừa            | $x ** $y | $x được nâng lên thành lũy thừa $y |
| %        | Mô đun              | $x % $y  | Phần còn lại của $x chia cho $y    |
| ">"      | Lớn hơn             | $x > $y  | $x phải lớn hơn $y                 |
| <        | Nhỏ hơn             | $x < $y  | $x phải lớn hơn $y                 |
| ==       | Bằng                | $x == $y | $x bằng $y                         |
| <=       | Nhỏ hơn hoặc bằng   | $x <= $y | $x nhỏ hơn hoặc bằng $y            |
| `>=      | Lớn hơn hoặc bằng   | $x >= $y | $x lớn hơn hoặc bằng               |

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

6. Hàm `trim()` : Loại bỏ các ký tự từ cả hai bên của một chuỗi.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$str = "Hello World!";
echo $str . "<br>";
echo trim($str,"Hed!");
?>
```

Return: llo Worl

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

13. Hàm `stripos()` : Tìm vị trí xuất hiện đầu tiên của một chuỗi bên trong chuỗi khác.

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

14. Hàm `strlen()` : Tìm vị trí xuất hiện đầu tiên của một chuỗi bên trong chuỗi khác.

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

- Các hàm mảng cho phép bạn truy cập và thao tác với mảng:

1. Hàm `array()` : Hàm được sử dụng để tạo một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$cars=array("Volvo","BMW","Toyota"); 
echo "I like " . $cars[0] . ", " . $cars[1] . " and " . $cars[2] . ".";
?> 
```

Return: I like Volvo, BMW and Toyota.

</p>
</details>

2. Hàm `array_pop()` : Xóa phần tử cuối của mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a=array("red","green","blue");
array_pop($a);
print_r($a);
?> 
```

Return: Array ( [0] => red [1] => green )

</p>
</details>

3. Hàm `array_push()` : Chèn một hoặc nhiều phần tử vào cuối mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a=array("red","green");
array_push($a,"blue","yellow");
print_r($a);
?> 
```

Return: Array ( [0] => red [1] => green [2] => blue [3] => yellow )

</p>
</details>

4. Hàm `array_replace()` : Hàm thay thế các giá trị của mảng đầu tiên bằng các giá trị từ các mảng sau.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a1=array("red","green");
$a2=array("blue","yellow");
print_r(array_replace($a1,$a2));
?> 
```

Return: Array ( [0] => blue [1] => yellow )

</p>
</details>

5. Hàm `array_shift()` : Hàm loại bỏ phần tử đầu tiên khỏi một mảng và trả về giá trị của phần tử bị loại bỏ.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a=array("a"=>"red","b"=>"green","c"=>"blue");
echo array_shift($a);
print_r ($a);
?> 
```

Return: Array ( [b] => green [c] => blue )

</p>
</details>

6. Hàm `array_slice()` : Hàm trả về các phần đã chọn của một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a=array("red","green","blue","yellow","brown");
print_r(array_slice($a,2));
?> 
```

Return: Array ( [0] => blue [1] => yellow [2] => brown )
</p>
</details>

7. Hàm `array_unshift()` : Hàm chèn các phần tử mới vào một mảng. Các giá trị mảng mới sẽ được chèn vào đầu mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$a=array("a"=>"red","b"=>"green");
array_unshift($a,"blue");
print_r($a);
?> 
```

Return: Array ( [0] => blue [a] => red [b] => green )
</p>
</details>

8. Hàm `sort()` : Hàm chèn các phần tử mới vào một mảng. Các giá trị mảng mới sẽ được chèn vào đầu mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$cars=array("Volvo","BMW","Toyota");
sort($cars);
?> 
```

Return: Array ( [0] => BMW [1] => Toyota [2] => Volvo )
</p>
</details>

## File handling

- Các chức năng của hệ thống tệp cho phép bạn truy cập và thao tác với hệ thống tệp.

### Các hàm:

1. Hàm `fopen();` : Dùng để mở một tết hoặc URL.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$file = fopen("test.txt","r");
?> 
```

</p>
</details>

2. Hàm `fclose();` : Dùng để đóng tệp.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$file = fopen("test.txt", "r");
fclose($file);
?> 
```

</p>
</details>

3. Hàm `file();` : Đọc một tệp thành một mảng.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
print_r(file("test.txt"));
?> 
```

return : Array ( [0] => Hello, this is a test file. [1] => There are three lines here. [2] => This is the last line. )

</p>
</details>

4. Hàm `fgets();` : Trả về một dòng từ một tệp đang mở.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
$file = fopen("test.txt","r");
echo fgets($file);
fclose($file);
?> 
```

return : Hello, this is a test file.

</p>
</details>

5. Hàm `copy();` : Hàm sao chép một tệp.

<details><summary><b>Demo</b></summary>
   <p>

```php
<?php
echo copy("source.txt","target.txt");
?> 
```

</p>
</details>

### Các chế độ mở tệp:

- “r” - Tệp tìm kiếm. Nếu tệp được mở thành công, fopen () sẽ tải tệp đó vào bộ nhớ và thiết lập một con trỏ trỏ đến ký
  tự đầu tiên trong đó. Nếu không mở được tệp, fopen () trả về giá trị NULL.
  <br><br>
- “rb” - Mở để đọc ở chế độ nhị phân. Nếu tệp không tồn tại, fopen () trả về NULL.
  <br><br>
- “w” - Tệp tìm kiếm. Nếu tệp tồn tại, nội dung của nó sẽ bị ghi đè. Nếu tệp không tồn tại, một tệp mới sẽ được tạo. Trả
  về NULL, nếu không thể mở tệp.
  <br><br>
- “wb” - Mở để viết ở chế độ nhị phân. Nếu tệp tồn tại, nội dung của nó sẽ bị ghi đè. Nếu tệp không tồn tại, nó sẽ được
  tạo.
  <br><br>
- “a” - Tệp tìm kiếm. Nếu tệp được mở thành công, fopen () sẽ tải tệp đó vào bộ nhớ và thiết lập một con trỏ trỏ đến ký
  tự cuối cùng trong đó. Nếu tệp không tồn tại, một tệp mới sẽ được tạo. Trả về NULL, nếu không thể mở tệp.
  <br><br>
- “ab” - Mở để nối thêm ở chế độ nhị phân. Dữ liệu được thêm vào cuối tệp. Nếu tệp không tồn tại, nó sẽ được tạo.
  <br><br>
- “r+” - Tệp tìm kiếm. Nếu được mở thành công, fopen () sẽ tải nó vào bộ nhớ và thiết lập một con trỏ trỏ đến ký tự đầu
  tiên trong đó. Trả về NULL, nếu không thể mở tệp.
  <br><br>
- “rb+” - Mở cho cả đọc và ghi ở chế độ nhị phân. Nếu tệp không tồn tại, fopen () trả về NULL.
  <br><br>
- “w+” - Tệp tìm kiếm. Nếu tệp tồn tại, nội dung của nó sẽ bị ghi đè. Nếu tệp không tồn tại, một tệp mới sẽ được tạo.
  Trả về NULL, nếu không thể mở tệp.
  <br><br>
- “wb+” - Mở cho cả đọc và ghi ở chế độ nhị phân. Nếu tệp tồn tại, nội dung của nó sẽ bị ghi đè. Nếu tệp không tồn tại,
  nó sẽ được tạo.
  <br><br>
- “a+” - Tệp tìm kiếm. Nếu tệp được mở thành công, fopen () sẽ tải tệp vào bộ nhớ và thiết lập một con trỏ trỏ đến ký tự
  cuối cùng trong đó. Nếu tệp không tồn tại, một tệp mới sẽ được tạo. Trả về NULL, nếu không thể mở tệp.
  <br><br>
- “ab+” - Mở cho cả đọc và thêm ở chế độ nhị phân. Nếu tệp không tồn tại, nó sẽ được tạo.