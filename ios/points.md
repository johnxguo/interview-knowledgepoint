wkwebview  
gcd,queue，NSOperation  
NSThread，队列与线程的关系，线程安全，同步，生产者消费者，有哪几种锁，自旋锁和互斥锁，线程可以取消吗，多线程与多进程  
子线程调用connection，为什么不回调，因为没有runloop  
SDWebImage内部实现，对比UIL  
复习表情面板用了哪些view实现  
UICollectionView  
左滑删除怎么实现  
网络五层结构，tcp，udp， 三次握手，四次握手 
建立连接需要三次握手是因为双方各自需要对方的SYN(seq初始序号)和ACK,要满足这一点，至少需要三个包
TCP是全双工通信，断开的时候需要四个包（FIN-ACK双方，FIN只是告诉对方我不会再发包了，但是可以接收，为什么被动方的ACK和FIN不能合并成一个包，因为可能还有包没有发完，是异步的，跟建立连接的时候不一样，但是ack要先发给主动方，免得它以为我没收到，一直重发）
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
LLDB常用命令， p, po, bt, expression, 
NSDictionary实现  
objc_msgsend，jspatch  
block，内存形式，为什么循环引用  
weak的实现  
arc，autorelease pool原理  
进程与线程，进程是资源分配的最小单位，而线程是CPU调度的最小单位。
资源包括（内存，文件句柄，信号量，消息队列）
PCB进程控制块
linux用户态的进程、线程基本满足上述概念，但内核态不区分进程和线程。可以认为，内核中统一执行的是进程，但有些是“普通进程”（对应进程process），有些是“轻量级进程”（对应线程pthread或npthread），都使用task_struct结构体保存保存。
使用fork创建进程，使用pthread_create创建线程。两个系统调用最终都都调用了do_dork，而do_dork完成了task_struct结构体的复制，并将新的进程加入内核调度。
持久化  
FMDB  
布局，layoutSubViews，masonry，约束布局计算约束  
图片在内存中的形式  
最小k数  
浏览器发送http请求的过程  
知道哪些设计模式  
深拷贝 浅拷贝  
性能优化（TableView,willDisplayCell,高度缓存，离屏渲染，离线渲染image context），缓存与批量，卡顿监控  
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
Block是将函数及其执行上下文封装起来的对象。（闭包）
copy assign retain weak  ，注意copy
NSArray的copy并不copy item，属于浅拷贝
屏幕单位  
NSCache,自己设计一个缓存器  
LRU算法  
画家算法
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
UIView和UIResponser的关系，触摸事件响应顺序 屏幕驱动IOKit-系统加入前台app的UIApplication的runloop-keywindow-hittest superview-subview

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
设计模式的六大原则
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

苹果审核规则

meshO格式

Category和Class Extension的区别是什么？
Class Extension在编译的时候，它的数据就已经包含在类信息中
Category是在运行时，才会将数据合并到类信息中


iOS沙箱怎么实现的，NSHomeDirectory，NSDocumentDirectory，NSCachesDirectory

singleton实现，dispatch_once
+ (instancetype) sharedInstance
{
    static MyClass *instance = nil;
    static dispatch_once_t onceToken;
    dispatch_once(&onceToken, ^{
        instance = [[MyClass alloc] init];
    });
    return instance;
}

一个C++源文件从文本到可执行文件经历的过程

iOS的内存管理机制

nil调用函数的返回值
nil，NULL，NSNull

反射的实现，类是元类的对象，isa指针，oc对象

objc_msgSend_stret：处理待发送消息需要返回结构体的情况，但当结构体过大，导致CPU寄存器无法容纳时，会把消息交给另一个函数派发，把返回的机构体通过分配在栈上的某个变量处理。只有写动态化框架的时候会用到

id NSObject  instancetype

尾调用优化

这个比较全  
https://zhuanlan.zhihu.com/p/77721837  

拼多多
https://zhuanlan.zhihu.com/p/99341038

clang -rewrite-objc WYTest.m

__weak的实现

block导致的内存泄露不一定是循环引用，block被其它对象持有了，导致self释放不掉

多线程必须用的例子：读写文件

mvc，mvp，mvvm是架构模式

category为什么不能添加实例变量

dyld

Runtime的弊端：太灵活，根本没必要，很乱，没有真正的私有属性，可以到处hook，到处动态添加函数，代码维护性差。好像做客户端的整天没事干就想着怎么去做个动态化，搞个jspatch

我不知道为什么会有单例这种设计模式，因为它就是反面向对象的

block的写法
直接声明：^(int){}
声明变量：NSString*(^name)(int) = ^(int){}
声明属性: @property (nonatomic, copy) NSString*(^name)(int);
函数参数: - (void)setCallback:(NSString*(^)(int))name
函数返回: - (NSString*(^)(int))getCallback;

所有问题使用需要注意的点  

为什么必须在主线程操作UI - UIKit非线程安全，也无法设计成线程安全，性能康不住
哪些OC对象是线程安全的 - NSArray这种不变的

NSMutableArray如何保证线程安全（对内部每一个操作都加锁）

首先业务代码应该尽量避免处理多线程问题

IOS多线程使用GCD与信号量实现生产者与消费者模式

Notification与多线程

MachPort

iOS中有很多进程通信的方式Mach Ports,Distributed Notifications,Distributed Objects,XPC等等

如何让UITableView在滚动的时候还有动画。两种方法，一种是NSTimer注册到NSRunLoopCommonModes，另一种是在子线程处理timer，炮事件到主线程更新UI

离屏渲染

AsyncDisplayKit(Texture)

cornerRadius一定触发离屏渲染吗

从设计的角度来看，需要使用者理解底层原理的设计，是失败的设计

GET请求的URL有长度限制，POST请求不会有长度限制