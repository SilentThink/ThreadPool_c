线程池错误：

![image-20231125161644963](C:\Users\27646\AppData\Roaming\Typora\typora-user-images\image-20231125161644963.png)

没有连接动态库

gcc 编译时 -lpthread	指定库的名字

vs编译前指定库

![image-20231125161758049](C:\Users\27646\AppData\Roaming\Typora\typora-user-images\image-20231125161758049.png)

![image-20231125161902169](C:\Users\27646\AppData\Roaming\Typora\typora-user-images\image-20231125161902169.png)

# 解决C语言重复定义：multiple definition of“xxx”问题

产生这个错误的原因是**重复定义**

在threadpool.h中

const int NUMBER = 2;

threadpool.c和main.c中都include "threadpool.h"

导致

multiple definition of NUMBER