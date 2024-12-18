KeaTest
===========================

KeaTest 是提供给用户编写性质的测试类。继承 KeaTest 就创建了一个测试样例。

在继承的 KeaTest 子类中，我们编写对应的函数，并通过装饰器的方式定义性质中的初始化函数(Initializer)、
前置条件(Precodition)、交互场景(Rule)和主路径函数(MainPath)。

KeaTest 本质上是为用户提供了一个容器，Kea会在此容器中寻找用户自定义的性质，并将其加载入 Kea 中。
