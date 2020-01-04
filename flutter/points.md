为什么用dart(双模，AOT，JIT)
Future，协程，响应式编程，async await
状态管理
Stream，StreamController ，StreamSink ， map, rx相关操作
zone
渲染流程
platformchannel，非线程安全，实验看下同步异步，线程模型
statelesswidget， statefulwidget
Flutter 中存在 Widget 、 Element 、RenderObject 、Layer 四棵树，其中 Widget 与 Element 是一对多的关系 ，
setState 
InheritedWidget 
key, 刷新机制
statefulwidget生命周期，
initState， didChangeDependencies，deactivate， dispose， didUpdateWidge 
build
FlutterEngine的线程模型，isolate
Flutter 中存在四大线程，分别为 UI Runner、GPU Runner、IO Runner， Platform Runner （原生主线程） ，同时在 Flutter 中可以通过 isolate 或者 compute 执行真正的跨线程异步操作。（找到原始英文文档阅读）
PlatformView
mixins （本质是继承）
hitTest， gesturedetector opacity，behavior
FlutterEngine启动流程，渲染流程
dart是值传递还是引用传递
Widget和element和RenderObject之间的关系
widget的root节点，挂在哪里
mixin extends implement之间的关系
Future和microtask执行顺序
..操作符
await for， listen
Dart 在单线程中是以消息循环机制来运行的，其中包含两个任务队列，一个是“微任务队列” microtask queue，另一个叫做“事件队列” event queue。
Plugin
状态管理
ScopedModel•BLoC•Redux / FishRedux•Provider
如何统一管理错误页面？
ErrWidget.builder
如何获得一个context（有一个widget叫Buider）
异步widget, FutureBuilder, StreeamBuilder
ListView
flutter_boost
flutter与React Native有什么不同？
Flutter中定义边距和填充？
Texture widget, 视频渲染，platformview，实现方式对比
开启摄像头
处理键盘
Stream有两种订阅模式：单订阅(single) 和 多订阅（broadcast）
FrameWork层和Engine层，分别负责什么
编译engine代码
绘制流程，vsync
路由，自定义route
MaterialApp
image.network  缺点， 共享native图片缓存
_私有变量，相对什么来说私有
统一处理异常，crash上报
运算符重载
事件机制，竞技场
Widget 和 element 和 RenderObject
什么是Navigator? MaterialApp做了什么
const  final   static  
Constant constructors, Factory constructors

