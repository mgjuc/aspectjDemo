# aspectj Demo

---

aspectj，代码织入形式的切面实现。

没有引用Spring Aop。Spring Aop是基于动态代理实现Aop。


利用aspectj-maven-plugin插件自动执行aspectj织入处理。

aspectj编译前织入脚本：
```bash
#!/usr/bin/env bash
ASPECTJ_WEAVER=/home/myths/.m2/repository/org/aspectj/aspectjweaver/1.8.13/aspectjweaver-1.8.13.jar
ASPECTJ_RT=/home/myths/.m2/repository/org/aspectj/aspectjrt/1.8.9/aspectjrt-1.8.9.jar
ASPECTJ_TOOLS=/home/myths/.m2/repository/org/aspectj/aspectjtools/1.8.9/aspectjtools-1.8.9.jar
 
java -jar $ASPECTJ_TOOLS -cp $ASPECTJ_RT -source 1.5 -sourceroots src/main/java/ -d target/classes
```




---

#### Rep

[原生AspectJ用法分析以及Spring-AOP原理分析](https://blog.csdn.net/maoyeqiu/article/details/108005473)
