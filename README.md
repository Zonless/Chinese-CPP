# Chinese-CPP
用中文编写c++代码
## 使用样例1(A+B Problem)：
```cpp
#include"chinese.h"
#include 库
使用 命名空间 标准
整数 主函数{
	整数 苹果，香蕉；
	输入 苹果 与 香蕉；
	输出 苹果 加 香蕉；
	返回 0；
}
```
## 使用样例2(BIT 即 树状数组)：
```cpp
#include "chinese.h"
使用 命名空间 标准 ；
整型 长度 ， 问题数 ， 树状数组 [ 1005 ] ；
整型 范围 （ 整型 某 ） {
	返回 某 按位与 （ 减 某 ） ；
}
无返回 添加 （ 整型 位置 ， 整型 数值 ）
{
	条件循环 （ 位置 小于等于 长度 ） {
		树状数组 [ 位置 ] 赋予 树状数组 [ 位置 ] 加 数值 ；
		位置 赋予 位置 加 范围 （ 位置 ） ；
	}
}
整型 询问 （ 整型 左界 ， 整型 右界 ）{
	长整数 左答案 赋予 0 ， 右答案 赋予 0 ；
	左界 赋予 左界 减 1 ；
	如果 （ 左界 大于 右界 ） {
		返回 -1 ；
	}
	条件循环 （ 左界 ） {
		左答案 赋予 左答案 加 树状数组 [ 左界 ] ；
		左界 赋予 左界 减 范围 （ 左界 ） ；
	}
	条件循环 （ 右界 ） {
		右答案 赋予 右答案 加 树状数组[ 右界 ] ；
		右界 赋予 右界 减 范围 （ 右界 ） ；
	}
	返回 右答案 减 左答案 ；
}
整型 主函数 {
	输入 长度 右移 问题数 ；
	有终循环 （ 整型 指针 赋予 1 ； 指针 小于等于 长度 ； 指针 赋予 指针 加 1 ） {
		整型 缓存 ；
		输入 缓存 ；
		添加 （ 缓存 ， 指针 ） ；
	}
	有终循环 （ 整型 指针 赋予 1 ； 指针 小于等于 问题数 ； 指针 赋予 指针 加 1 ） {
		整型 左界 ， 右界 ；
		输入 左界 右移 右界 ；
		输出 询问 （ 左界 ， 右界 ） ；
	}
	返回 0 ；
}
```
