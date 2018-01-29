# MVVM

![mvvm](_images/mvvm.png)

- `Model` 数据层，读写数据，保存 App 状态
- `View` 页面层，提供用户输入行为，并且显示输出状态
- `ViewModel` 逻辑层，它将用户输入行为，转换成输出状态
- `ViewController` 主要负责数据绑定

`MVVM`是一种从`MVC`中进化而来的设计模式，与`MVC`不同的是:
  1. 多了`View Model`
  2. View Controller 不再能够访问`Model`

`ViewModel` 能主动调用对 `Model` 做更改，也能在 `Model` 更新的时候对自身进行调整，然后通过 `View` 和 `ViewModel` 之间的绑定，对 `View` 也进行对应的更新。

`MVVM` 几点特征：

- `Model` 不可以访问其它模块（和 MVC 类似）。
- `View  Model` 只能访问 `Model`
- `View Controller` 不能直接访问`Model`，只能与`View` 和`View Model`交互。
- `View` 只能访问 view controllers，通知它们交互事件（和 MVC 类似）。

### 数据绑定

- 基于`KVO` 绑定
- 使用 `函数式响应编程`框架，如 [ReactiveCocoa][ReactiveCocoa], [RxSwift][RxSwift]

### 参考资料

[iOS 架构模式 - 简述 MVC, MVP, MVVM 和 VIPER (译)](https://blog.coding.net/blog/ios-architecture-patterns)

[ReactiveCocoa]: https://github.com/ReactiveCocoa/ReactiveCocoa
[RxSwift]: https://github.com/ReactiveX/RxSwift

