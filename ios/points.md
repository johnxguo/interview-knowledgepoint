wkwebview
gcd,queue，NSOperation
NSThread，队列与线程的关系，线程安全，同步，生产者消费者，有哪几种锁，自旋锁和互斥锁，线程可以取消吗，多线程与多进程
子线程调用connection，为什么不回调，因为没有runloop
SDWebImage内部实现，对比UIL
复习表情面板用了哪些view实现
UICollectionView
左滑删除怎么实现
网络五层结构，tcp，udp，
http，https，http2,http请求头和响应头，cookie，断点续传原理
MVVM vs MVC vs MVP，MVC缺点（想一下MVVM缺点，反怼面试官），
clock
除了instruments，怎么检测内存泄漏（MLeaksFinder，原理）
id，nil, NULL,发消息
机型适配
oc-runtime，方法hook，（交换方法，创建类，给新创建的类增加方法，改变isa指针）
runloop，mode，nstimer
viewcontroller的生命周期
app前后台
kvo
LLDB常用命令
NSDictionary实现
objc_msgsend，jspatch
block，内存形式，为什么循环引用
weak的实现
arc，autorelease pool原理
进程与线程
持久化
FMDB
布局，layoutSubViews，masonry，约束布局计算约束
图片在内存中的形式
最小k数
浏览器发送http请求的过程
知道哪些设计模式
深拷贝 浅拷贝
性能优化（TableView,），缓存与批量，卡顿监控
YYModel, json转Model
架构设计
编译过程，xcode的编译选项
签名
IAP
UIApplication 生命周期
APNS
发布流程
擅长的
难点
减包
frame和bounds有什么不同?
NSString为什么用copy
方法和选择器有何不同?
injectionforxcode，原理
自定义导航跳转动画
method swizzling
类别与扩展的实现原理
引用计数
copy assign retain weak
屏幕单位
NSCache,自己设计一个缓存器
LRU算法
深搜广搜，递归，queue
字符串翻转
encoding
cocopods, podspec, podfile， pod install与pod update
layoutIfNeeded与setNeedsLayout
https抓包原理
isEquel和hash的关系
bitmap的结构
可变数组的实现
如何hook一个对象的方法，不影响其它对象
如何避免if else
数组copy,里面的元素会copy吗
tcp为什么是三次握手，四次挥手
看过什么开源代码，优秀三方开源代码阅读
GLSurfaceView,shader,绘制流程
多进程通讯，binder机制
Volley，Eventbus
delegate, notification,kvo,block优缺点
在一个UI的正中间实现一个正方形的红色视图有几种方式
做动画有几种方式
UIView和UIResponse的关系，触摸事件相应顺序
UIViewcontroller的view什么时候加载
UILabel和自绘哪个性能好，内存少，为什么
ipV6,
AFNetworking，是否支持ipV6
编译架构，arm64,i386
手动还原符号表，查看ipa架构，二进制，linkmap等
iosapp有几种状态，后台的时候代码是否执行，按Home键是否执行，不同版本之间有什么区别
内存泄漏查找，卡顿检测，非instrument
object copy为什么是浅拷贝，实现了哪个协议
DNS，网络故障排查
TCP连接断开的过程
get post put
MVVM如何实现绑定
找出数组中重复的数字
程序在运行时，os除了分配内存还做了什么
怎么收集crash，bugly的原理（系统设置，堆栈还原）
在block里面 setValueForKey
oc中对象内存模型
ping是什么协议，原理
MTU
arc和mrc的本质区别
存一个通讯录，包括增删改查，用什么数据结构
autorelease变量什么时候释放，手动添加时在变量生命周期结束，系统最终释放是在当前runloop当前循环结束的时候，那子线程的autorelease变量什么时候释放
子线程里面需要加autoreleasepool吗
init做什么，viewdidload做什么
init里面设置背景颜色为什么会生效
对ios的最新特性有关注吗
2链表找共同节点，判断链表环
链表倒数第k个节点
链表某个值大的放左边，小的放右边
中序遍历，非递归
二叉树遍历（前序、中序、后序、层次遍历、深度优先、广度优先）
App用户量
怎么提升app启动速度，什么工具调试
约束layout和手动布局的优缺点
UIView在什么手机对subviews进行布局
自绘有哪些方法,CGLayer
第k大数
离屏渲染
block变量截获
加密  对称非对称，签名
网络地址转换nat
tcp可靠数据传输，滑动窗口，拥塞控制
ios应用导航模式有哪些
iOS 中持久化方式有哪些？
iOS 单元测试框架有哪些？
atomatic, nonatomic
class和struct的区别
kvo与kvc
delegate与nsnotifition
常用sql语句
iOS @synthesize、@dynamic的理解?
沙盒的理解
如何进行真机调试  证书
json解析用什么库，pb如何减包
iOS ASIHttp
socket http
Apple设备尺寸和编程尺寸?
iOS 使用block有什么好处？使用NSTimer写出一个使用block显示（在UILabel上）秒表的代码?
cell重用的问题?
performSelector传入3个以上参数，其中一个为结构体?
解释self = [super init]方法?
Core Data的6成员对象?
isMemberOfClass 和 isKindOfClass 联系与区别?
如何动态创建对象，如何反射
iOS @public、@protected、@private 它们的含义与作用?
 #include与#import的区别、**#import **与@class 的区别?
