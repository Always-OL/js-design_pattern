learn《javascript 设计模式与开发实践》
=========

> 学习心得 

- [单例模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E5%8D%95%E4%BE%8B%E6%A8%A1%E5%BC%8F)

    
    *  惰性单例是单例模式的重点，是指在需要的时候才创建实例 

    *  创建对象和管理单例的指责分布在两个不同的方法中 这两个方法组合起来才具有单例模式的威力

    * 场景：比方在一个页面中需要初始化化多个我们自己封装的第三方sdk 类 

    创建弹框的dom对象等等

- [策略模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E7%AD%96%E7%95%A5%E6%A8%A1%E5%BC%8F)

    
    *  策略模式的目的就是将算法的实现和算法的使用分离开来

    *  策略模式利用组合、委托、和多态等技术和思想，可以有效的避免多重条件选择语句

    *  策略模式提供了对开放-封闭原则的完美支持，将算法封装在独立的strategy中

    *  应用场景也十分广泛比如接口请求返回的状态 根据不同状态执行不同的逻辑 这部分逻辑就可以抽象到单独的一个对象中 

- [代理模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E4%BB%A3%E7%90%86%E6%A8%A1%E5%BC%8F)

	* 代理模式分为保护代理和虚拟代理（缓存代理） 典型的应用是对接口请求的数据进行缓存节省流量个带宽 这在移动端显得尤为重要
	* 保护代理: 在代理对象中对本体对象的请求进行过滤 用于控制不同权限的对象对目标对象的访问
	* 虚拟代理：把一些开销很大的对象延迟到真正需要他的时候再去创建

    
- [迭代器模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E8%BF%AD%E4%BB%A3%E5%99%A8%E6%A8%A1%E5%BC%8F)

    * 迭代器模式是指提供一种方法顺序访问一个聚合对象中的各个元素 而又不需要暴露该对象的内部表示。 
    * 内部迭代器：函数内部定义好了迭代的过程
    * 外部迭代器：手工控制迭代的过程和顺序 

- [发布订阅模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E5%8F%91%E5%B8%83%E8%AE%A2%E9%98%85%E6%A8%A1%E5%BC%8F)

	* 发布订阅模式 又叫观察者模式 它定义对象间的一种一对多的依赖关系 
	* 当一个对象的状态发生改变时，所有依赖它的对象 都将得到通知 ，这也是异步的解决方案之一
	* 发布订阅模式在软件开发中占有举足轻重的位置  比如 vue中双向数据绑定  vuex redux webpack 的核心库tapable中的同步异步hook 等等

- [命令模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E5%91%BD%E4%BB%A4%E6%A8%A1%E5%BC%8F)

    * 命令模式的意图是把请求封装为对象，从而分离请求的发送者和请求的响应者之间的偶和关系 以便把响应  解偶。

- [组合模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E7%BB%84%E5%90%88%E6%A8%A1%E5%BC%8F)
	
	* 组合模式将对象组合成树形结构以表示部分到整体的层次结构除了用来表示树形结构之外 组合模式的另外一个好处是通过对象的多态性表现似的用户对单个对象的组合对象的使用具有一致性

