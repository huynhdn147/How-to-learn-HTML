 # Cấu trúc thẻ HTML
 ----
 Một thẻ HTML sẽ có cấu trúc như sau
 ``` 
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Tiêu đề trang web</title>
</head>
<body>
    Nội dụng trang web
</body>
</html>
```
1. **KHAI BÁO <!DOCTYPE>**  
- Khai báo <!DOCTYPE> định nghĩa kiểu tài liệu HTML và giúp cho trình duyệt hiển thị website một cách chính xác.  
- Nó chỉ được hiển thị một lần ở phía trên của trang. Trước bất kỳ thẻ HTML nào khác. Nó không phân biệt giữa chữ hoa và chữ thường.  
- Khai báo <!DOCTYPE> sử dụng cho HTML5 là:  
```
<!DOCTYPE html>
```
2. **Thẻ HEAD**  
- Thẻ <head> được sử dụng để chứa dữ liệu về metadata.  
 Ví dụ
 ```
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta http-equiv="X-UA-Compatible" content="ie=edge">
   <title>Tiêu đề trang web</title>
</head>
 ```
- Metadata là những dữ liệu phụ trợ cho một trang HTML, những dữ liệu này không hiển thị khi người dùng duyệt trang.  
- Metadata thường được dùng để định nghĩa tiêu đề của trang, gọi css, gọi scripts hay cung cấp những thông tin khác.  
- Những thẻ sau đây được coi là thẻ metadata: ```<title>```, ```<style>``` , ```<meta>```,```<link>```, ```<script>``` và ```<base>``` .  
- **Không khuyến khích** Bạn có thể làm giảm sự phức tạp trong HTML bằng cách bỏ thẻ ```<head>```, Ví Dụ:
 ```
 <!DOCTYPE html>
<html>
<title>Tiêu đề trang</title>
<body>
 
<h1>Đề mục</h1>
<p>Đoạn văn bản.</p>
 
</body>
</html>
```
2.1.**Tiêu đề ```<title>```**
- Thẻ <title> được dùng để tạo tiêu đề cho trang HTML.
- Thẻ <title> là thẻ bắt buộc trong HTML/XHTML.
- Thẻ <title> có các chức năng:  
  * tạo tiêu đề cho trang, hiển thị trên thanh công cụ của trình duyệt  
  * được sử dụng làm tên trang khi bạn lưu vào bookmark của trình duyệt  
  * hiển thị ở phần tiêu đề trang trong kết quả tìm kiếm (VD: tìm kiếm của google)  
Ta có thể thấy qua Ví dụ sau:  
```<!DOCTYPE html>
<html>
<title>Tiêu đề của trang</title>

<body>
<p>Nội dung trong thẻ body sẽ được hiển thị trong cửa sổ trình duyệt.</p>
<p>Nội dung trong thẻ title sẽ không hiển thị.</p>
</body>

</html>
```
**Kết quả**
```
Nội dung trong thẻ body sẽ được hiển thị trong cửa sổ trình duyệt.

Nội dung trong thẻ title sẽ không hiển thị.
```
---
2.2.**Thẻ ```<style>``` trong HTML:**
- Thẻ <style> được sử dụng để chứa kiểu trang trí cho trang HTML.
- Trong thẻ <style> bạn có thể quy định cách các thành phần HTML sẽ được hiển thị trên trình duyệt:
 Ví Dụ:
 ```
 <!DOCTYPE html>
<html>

<title>Tiêu đề trang</title>

<style>
body {background-color:yellow;}
p {color:blue;}
</style>

<body>
<h1>Đây là đề mục</h1>
<p>Đây là đoạn văn bản.</p>
</body>

</html>
```
**Kết quả**  

![Kết quả](https://github.com/huynhdn147/SourceImage/blob/master/115744921_3332021253690574_2369636928626870614_n.png)  
---
2.3.**Thẻ ```<link>``` trong HTML:**
- Thẻ ```<link>``` dùng để liên kết tới các tài nguyên bên ngoài trang HTML.  
- Thẻ ```<link>``` có thể được dùng để gọi tới các tệp tin CSS:  
```<link rel="stylesheet" href="style.css">```  

2.4.**Thẻ `<meta>` trong HTML**
- Thẻ <meta> được sử dụng để tạo miêu tả, từ khóa, thông tin tác giả và các thông tin khác cho trang HTML.
- Những thông tin này được sử dụng bởi trình duyệt (cách hiển thị nội dung), bởi các công cụ tìm kiếm (từ khóa) và những dịch vụ web khác.  
- Các Ví dụ về thẻ `<meta>`  
  * Tạo từ khóa dành cho các công cụ tìm kiếm:  
`<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">`  
  * Tạo miêu tả:
`<meta name="description" content="Đây là thẻ Meta"`  
  * Thông báo bộ mã ký tự mà trang sử dụng:  
`<meta charset="UTF-8">`
  * Tạo thông tin tác giả:  
`<meta name="author" content="WebVN">`  
  * Làm mới lại trang HTML sau mỗi 30 giây:  
`<meta http-equiv="refresh" content="30">`
- Chỗ đứng của thẻ `<meta>` trong html:  
  - Các thẻ meta được dùng đằng trước thẻ body.  
**Ví dụ**
```
<!DOCTYPE html>
<html>
 <head>
<meta name="description" content="Tự học lập trình web với HTML và CSS">
<meta name="keywords" content="HTML,CSS,XML,JavaScript">
<meta name="author" content="WebVN">
<meta charset="UTF-8">
 </head>
<body>
<p>Các thẻ meta được dùng đằng trước thẻ body.</p>
</body>
 
</html>
```
2.5.**Thẻ <script> trong HTML**
- Thẻ <script> được sử dụng để viết các đoạn mã với ngôn ngữ  JavaScript.  
Ví dụ:  
```
<!DOCTYPE html>
<html>
<body>
 
<p id="demo"></p>
 
<script>
document.getElementById("demo").innerHTML = "Xin chào JavaScript!";
</script>
 
</body>
</html>
```
Chúng ta sẽ đi sâu hơn với thẻ `<script>` và ngôn ngữ JavaScript tại [đây](https://www.facebook.com/huynh14789)  
2.6.**Thẻ `<base>` trong HTML:**  
- Thẻ <base> được sử dụng để quy định cách hiển thị liên kết và địa chỉ cho tất cả các liên kết tương đối trong trang.
  - Câu hỏi:`Sự khác nhau giữa l iên kết tương đối và liên kết tuyệt đối là gì?`
  - Trả lời:` Liên kết tương đối là những liên kết không có chứa domain, VD: “/page”. Còn liên kết tuyệt đối là liên kết có bao gồm đầy đủ cả domain,VD:  “http://domain.com/page”`  
- Ví dụ về thẻ `<base>`:  
`<base href="https://webvn.com/wp-content/uploads/2014/12/" target="_blank">`  
Nếu trong thẻ body chúng ta có khai bảo một thẻ `<img>` Ví dụ: `<img src="pic_html5.gif">`  
Vì ta đã quy định địa chỉ trong thẻ `<base>` trình duyệt sẽ tự động tìm ảnh tại địa chỉ `"https://webvn.com/wp-content/uploads/2014/12/pic_html5.gif"` và sẽ tự động mở một trang mới vì chúng ta có khai báo thuộc tính target của thẻ `<base>` là "_blank"