键路径(keyPath)、键值编码（KVC）、键值观察（KVO）?
category优点和缺点?
内存管理基本原则?
Category 为什么只能加方法不能加属性?
Category理论上不能添加成员变量,但是可以使用@dynamic(即运行时Runtime)来弥补这种不足
热更新方案
ocs原理，llvm，clang, 抽象语法树
iOS Category 中有 load 方法吗？load 方法是什么时候调用的？load 方法能继承吗？
main()之前的过程有哪些?
组件化方案
oc消息机制
实现 NSNotificationCenter，讲一下思路?  弱引用
为什么是三次握手？为什么是四次挥手？三次挥手不行吗？
HTTPS 密钥传输流程?
系统框架里使用了哪些设计模式？至少说6个?
Alamofire 比直接使用 URLSession，优势是什么？
手写一下快排?
找出两个字符串的最大公共子字符串?
StoryBoard
gcd  信号量
block的实质
为什么在默认情况下无法修改被block捕获的变量？ __block都做了什么？
模拟一下循环引用的一个情况？block实现界面反向传值如何实现？
什么时候会报unrecognized selector错误？iOS有哪些机制来避免走到这一步？
objc在向一个对象发送消息时，发生了什么？
iOS 能否向编译后得到的类中增加实例变量？能否向运行时创建的类中添加实例变量？为什么
主线程默认开启了runloop么？子线程呢？
为什么把NSTimer对象以NSDefaultRunLoopMode（kCFRunLoopDefaultMode）添加到主运行循环以后，滑动scrollview的时候NSTimer却不动了？
isa指针？（对象的isa，类对象的isa，元类的isa都要说）
运行时能增加成员变量么？能增加属性么？如果能，如何增加？如果不能，为什么？
[nil method]的返回值
iOS UITableview的优化方法（缓存高度，异步绘制，自绘，减少层级，hide，避免离屏渲染,ios版本影响，圆角）
集合操作符
UITableViewCell上有个UILabel，显示NSTimer实现的秒表时间，手指滚动cell过程中，label是否刷新，为什么？
iOS 有a、b、c、d 4个异步请求，如何判断a、b、c、d都完成执行？如果需要a、b、c、d顺序执行，该如何实现？
一个view已经初始化完毕，view上面添加了n个button，除用view的tag之外，还可以采用什么办法来找到自己想要的button来修改button的值?
NSTimer内存泄漏
ios代码混淆方法，，https://blog.csdn.net/u014220518/article/details/95482006
ios编译产物里面是否有方法名等信息
enable BitCode是什么
NSURLConnection
volatile
Core Animation
Core Audio
Core Data
下面是 Cocoa Touch 中一小部分可用的框架：
   音频和视频：Core Audio ，OpenAL ，Media Library ，AV Foundation
   数据管理 ：Core Data ，SQLite
   图形和动画 ：Core Animation ，OpenGL ES ，Quartz 2D
   网络：Bonjour ，WebKit ，BSD Sockets
   用户应用：Address Book ，Core Location ，Map Kit ，Store Kit

如何让键盘弹出

Socket开发，底层长连接


如果我们不创建内存池，是否有内存池提供给我们?
答:界面线程维护着自己的内存池，用户自己创建的数据线程，则需要创建该线程的内存池


这个比较全
https://zhuanlan.zhihu.com/p/77721837


所有问题使用需要注意的点