- [模板方法模式 案例](https://github.com/FreemenL/js-design_pattern/blob/master/%E6%A8%A1%E6%9D%BF%E6%96%B9%E6%B3%95%E6%A8%A1%E5%BC%8F/index.html)

	* 模板方法模式是一种只需使用继承就可以实现的模式 

	* 模板方法模式由两部分组成 第一部分是抽象父类 第二部分是非常具体的实现子类，通常在抽象父类中封装了子类的算法框架，包括实现一些公共方法 以及封装子类中所有方法的执行顺序。

	* 框架中的生命周期函数 就是模板方法模式的体现

- [享元模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E4%BA%AB%E5%85%83%E6%A8%A1%E5%BC%8F) 

	* 享元模式可以很好地解决大量的对象带来的性能问题 

	* 享元模式的核心 是要保证内部属性的唯一 和外部状态的共享 

	* 享元模式中对象池的概念  数组实现对象的回收重复利用 

- [职责链模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E8%81%8C%E8%B4%A3%E9%93%BE%E6%A8%A1%E5%BC%8F)

	* 职责链模式的定义是：使多个对象都有机会处理请求，从而避免请求的发送者和接受者之间的耦合关系 ，将这些对象连成一条链 并沿着这条链 传递请求 直到有一个对象处理它为止 或者每个接受对象都对请求做一次处理然后交给下一个对象   

	* webpack 中的loader 对代码的处理 可以看成是职责连模式的一种应该   

	* 还有异步阻塞的情况   当前的处理依赖前一个处理的结果  

- [中介者模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E4%B8%AD%E4%BB%8B%E8%80%85%E6%A8%A1%E5%BC%8F)

	* 中介者模式的作用就是解除 对象与对象之间的紧耦合关系 ，增加一个中介者之后所有的相关对象都通过中介者来通信，而不是互相引用 ，所以当一个对象发生改变时，只需要通知中介者对象即可 ，中介者是各个对象之间耦合松散 而且可以独立的改变他们之间的交互。

- [装饰者模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E8%A3%85%E9%A5%B0%E8%80%85%E6%A8%A1%E5%BC%8F)

	* 给对象动态添加职责方式称为装饰者模式 装饰者模式能够在不改变对象自身的基础上 在程序运行期间给对象动态的规划职责 
    * 一个很典型的应用就是AOP  给ajax 请求添加请求和响应的拦截

- [状态模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E7%8A%B6%E6%80%81%E6%A8%A1%E5%BC%8F)

	* 状态模式：把对象内部的各种if else 抽取成单个的状态 并定义统一的方法 通过状态的改变进行不同的操作 

- [适配器模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/适配器模式) 

	* 适配器模式的作用是解决两个软件实体间的接口不兼容问题 使用适配器之后原本由于接口不兼容而不能工作的两个软件实体可以一起工作



#### 设计原则

	* 里氏替换原则  ：     子类必须完全实现父类的方法 可以替代父类 反过来则不行

	* 单一职责原则  ：     一个对象只干一件事情 单一职责原则被定义为引起变化的原因

	                    。如果我们有两个动机去改写一个方法 那么这个方法就有两个职责 

	                    。每个职责都是变化的一条轴线 ，如果一个方法承担了过多的职责 

	                    需要改写这个方法的可能性就越大

	* 最少知识原则  ：   最少知识原则要求我们在设计程序的时候 应当尽量减少对象之间的交互

	                   如果两个对象之间不必直接通信 那就不要发生直接的关联 

	                   常见的做法是引入一个第三者对象来承担这些对象之间的通信

	* 开放封闭原则  ：   开放封闭原则是一个看起来比较虚幻的原则

			   没有实际的模板教导我们怎样亦步亦趋的实现它，

			   可以理解为找出程序中将要发生变化的部分 然后把它封装起来

	* 好莱坞原则 ：      父类中决定何时调用子类的方法   
     

##### 拓展 
> 闭包
> 闭包会使一些数据无法被及时销毁 (常驻内存) 如果要回收这些变量 需要手动吧把这些变量设置为null 
> 闭包跟内存泄漏有关的地方是，使用闭包的同时容易形成循环引用 如果闭包的作用域链中保存着一些DOM节点 ，这时
> 候就有可能造成内存泄漏 。但这并非闭包的问题 ，也并非jsvascript的问题 ， 在ie浏览器中， 由于bom和dom中
> 的对象是使用c++，以COM对象的方式实现的 ，而COM 对象的垃圾回收机制采用的是引用记数策略 ，在基于引用计数
> 策略的垃圾回收机制中 如果两个对象之间存在循环引用那这两个对象都无法被回收，但是循环引用造成的内存泄漏本质
> 上也不是闭包造成的。  注意在实际开发中删除dom节点的时候要把其绑定的事件也删除

>AOP [面向切面编程](https://github.com/FreemenL/js-design_pattern/blob/master/%E8%A3%85%E9%A5%B0%E8%80%85%E6%A8%A1%E5%BC%8F/AOP.html)

>AOP的主要作用是把一些跟业务逻辑无关的功能抽离出来这些跟业务逻辑无关的功能通常包括日志统计，安全控制，异常处理等。把这些功能抽离出来之后，再通过动态织入的方式惨入业务逻辑模块中，这样做的好处首先是可以保持业务逻辑模块的纯净和高内聚性其次是可以很方便的复用日志统计等功能模块
