### 使用方法
1、定义代理启动方法

META-INF/MANIFEST.MF:Agent-Class   代理类

META-INF/MANIFEST.MF:Premain-Class 代理方法 


2、打包命令

source ~/.bash_profile

mvn assembly:assembly -f pom.xml 


3、启动项目配置如下命令

-javaagent:'打包生成的地址'

-javaagent:/Users/devjys/Desktop/WorkSpaces/LearnWorkSpaces/com-jys-arithmetic/javaagent-demo/target/com-jys-javaagent-demo-0.0.1-SNAPSHOT-jar-with-dependencies.jar