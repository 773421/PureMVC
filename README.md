# PureMVC
PureMVCDemo完整版
# Controller
控制器，包含了项目的业务逻辑。
# Model
模型，包含了项目的数据模型。
# View
视图，包含了项目所有的UI组件。
# Model与Proxy
Proxy（模式），提供了一个一个包装器或一个中介被客户端调用，从而达到去访问在场景背后的真实对象。Proxy模式可以方便的将操作转给真实对象，或者提供额外的逻辑。
在PureMVC中，Model保存了对Proxy对象的引用，Proxy去操作具体的数据模型（Data Object）。
# View与Mediator
Mediator（模式），定义了一种封装对象之间交互的中介. View只关心UI，具体的对对象的操作由Mediator来管理，包括添加事件监听，发送或接受Notification，改变组件状态等。
# PureMVC各层之间的交互
View可以知道Model层有什么，但是Model层不需要知道View的任何内容。Mediator访问数据可以直接通过Proxy来完成，但是如果要对Proxy具体的内容进行加工，必须要通过Controller的Command来完成


