# java-Experiment-One
一、实验目的
1. 基本掌握本人所选择的集成开发工具的使用方法；
2. 利用给出的指定源代码，在开发工具中组织、初步理解并运行；
3. 理解、掌握创建包的方法；
4. 初步了解类的实例化方法；
5. 在本人实验代码平台撰写 readme 报告，对类进行分析，描写实验过程。
二、实验方法
1. 实验环境准备
使用  VS Code。
确保已安装 JDK（建议 JDK 8 或以上版本）。
2. 代码组织步骤
创建一个 Java 项目，命名为 BankingSystem。
在项目中创建包（package）名为 banking。
在 banking 包中分别创建三个类文件：
Account.java
Customer.java
TestBanking.java
编译并运行 TestBanking 类，观察控制台输出。
3. 程序运行与调试
运行 TestBanking 类，检查输出是否符合预期。
若出现编译错误，检查包名、类名、语法是否正确。
可通过调试模式逐步执行，理解对象创建和方法调用的流程。
三、类的设计分析
1. Account 类
职责：模拟银行账户的基本操作。
属性：
balance：账户余额（private double）。
方法：
Account(double bal)：构造方法，初始化余额。
getBalance()：获取当前余额。
deposit(double amount)：存款方法，返回操作成功标志。
withdraw(double amount)：取款方法，若余额不足则失败。
2. Customer 类
职责：表示银行客户，关联一个账户。
属性：
firstName、lastName：客户姓名（private String）。
account：客户持有的账户（private Account）。
方法：
构造方法初始化姓名。
getAccount() / setAccount(Account acct)：用于关联账户。
getFirstName() / getLastName()：获取姓名。
3. TestBanking 类
职责：测试类，模拟客户开户、存款、取款等业务流程。
方法：
main(String[] args)：程序入口，创建客户和账户，执行一系列交易并输出结果。
4. 类之间的关系
Customer 类中包含一个 Account 类型的成员变量，体现组合关系。
TestBanking 类通过创建 Customer 和 Account 对象，模拟业务逻辑流程。
四、程序调试及运行结果
<img width="2559" height="1522" alt="image" src="https://github.com/user-attachments/assets/e728dc64-817c-4c64-bf67-9d07b37fa4f7" />

五、实验感想
通过本次实验，我初步掌握了以下内容：
Java 包的使用：理解了包的作用在于组织类、避免命名冲突，并通过 package 和 import 语句实现模块化管理。
面向对象的基本概念：学会了如何设计类、定义属性和方法，理解封装的重要性。
对象之间的协作：通过 Customer 与 Account 的关联，体会到对象之间如何通过引用来交互。
初步的调试与测试能力：通过运行 TestBanking 类，验证了程序的正确性，并学会了基本的输出调试方法。
本次实验为我后续学习面向对象编程和复杂系统设计打下了基础。
