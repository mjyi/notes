# Model-View-Controller in iOS

模型 - 视图 - 控制器（MVC）设计模式为应用程序中的对象分配三个角色之一：模型，视图或控制器。该模式不仅定义了对象在应用程序中扮演的角色，还定义了对象之间的通信方式。

![mvc.png](_images/diagram-mvc.png)


- `Model` 数据层，读写数据，保存 App 状态

- `View` 页面层，和用户交互，向用户显示页面，反馈用户行为

- Controller 逻辑层，更新数据，或者页面，处理业务逻辑，是`Model`和`View`之间的媒质。

## 通信方式

在 `MVC` 中，`Model`层与`View`层并不会直接通信，二者分别可以与`Controller`通信。

### Controller ⇉ Model、Controller ⇉ View

`Controller` 可以直接调用`Model`和`View`。

### View ⇎ Model

!>　`View`和`Model`并不能通信。

### View ⇉ Controller

- Target-Action
- Delegate
- Callback

### Model ⇉ Controller

- Notification & KVO
