# DOCSIFY JS

Javascript tạo file document nền web- template HTML riêng biệt - thích hợp làm các file guide, hướng dẫn, trình bày source code, các tính năng.
Không giống như [GitBook] - nó ko chỉ tạo ra các file HTMl tĩnh, nó đọc file README và chuyển thành file HTML cho website đọc.

### Tính năng:
* No statically built html files
* Simple and lightweight (~16kB gzipped)
* Smart full-text search plugin
* Multiple themes
* Useful plugin API
* Emoji support
* Compatible with IE10+

### Cài đặt
* Cài đặt Node.js (4.0.0 or later)

* Cài đặt Docsify

```
$ npm i docsify-cli -g
```

* Khởi tạo thư mục project mới của docsify ( ví dụ là ./docs)

```
$ docsify init ./docs
```

* Sau khi khởi tạo thành công thì vào thư mục docs 

```
> index.html là trang bắt đầu cho trang tài liệu của bạn.
> README.md là trang soạn nội dung homepag của bạn.
> .nojekyll 
```

* Docsify cung cấp cho chúng ta 1 local server, vì thế có thể chạy server như sau

```
docsify serve docs
```

* Preview tại Local Server

```
http://localhost:3000
```

### 1 số code tùy chỉnh

* Thêm loading text khi chờ load files
```
<div id="app">Please wait...</div>
```

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Docisfy]: <https://docsify.js.org/>
   [GitBook]: <https://www.gitbook.com/>
 