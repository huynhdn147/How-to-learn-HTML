# Tổng quan về HTML
--- 
## Tổng quan 
  **HTML**  (viết tắt cho HyperText Markup Language, hay là "Ngôn ngữ Đánh dấu Siêu văn bản") là một ngôn ngữ đánh dấu được thiết kế ra để tạo nên các trang web
với các mẩu thông tin được trình bày trên World Wide Web. Cùng với CSS và JavaScript, HTML tạo ra bộ ba nền tảng kỹ thuật cho World Wide Web.  
**HTML** còn được định nghĩa như là một ứng dụng đơn giản của SGML và được sử dụng trong các tổ chức cần đến các yêu cầu xuất bản phức tạp. Do vậy **HTML** đã trở thành một chuẩn  
Internet do tổ chức World Wide Web Consortium (W3C) duy trì. Phiên bản chính thức mới nhất của **HTML** là **HTML** 4.01 (1999). Sau đó, các nhà phát triển đã thay thế nó bằng 
**XHTML**.
Hiện nay, **HTML** đang được phát triển tiếp với phiên bản HTML5 hứa hẹn mang lại diện mạo mới cho Web.  

Bằng cách dùng **HTML** động hoặc **Ajax**, lập trình viên có thể được tạo ra và xử lý bởi số lượng lớn các công cụ, từ một chương trình soạn thảo văn bản đơn giản – có thể 
gõ vào ngay từ những dòng đầu tiên – cho đến những công cụ xuất bản WYSIWYG phức tạp. Hypertext là cách mà các trang Web (các tài liệu HTML) được kết nối với nhau. Và như thế,
đường link có trên trang Web được gọi là Hypertext. Như tên gọi đã gợi ý, **HTML** là ngôn ngữ đánh dấu bằng thẻ (Markup Language), nghĩa là bạn sử dụng **HTML** để đánh dấu một 
tài liệu text bằng các thẻ (tag) để nói cho trình duyệt Web cách để cấu trúc nó để hiển thị ra màn hình.  
***
## Đánh dấu
 #### các loại phần tử đánh dấu trong **HTML**:
 - Đánh dấu Có cấu trúc miêu tả mục đích của phần văn bản
 - Đánh dấu trình bày miêu tả phần hiện hình trực quan của phần văn bản bất kể chức năng của nó là gì (ví dụ, ```<b>boldface</b> ```sẽ hiển thị đoạn văn bản: **boldface**) 
(Chú ý là cách dùng đánh dấu trình bày này bây giờ không còn được khuyên dùng mà nó được thay thế bằng cách dùng CSS)  
 - Đánh dấu liên kết ngoài chứa phần liên kết từ trang này đến trang kia (ví dụ, ```<a href="http://www.wikipedia.org/">Wikipedia</a>``` sẽ hiển thị từ Wikipedia như là một liên kết ngoài đến một URL)
## Tách phần trình bày và nội dung
 - Nỗ lực tách phần nội dung ra khỏi phần hình thức trình bày của trang HTML đã đưa đến sự xuất hiện của các chuẩn mới như XHTML. Các chuẩn này nhấn mạnh vào việc sử dụng thẻ đánh dấu vào việc xác định cấu trúc tài liệu như phần đề mục, đoạn văn, khối văn bản trích dẫn và các bảng, chứ không khuyên dùng các thẻ đánh dấu mang tính chất trình bày trực quan, như ```<font>```, ```<b> (in đậm)```, và ```<i> (in nghiêng)```. Những mã mang tính chất trình bày đó đã được loại bỏ khỏi HTML 4.01 Strict và các đặc tả XHTML nhằm tạo điều kiện cho CSS. CSS cung cấp một giải pháp giúp tách cấu trúc HTML ra khỏi phần trình bày của nội dung của nó. Xem phần tách nội dung và trình bày.
 ## Cấu trúc trang HTML
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
**KHAI BÁO <!DOCTYPE>**  
- Khai báo <!DOCTYPE> định nghĩa kiểu tài liệu HTML và giúp cho trình duyệt hiển thị website một cách chính xác.  
- Nó chỉ được hiển thị một lần ở phía trên của trang. Trước bất kỳ thẻ HTML nào khác. Nó không phân biệt giữa chữ hoa và chữ thường.  
- Khai báo <!DOCTYPE> sử dụng cho HTML5 là:  
```
<!DOCTYPE html>
```
**THẺ HEAD **  <HEAD>
- Thẻ <head> được sử dụng để chứa dữ liệu về metadata.  
- Metadata là những dữ liệu phụ trợ cho một trang HTML, những dữ liệu này không hiển thị khi người dùng duyệt trang.  
- Metadata thường được dùng để định nghĩa tiêu đề của trang, gọi css, gọi scripts hay cung cấp những thông tin khác.  
- Những thẻ sau đây được coi là thẻ metadata: <title>, <style>, <meta>, <link>, <script> và <base>.  

