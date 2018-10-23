# windows--jdk
windows环境配置jdk环境变量

下载jdk安装包，默认安装（记下安装目录）

安装完JDK后配置环境变量  计算机→属性→高级系统设置→高级→环境变量

系统变量→新建 JAVA_HOME 变量 。
变量值填写jdk的安装目录（本人是 E:\Java\jdk1.7.0)

在系统变量区域，选择“新建”，输入变量名“CLASSPATH”；变量值：“.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;”。请注意变量值中，前面的“点“和”分号”，可以直接复制此变量值。然后点击“确定”。

系统变量→寻找 Path 变量→编辑
在变量值最后输入 %JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;
（注意原来Path的变量值末尾有没有;号，如果没有，先输入；号再输入上面的代码）
