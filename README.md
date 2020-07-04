首先unity是什么？
有人说unity是一个游戏引擎，组件式开发，没错，开发人员利用它可以快速开发出游戏。
有的说它是一个工具集合，Unity集合从开发到打包发布的各种工具，包括了代码编辑，编译，切图，压缩，动画制作，网络通讯工具等等，显然这个说法也没错。
也有的人说它是一个总体解决方案，提供了UI，数据存储，网络通信端，图形渲染，物理渲染，输入输出，动画，视频语言播放等等方案，这个说法也对。
还有人的人说，它就是一个类库，组件也好，工具也罢，都不过是类的变现形式，所有的使用最终都是通过类的接口来调用而已，只不过有一些操作用软件的UI来替代了代码的编写，说的也有道理。
理论上，这些说法都是对，只是看问题角度不同，横看成岭侧成峰。
总结来说，Unity是组件式开发引擎，包含开发工具集合，提供一站式解决方案和各种类库。

## 为什么要建立体系
- 1、搭建的过程就是学习的过程，输出是最好的学习方式。
- 2、体系可以帮助快速定位知识点和问题，提高开发效率

## 学习和搭建思路
- 提出问题，思考问题，解决问题。
- 收集知识点，包括理论和案例，对知识点组合拆分，不断提出问题，归纳总结，去用实践。
- 查百度，看手册，读别人的代码。
- 用工程和代码去实践，验证想法。
- 输出，按条理写到博客上，较大的工程和代码，项目之类的可以放到GitHub上

##### 说明
这整个系列已经建立了一个主题:Unity知识体系。
这个总目录首页相当于一个入口或者说框架约定。每个问题地下都会有对应的链接到具体的子页面。
可以针对某个子目录的某个问题做出解答，也可以自己提出新的问题自己做解答，或者让别人解答。
我会维护更新这个总目录，不断增加，修改。
正在学习unity的朋友或者有兴趣一起管理这个主题的朋友欢迎加入进来。

## 学习目标 
总体目标概述：这可能会要求自己能熟练使用unity软件，熟悉unity组件和类库API，还会需要自己对C#语言运用自如，能用代码灵活处理游戏里的各种实际问题，熟悉各类型游戏的业务流程和框架，最后是对游戏性能优化和渲染优化。

### Unity
理解并熟练使用

- **软件操作**
1、软件去哪里下载安装？如何找到自己想要的版本？
现在装unity已经相当简单了，一键下载安装，而且自带VS。没收藏地址就百度一次。
2、如何查看一个工程的版本？
3、如何配合使用VS调试Unity？
4、软件通常有哪些面板？
场景、Game面板、场景结构、检视面板、工程资源、打印。
5、面板上锁是什么？干嘛的？
6、什么是unity资源？如何找资源？AssetStore？蛮难网？各种教程网？
7、如何导入package到工程中？
8、如何打包出一个桌面应用？有哪些选项？
9、打包到其他平台又需要哪些点？比如打包安卓平台？
10、精灵图集如何切割？
11、动画模型如何导入？材质贴图丢失了怎么办？

-  **理解unity里的概念**
1、GameObject、相机、场景、灯光、烘焙、材质、贴图、模型、图集又是什么？
2、预制体、脚本、插件、组件、属性、
3、锚点、中心点
4、世界坐标、本地坐标、子物体、父物体
5、精灵Sprite，Texture是什么？引申：Sprite <-> Texture2D <->  bytes[]，这三种图片数据如何互相转化？
6、Unity里的特殊文件夹有哪些？Resource、SteamingAssets，可以先从字面意思想一下，Resource资源，SteamingAssets热气腾腾的资源？
7、脚本的生命周期，各个函数的意义和使用要点
8、Awake，Start，Onable，OnDisable， 脚本和物体禁用开启时，怎么个调用？
9、drawcall是什么？如何优化？
10、什么是协程？有什么用？怎么用？

-  **游戏物体**
游戏是有场景组成的，场景又是有各种游戏物体组成的，游戏物体又由各种组件组成的。
1、GameObject
2、各种2D和3D物体
3、Camera
4、Sprite
5、Light
6、模型、材质、贴图
7、画布Canvas
8、各种UI
      - Image
      - Text
      - Button
      - ...
9、如何去搭游戏的场景？

-  **组件**
1、Transform
2、MeshRender
3、Collider
4、Rigidboy
5、NavmeshAgent
6、音频 Audio Listener  Audio Source
7、...

- **API**
不管游戏物体还是组件，通常都是静态的，要他们能够运作起来，并且更好地使用他们，还需要很多的API。
1、移动
2、旋转
3、查找
4、输入类

### C#语言
需要写脚本来管理游戏资源和控制游戏逻辑。

1、语法，如同英语的语法。

变量、声明、定义、修饰符，函数、类与实例，这些是基本元素，每一个元素都要知道是什么，有哪些类型，如何写，而是要熟练使用。

比如一个函数参数有哪些类型，如何写？值传递和引用传递是怎样的？

比如修饰符，static表示什么，在哪些场合有哪些用处？

又比如类的构造函数有几种类型，怎样写，有派生时类的生命周期是怎样的？

2、C#里的数据结构。

命名空间、基本数据类型、结构体、枚举、数组、列表、字典、栈、队列、表、树。每中结构的特性，常用接口。

3、C#的高级特性，往往是这些特点才促成了这门语言。

（1）面向对象，这个就有点多了，特点是封装，继承，多态，这个方面更多是设计思想方面的东西。

（2）属性。作用是什么，可以分开一个类的变量的访问和修改权限，还可以限制变量的数值范围，保护数据安全。

（3）泛型函数。有什么用？怎么写？

（4）Lambda表达式。有什么用，一是Lambda表达式替代委托，简化代码。二是在集合中如List，Dictionary，数组中查找或者筛选，不用写循环。此外我认为是，可以更好地读懂别人的代码，假如你不用甚至不懂Lambda表达式，你看别人的有Lambda表达式的代码，你就不容易读懂。

（5）委托。委托为了解决观察者模式的缺陷而出现，那观察者模式有什么缺陷，观察者必须要拥有被观察对象，有了委托后不需要拥有观察者对象，但仍然依赖被观察者对象。

C#委托是很重要的应用，很多场合都需要用它。

（6）事件。事件实际是一种特殊的委托，事件规定了只能在事件拥有者方(观察者)才能调用事件。

（7）接口。有什么用？怎么用？有哪些使用场合？

（8）抽象函数。有什么用？怎么用？有哪些使用场合？

（9）虚函数。灵魂三连问？

### 设计模式
一些问题，如果能归纳为某种模式，那么不仅能简化代码，也能触类旁通，思考问题的一般方法。

- 单例
- 观察者模式
- 状态机
- 工厂模式
- ......

### 游戏里的实际应用
- 如何加载场景？
    - [协程和回调应用：异步加载场景、传出战斗计算]([https://github.com/linguoyuan/Unity/blob/master/5_%E5%85%B7%E4%BD%93%E5%BA%94%E7%94%A8/01_%E5%9C%BA%E6%99%AF%E5%8A%A0%E8%BD%BD%E5%92%8C%E6%88%98%E6%96%97%E8%AE%A1%E7%AE%97.cs)
)
- 如何制作血条？
- 怪物的AI？ 

### 项目实战


(后续还要补充很多内容,慢慢修改)
游戏框架。
插件。
工具链。
对外接入，如SDK。
