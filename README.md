SwiftObjcCocoapodsExample
=========================

Swift ,Objective-C and Cocoapods mix and match example

It demonstrated :
* Swift calling Swift function 
* Swift calling Objective-C function
* Objective-C calling Swift function
* Swift calling Objective-C function from Swift function
* and integrated Cocoapods with powerful libs created by Objective-C


SwiftIPManager.swift
一個使用 AFNetworking 取得 IP 的類別
並且 定義 @objc 開放給 Objective-C 呼叫

ObjcIPManager.h
裡面提供兩個 function: 
  1. getIP (使用 Objective-C 語法)
  2. getIPFromSwift (在 Objective-C 中 呼叫 Swift)

#ViewController.swift
```swift
// call Swift
SwiftIPManager.getIP()

// call ObjC
ObjcIPManager.getIP()

// from Objc call Swift
ObjcIPManager.getIPFromSwift()
```
