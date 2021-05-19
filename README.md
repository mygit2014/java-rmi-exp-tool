-------------------------------JAVA RMI反序列化漏洞利用工具----------------------------------
![image](https://raw.githubusercontent.com/msx2009/RMIAllExpTools/master/1.jpg)
![image](https://raw.githubusercontent.com/msx2009/RMIAllExpTools/master/2.jpg)
主要功能：

一、检测所有回显Payload

使用方法：

填写IP和端口，点击 检测所有回显Payload，程序自动检测 cc1-cc7 基于回显的Payload，

可用的payload将自动添加到 回显可以Payload 列表，接着就可以执行命令和上传文件了

二、检测单个Payload

使用方法： 

UnicastRemoteObjectBypass8u231 和 UncastRefForBypassJEP290 是反弹Payload，

1、JRMP监听

填写监听端口，选择Payload，开始监听

2、填写Payload参数，点击开始检测

如果存在漏洞，会接收到反弹连接

3、反弹之后检测是否可以利用，点击 检测是否可利用


其他payload，直接点 开始检测


三、方法参数反序列化漏洞

1、获取 RMI regNames，获取后，填写接口相应方法（函数）信息

如果本地存在远程接口的话，会自动填写方法信息，

不存在的话，就需要自己想办法去找远程接口可能会存在的方法

如果方法（函数）参数里有不是基本类型和String类型的参数就可以反序列化攻击

2、选择Payload，点击 方法信息 后的检测,如果漏洞存在，就可以执行命令了

可用payload自动增加到回显可用Payload

