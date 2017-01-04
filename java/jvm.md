#JVM
##  1   概述
   1.1 关键词
   - jvm: java virtual machine           #java虚拟机
   - jre: java run-time environment      #java运行时环境
   - jdk: java development kit           #java开发组件
   - jit: just-in-time compilation       #即时编译
   
   1.2  知识点
   - jvm内存模型
   - gc:垃圾收集器
   - 类加载机制
   - jvm性能监控及调优
##  2   java内存模型
    Java虚拟机在执行java程序运行的过程中会把所管理的内存划分为若干个不同的区域
   ![内存模型](https://raw.githubusercontent.com/ch15084/study/master/imgs/jvm_memory_1.png "内存模型图")

1.   线程私有区
-   程序计数器:  记录正在执行的虚拟机字节码的地址
-   虚拟机栈:   方法执行的内存区，每个方法执行时会在虚拟机栈中创建栈帧
-   本地方法栈:  虚拟机的Native方法执行的内存区
2.  线程共享区
-   java堆:  对象分配内存的区域
-   方法区:    存放类信息、常量、静态变量、编译器编译后的代码等数据
    -    常量池：存放编译器生成的各种字面量和符号引用，是方法区的一部分


