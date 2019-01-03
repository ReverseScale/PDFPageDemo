# PDFPageDemo

![](https://img.shields.io/badge/platform-iOS-red.svg) ![](https://img.shields.io/badge/language-Swift-blue.svg) ![](https://img.shields.io/badge/download-9.9MB-yellow.svg) ![](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)

[EN](https://github.com/ReverseScale/PDFPageDemo) | [中文](https://github.com/ReverseScale/PDFPageDemo/blob/master/README_zh.md)

## 🤖 Requirements

* iOS 9.0+
* Xcode 9.0+
* Swift

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

## 😬 Contributions

* WeChat : WhatsXie
* Email : ReverseScale@iCloud.com
* Blog : https://reversescale.github.io

