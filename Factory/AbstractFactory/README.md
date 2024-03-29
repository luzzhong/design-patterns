**定义:**

抽象工厂模式，即Abstract Factory Pattern，提供一个创建一系列相关或相互依赖对象的接口，而无须指定它们具体的类；具体的工厂负责实现具体的产品实例

> 抽象工厂模式与工厂方法模式最大的区别：抽象工厂中每个工厂可以创建多种类的产品；而工厂方法每个工厂只能创建一类

**主要作用:**

允许使用抽象的接口来创建一组相关产品，而不需要知道或关心实际生产出的具体产品是什么，这样就可以从具体产品中被解耦。

**解决的问题:**

每个工厂只能创建一类产品

**使用步骤:**

步骤1： 创建抽象工厂类，定义具体工厂的公共接口；

步骤2： 创建抽象产品族类 ，定义抽象产品的公共接口；

步骤3： 创建抽象产品类 （继承抽象产品族类），定义具体产品的公共接口；

步骤4： 创建具体产品类（继承抽象产品类） & 定义生产的具体产品；

步骤5：创建具体工厂类（继承抽象工厂类），定义创建对应具体产品实例的方法；

步骤6：客户端通过实例化具体的工厂类，并调用其创建不同目标产品的方法创建不同具体产品类的实例


