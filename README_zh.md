[EN](https://github.com/ReverseScale/PDFPageDemo) | [中文](https://github.com/ReverseScale/PDFPageDemo/blob/master/README_zh.md)

## 🤖 要求

* iOS 9.0+
* Xcode 9.0+
* Swift

## 🚀 准备开始

## 🎨 测试 UI 什么样子？

|1.展示页 |2.展示页 |3.展示页 |
| ------------- | ------------- | ------------- | 
| ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/62891283.jpg) | ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/76653831.jpg) | ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/68509759.jpg) | 
| 展开缩放索引 | 隐藏缩放索引 | 局部放大 | 

### 🎯 安装方法

#### 安装
```Swift
import PDFKit
```

## 🛠 使用

### 核心代码
```Swift
// 声明控件
@IBOutlet weak var pdfView: PDFView!
// 加载资源
let pdfURL = Bundle.main.url(forResource: "mongodb", withExtension: "pdf")
guard let url = pdfURL else { return }
let document = PDFDocument(url: url)
pdfView.document = document
// 设置索引视图
pdfThumbnailView.pdfView = pdfView
pdfThumbnailView.thumbnailSize = CGSize(width: thumbnailDimension, height: thumbnailDimension)
pdfThumbnailView.backgroundColor = sidebarBackgroundColor
```

## ⚖ 协议

```
MIT License

Copyright (c) 2017 ReverseScale

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 😬  联系

* 微信 : WhatsXie
* 邮件 : ReverseScale@iCloud.com
* 博客 : https://reversescale.github.io
