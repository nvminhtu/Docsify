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
* Language Hightlight

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

* Thay đổi id của app, mặc định Docsify cài đặt là id="app", nếu chúng ta muốn đổi tên id, chúng ta phải thực hiện các bước sau

- Chúng ta phải thêm thuộc tính 'el' trong script và thiết lập ở đó tên id của app mà chúng ta mới thay.
- Thêm thuộc tính data-app cho thẻ của id

```
  <!-- index.html -->

  <div data-app id="main">Please wait...</div>

  <script>
    window.$docsify = {
      el: '#main'
    }
  </script>
```

* Language Highlight
Mặc định Docsify sử dụng Prim để highlight language của chúng ta (tuy nhiên nó chỉ highlight HTML, CSS, Javascript), nếu muốn nhúng thêm thì chúng ta có thể thêm các ngôn ngữ khác như sau
```
<script src="//unpkg.com/docsify/lib/docsify.min.js"></script>
<script src="//unpkg.com/prismjs/components/prism-bash.min.js"></script>
<script src="//unpkg.com/prismjs/components/prism-php.min.js"></script>
```
Hoặc check [Component List] để tìm thêm các ngôn ngữ khác được cập nhật.

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Docisfy]: <https://docsify.js.org/>
   [GitBook]: <https://www.gitbook.com/>
   [Component List]: <https://github.com/PrismJS/prism/tree/gh-pages/components>