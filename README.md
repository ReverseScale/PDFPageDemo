# PDFPageDemo

![](https://img.shields.io/badge/platform-iOS-red.svg) ![](https://img.shields.io/badge/language-Swift-blue.svg) ![](https://img.shields.io/badge/download-9.9MB-yellow.svg) ![](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)

[EN](#Requirements) | [中文](#中文说明)

## 🤖 Requirements

* iOS 9.0+
* Xcode 9.0+
* Swift

## 🚀 Getting started

## 🎨 Why test the UI?

|1.Show Page |2.Show Page |3.Show Page |
| ------------- | ------------- | ------------- |
| ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/62891283.jpg) | ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/76653831.jpg) | ![](http://ghexoblogimages.oss-cn-beijing.aliyuncs.com/19-1-3/68509759.jpg) | 
| Expand Zoom Index | Hide Zoom Index | Zoom in |

### 🎯 Installation

#### Install

```Swift
import PDFKit
```

## 🛠 Used

### Core code

```Swift
// Declare the control
@IBOutlet weak var pdfView: PDFView!
// Load resources
let pdfURL = Bundle.main.url(forResource: "mongodb", withExtension: "pdf")
guard let url = pdfURL else { return }
let document = PDFDocument(url: url)
pdfView.document = document
// Set index view
pdfThumbnailView.pdfView = pdfView
pdfThumbnailView.thumbnailSize = CGSize(width: thumbnailDimension, height: thumbnailDimension)
pdfThumbnailView.backgroundColor = sidebarBackgroundColor
```


## 📝 App Submission

## ⚖ License

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

## 😬 Contributions

* WeChat : WhatsXie
* Email : ReverseScale@iCloud.com
* Blog : https://reversescale.github.io

