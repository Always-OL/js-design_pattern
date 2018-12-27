learn《javascript 设计模式与开发实践》
=========

> 学习新心得 

**[单例模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E5%8D%95%E4%BE%8B%E6%A8%A1%E5%BC%8F)

    
    *  惰性单例是单例模式的重点，是指在需要的时候才创建实例 
    
    *  创建对象和管理单例的指责分布在两个不同的方法中 这两个方法组合起来才具有单例模式的威力
**[策略模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E7%AD%96%E7%95%A5%E6%A8%A1%E5%BC%8F)

    
    *  策略模式的目的就是将算法的实现和算法的使用分离开来

    *  策略模式利用组合、委托、和多态等技术和思想，可以有效的避免多重条件选择语句

    *  策略模式提供了对开放-封闭原则的完美支持，将算法封装在独立的strategy中
**[命令模式 案例](https://github.com/FreemenL/js-design_pattern/tree/master/%E5%91%BD%E4%BB%A4%E6%A8%A1%E5%BC%8F)

    * 命令模式的意图是把请求封装为对象，从而分离请求的发送者和请求的响应者之间的偶和关系 以便把响应  解偶。


##### 拓展 
> 闭包
> 闭包会使一些数据无法被及时销毁 (常驻内存) 如果要回收这些变量 需要手动吧把这些变量设置为null 
> 闭包跟内存泄漏有关的地方是，使用闭包的同时容易形成循环引用 如果闭包的作用域链中保存着一些DOM节点 ，这时
> 候就有可能造成内存泄漏 。但这并非闭包的问题 ，也并非jsvascript的问题 ， 在ie浏览器中， 由于bom和dom中
> 的对象是使用c++，以COM对象的方式实现的 ，而COM 对象的垃圾回收机制采用的是引用记数策略 ，在基于引用计数
> 策略的垃圾回收机制中 如果两个对象之间存在循环引用那这两个对象都无法被回收，但是循环引用造成的内存泄漏本质
> 上也不是闭包造成的。  注意在实际开发中删除dom节点的时候要把其绑定的事件也删除
