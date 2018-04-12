### 前言
这个系列的笔记是记录Android常见的23种设计模式。会记录每种设计模式的设计思想，表现形式和使用情景。本人健忘，因此记录下学习过程，以便后续的查询工作。通过设计模式地学习，能够有效地降低阅读源码的门槛，减少阅读源码时瞌睡的几率。

---

### 什么是设计模式？
>通俗来讲，设计模式就是针对某一种特殊场景而给出的标准解决方案，它是前辈们的经验性总结。

更通俗一点讲，就是为了解决一类问题，大牛们总结出的开发套路。

---

### 为什么要使用设计模式？
>设计模式是实现软件工程化的基础。良好的设计模式应用，可以使我们的软件变得更加健壮可维护。

既然是大牛们的经验之实，必然有很强的可取之处，可以说是解决问题的最优解，广泛地使用设计模式，不仅能让我们的代码更清晰，也能使我们的程序更稳定。同一个世界，同一套设计模式，开源的可读性方面也能够得以保障。

---

### 设计模式的六大原则
常见的设计模式有23种之多，甚至随着Android的不断发展，越来越多的设计模式得到广大开发者的认可。难道这些设计模式都是天马行空想到的吗？

做任何事都要遵从一些规范，才能得到广泛的认可。Android设计模式就需要遵从如下六大原则去设计去丰富。
![设计模式六大原则](http://7xslhx.com1.z0.glb.clouddn.com/android_pic/%E5%85%AD%E5%A4%A7%E5%8E%9F%E5%88%99.png)

> [1. 单一职责原则(SRP Single Responsibility Principle)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E5%8D%95%E4%B8%80%E8%81%8C%E8%B4%A3%E5%8E%9F%E5%88%99.md) √
> 
> [2. 开放封闭原则(OCP Open Closed Principle)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E5%BC%80%E6%94%BE%E5%B0%81%E9%97%AD%E5%8E%9F%E5%88%99.md) √
> 
> [3. 里氏替换原则(LSP Liskov Substitution Principle)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E9%87%8C%E6%B0%8F%E6%9B%BF%E6%8D%A2%E5%8E%9F%E5%88%99.md) √
> 
> [4. 依赖倒置原则(DIP Dependence Inversion Principle)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E4%BE%9D%E8%B5%96%E5%80%92%E7%BD%AE%E5%8E%9F%E5%88%99.md) √
> 
> [5. 迪米特原则(LoD Law of Demeter)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E8%BF%AA%E7%B1%B3%E7%89%B9%E5%8E%9F%E5%88%99.md) √
> 
> [6. 接口隔离原则(ISP Interface Segregation Principle)](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%85%AD%E5%A4%A7%E8%AE%BE%E8%AE%A1%E5%8E%9F%E5%88%99%E4%B9%8B%E6%8E%A5%E5%8F%A3%E9%9A%94%E7%A6%BB%E5%8E%9F%E5%88%99.md) √

---

### 常见的设计模式
以此六大原则为基础，结合具体的情景，衍生出了一系列的设计模式。常见的设计模式大概有24种，可以归纳为三种类型：

![image](http://7xslhx.com1.z0.glb.clouddn.com/android_pic/%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F.png)

**创建型设计模式**

> [1. 创建型设计模式——单例模式](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%88%9B%E5%BB%BA%E5%9E%8B%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E4%B9%8B%E5%8D%95%E4%BE%8B%E6%A8%A1%E5%BC%8F.md) √
> 
> [2. 创建型设计模式——建造者模式](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%88%9B%E5%BB%BA%E5%9E%8B%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E4%B9%8B%E5%BB%BA%E9%80%A0%E8%80%85%E6%A8%A1%E5%BC%8F.md) √
> 
> [3. 创建型设计模式——原型模式](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%88%9B%E5%BB%BA%E5%9E%8B%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E4%B9%8B%E5%8E%9F%E5%9E%8B%E6%A8%A1%E5%BC%8F.md) √
> 
> [4. 创建型设计模式——简单工厂模式](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%88%9B%E5%BB%BA%E5%9E%8B%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E4%B9%8B%E7%AE%80%E5%8D%95%E5%B7%A5%E5%8E%82%E6%A8%A1%E5%BC%8F.md) √
> 
> [5. 创建型设计模式——工厂模式](https://github.com/ColdPuppy/Android-Notes/blob/master/Android-Design-Pattern/%E5%88%9B%E5%BB%BA%E5%9E%8B%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E4%B9%8B%E5%B7%A5%E5%8E%82%E6%96%B9%E6%B3%95%E6%A8%A1%E5%BC%8F.md) √
> 
> [6. 创建型设计模式——抽象工厂模式]()

**结构型设计模式**

> [1. 结构型设计模式——适配器模式]()
> 
> [2. 结构型设计模式——组合模式]()
> 
> [3. 结构型设计模式——装饰模式]()
> 
> [4. 结构型设计模式——外观模式]()
> 
> [5. 结构型设计模式——桥接模式]()
> 
> [6. 结构型设计模式——享元模式]()
> 
> [7. 结构型设计模式——代理模式]()

**行为型设计模式**

> [1. 行为型设计模式——模板模式]()
> 
> [2. 行为型设计模式——解释器模式]()
> 
> [3. 行为型设计模式——策略模式]()
> 
> [4. 行为型设计模式——状态模式]()
> 
> [5. 行为型设计模式——观察者模式]()
> 
> [6. 行为型设计模式——备忘录模式]()
> 
> [7. 行为型设计模式——中介者模式]()
> 
> [8. 行为型设计模式——命令模式]()
> 
> [9. 行为型设计模式——访问者模式]()
> 
> [10. 行为型设计模式——责任链模式]()
> 
> [11. 行为型设计模式——迭代器模式]()

学好设计模式是阅读源码的必备基础，也是Android进阶的必经之路。学好它任重而道远，还需静心沉淀。
