tesseract-clipboard
=====================

![](https://github.com/xulihang/tesseract-clipboard/raw/master/demo.gif)

This program will convert images stored in the clipboard to texts using [tesseract ocr engine](https://github.com/tesseract-ocr/tesseract).

It is written in b4j and tesseract is open sourced, thus it is cross-platform.


Installation
-------------

tesseract and jre8 are needed to run this program.

See [here](https://github.com/tesseract-ocr/tesseract/wiki) for tesseract installation.

I would like to run a portable tessract in windows. So if there is tesseract in the path, it will use the tesseract installed in the system. If not, it will run the tesseract I put under the app's root.

```
If tesseractInstalled Then
    sh1.Initialize("sh1","tesseract",args)
Else
    sh1.Initialize("sh1",File.Combine(File.Combine(File.DirApp,"tesseract-ocr"),"tesseract"),args)
End If 
```

How to capture screen
----------------------

We can use operating systems' built-in screencapture shortcuts to get images into the clipboard. 

Windows 10: win+shift+s

macOS: Command+shift+4

Linux: Ctrl+Shift+PrntScrn

