## 简介
一个[aardio](https://www.aardio.com)的自定义库，用于获取多个屏幕的大小、位置等信息。
获取屏幕信息的源码参考了标准库**sys.monitor**，做了精简处理，仅保留了最核心的代码。
由于通过调用WinAPI来实现，如果在导入此库时报错，请先导入raw库。
## 用法
将源码放在工程目录下，使用下列代码导入即可：
```
import multiMonitors;
```
具体调用方法请参考语法智能提示或源代码。
## 代码示例
```java
multiMonitors.getSize(0,true);
/* 获取主屏幕的大小，返回宽度和高度。
参数1为屏幕编号，0为主屏幕。
参数2为true表明获取到的区域大小是扣除了任务栏的。*/
```